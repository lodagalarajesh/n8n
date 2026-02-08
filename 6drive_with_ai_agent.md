# “Automated Document Ingestion and Querying System Using Vector Embeddings”
## PART 1: DATA INGESTION PIPELINE (Left side)

This part automatically takes files from Google Drive and stores their knowledge in Pinecone.

Step 1: Google Drive Trigger

Node: Google Drive Trigger (fileCreated)

Watches a specific Google Drive folder.

Triggers automatically whenever a new file is uploaded.

+ Purpose: Start the workflow as soon as new data arrives.

Step 2: Download File

Node: Download file

Downloads the newly created file from Google Drive.

Converts it into a format that can be processed downstream.

+ Purpose: Get the actual file content into the workflow.

Step 3: Default Data Loader

Node: Default Data Loader

Reads the downloaded file (PDF, DOCX, TXT, etc.).

Extracts raw text from the document.

+ Purpose: Convert files → readable text.

Step 4: Recursive Character Text Splitter

Node: Recursive Character Text Splitter

Breaks large text into small overlapping chunks.

Helps improve embedding quality and retrieval accuracy.

+ Purpose: Prepare text chunks suitable for embeddings.

Step 5: Generate Embeddings

Node: Embeddings OpenAI

Converts each text chunk into a vector embedding using OpenAI.

Each chunk becomes a numerical representation.

+ Purpose: Make text searchable using vector similarity.

Step 6: Store in Pinecone

Node: Pinecone Vector Store

Stores:

Text chunks

Their embeddings

Metadata (source, filename, etc.)

+ Purpose: Persist knowledge in a vector database for fast retrieval.

 Result:
Your Google Drive documents are now indexed and searchable in Pinecone.

## PART 2: CHAT + RETRIEVAL PIPELINE (Right side)

This part handles user questions and fetches relevant knowledge from Pinecone.

Step 7: When Chat Message Received

Node: When chat message received

Triggers whenever a user sends a message in the chat UI.

+ Purpose: Start the question-answer flow.

Step 8: AI Agent

Node: AI Agent

Acts as the brain of the system.

Orchestrates:

User question

Retrieval from Pinecone

Final response generation

+ Purpose: Decide how to answer the question.

Step 9: Retrieve Relevant Context from Pinecone

Node: Pinecone Vector Store1

Takes the user query.

Converts it into embeddings (via OpenAI).

Performs similarity search in Pinecone.

Returns the most relevant document chunks.

+ Purpose: Fetch only relevant knowledge for the query.

Step 10: OpenAI Chat Model

Node: OpenAI Chat Model

Receives:

User’s question

Retrieved context from Pinecone

Generates a grounded, context-aware answer.

+ Purpose: Produce accurate answers using your documents.

FINAL OUTPUT

The user sees a natural language response in the chat.

Example shown:

Question: “WHO IS MS DHONI?”

Answer generated using LLM (and Pinecone if relevant docs exist).
<img width="1920" height="1035" alt="Screenshot 2026-02-05 210216" src="https://github.com/user-attachments/assets/fde339f8-2e02-4ff1-aec6-2e4d00191a08" />
