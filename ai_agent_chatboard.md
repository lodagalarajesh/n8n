# ⭐ How to Build an AI Agent Chat Workflow in n8n (Step-by-Step Guide)

+ This guide explains how to create a public AI chat endpoint using Chat Trigger, AI Agent, Chat Model, and Memory in n8n.

## Step 1: Sign Up or Log In

+ Go to n8n.io, create an account, and log in.
+ After logging in, you will be taken to your workspace dashboard.

## Step 2: Create a New Workflow

+ On your dashboard, click New Workflow.
+ click add first step 
<img width="1920" height="1032" alt="New File at _ · lodagalarajesh_n8n - Google Chrome 21-11-2025 02_59_47 PM" src="https://github.com/user-attachments/assets/64b99191-3366-497e-9277-ed819a197f11" />

## Step 3: Choose a Trigger

+ After clicking add first step , n8n will ask:

+ “What trigger would you like to start with?”

+ In the search bar, type Chat trigger .
  
<img width="1920" height="1032" alt="New File at _ · lodagalarajesh_n8n - Google Chrome 21-11-2025 02_58_22 PM" src="https://github.com/user-attachments/assets/597a0559-3fc0-429e-9fd9-c89c2c386dff" />

## Step 4: Add the Chat Trigger

+ Select Chat Trigger and add it to your workflow.

+ This trigger receives messages from a public chat URL (or can be used to embed a chat widget later).

## Step 5: Configure Chat Trigger

+ Once added, the Chat Trigger will show a parameter:

+ Make Chat Publicly Available

+ Enable this option (turn it ON).

+ This generates a public chat endpoint that anyone can use to communicate with your workflow.

+ Click Check Test to verify that the endpoint is active.
  
<img width="1920" height="1032" alt="New File at _ · lodagalarajesh_n8n - Google Chrome 21-11-2025 03_02_00 PM" src="https://github.com/user-attachments/assets/bf635c92-98e3-40bf-8adc-45865a04b0b7" />


## Step 6: Add an AI Agent

+ Now add a second node:

+ + → AI → AI Agent

+ Link the Chat Trigger to the AI Agent by connecting the nodes.

+ The Chat Trigger will now send incoming chat messages directly into the AI Agent.
  
<img width="1920" height="1032" alt="Node js — Download Node js® - Google Chrome 21-11-2025 03_07_31 PM" src="https://github.com/user-attachments/assets/fe2317da-f49f-4293-b68a-900a8be08e7a" />


## Step 7: AI Agent Structure
+ after adding it shows parameters but you you just click execute step
  
<img width="1920" height="1032" alt="Workflow Automation - n8n - Google Chrome 21-11-2025 03_09_19 PM" src="https://github.com/user-attachments/assets/d123beef-b856-4195-a3dc-9b19cb773d20" />

+ The AI Agent node contains three main components:

+ Chat Model – the LLM you want to use

+ Memory – optional storage for conversation history

+ Tools – optional actions your agent can perform (API calls, code, databases, etc.)

+ You will now configure each part.
  
<img width="1920" height="1032" alt="Workflow Automation - n8n - Google Chrome 21-11-2025 03_09_51 PM" src="https://github.com/user-attachments/assets/78b5bd8c-65c1-49fc-b285-02a6fef5d053" />

## Step 8: Add a Chat Model (Example: Gemini)

+ Inside the AI Agent, click Add Chat Model.

+ Search for Gemini Chat Model and add it.
  

<img width="1920" height="1032" alt="Workflow Automation - n8n - Google Chrome 21-11-2025 03_10_34 PM" src="https://github.com/user-attachments/assets/2de1fb2f-967b-4e19-a9e8-d433f8b96d19" />

## Step 9: Configure Model Parameters

+ Once added, the Gemini Chat Model shows two main parameters:

+ Choose your Gemini API key.
+ If it is not created yet:

+ Click Add Credential

+ Paste your Gemini API Key

+ Model

+ Select the Gemini model you want to use (example: gemini-1.5-flash, gemini-1.5-pro, etc.).
  
<img width="1920" height="1032" alt="Workflow Automation - n8n - Google Chrome 21-11-2025 03_11_56 PM" src="https://github.com/user-attachments/assets/acd1c914-edc9-4697-a78a-15e13189049b" />

## Step 10: Add Memory (Optional but Recommended)

+ Inside the AI Agent panel, click Add Memory.

+ Choose any memory type depending on your workflow needs.
  
<img width="1920" height="1032" alt="Workflow Automation - n8n - Google Chrome 21-11-2025 03_12_49 PM" src="https://github.com/user-attachments/assets/83babc69-780f-46c1-9d64-b2513a357ff1" />

## Step 11: Execute the Workflow

+ Once everything is connected:

+ Chat Trigger → AI Agent

+ AI Agent → Chat Model + Memory

+ Click Execute Step on the Chat Trigger.
  # YOUR  FINAL WORKFLOW LOOK LIKE THIS
  <img width="1920" height="1032" alt="New File at _ · lodagalarajesh_n8n - Google Chrome 21-11-2025 02_55_05 PM" src="https://github.com/user-attachments/assets/041757fb-92e6-4ff1-824b-250d25acee99" />
