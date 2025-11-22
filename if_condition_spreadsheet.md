# N8N – Workflow Setup Explanation (Google Sheets + IF Condition)


Step 1:


Open n8n and Sign Up / Sign In to your account.



Step 2:


Click “Add first step” to start creating your workflow.



Step 3:


Search for “Manual Trigger” and add it.

🟢 This trigger allows you to run the workflow manually for testing.



Step 4:


Click on “+ Add node” again → search for “Google Sheets” → select “Append” operation and connect it to the Manual Trigger node.



Step 5:


On the Google Sheets node, you will see the following parameters:




Credentials to connect with




Resource




Operation




Document




Sheet





Step 6:


Fill the parameters one by one:


🔹 Credentials – Connect your Google account so n8n can access your Google Sheets.


🔹 Resource – Select what you want to work with:




Document




Sheet




🔹 Operation – Choose what action you want to perform:




Append




Delete




Create




Update, etc.




🔹 Document – Select document using:




From list




By ID




By URL





Step 7:


Select Sheet using one of the following:




From list




By URL




By ID




By Name





Step 8:


Next, you will see Mapping Column Mode. You have two options:




Map Each Column Manually

→ You need to provide values for each column manually.




Map Automatically

→ It will automatically detect incoming data and match it with Google Sheet columns.





Step 9:


After mapping columns, click “Execute Node” to test and ensure data is added to your Google Sheet.



🔀 Now Adding the IF Condition Node


Step 10:


Click “Add node” again → search “IF (Condition)” and add it.



Step 11:


The IF node will display Conditions.

Choose one type depending on your data:




String




Number




Date & Time




Boolean




Array




Object





Step 12:


After choosing the type, select a specific condition.

Example:




Equals




Contains




Greater than




Less than, etc.





Step 13:


Enter the value for the condition based on what you want to compare.

Example: If marks > 40 or if name = “John”, etc.



Step 14:


Click Execute Node to run the IF condition.



Step 15:


After execution, the IF node separates the output into:




True




False





Step 16:


You can send:




True output to a separate Google Sheet




False output to another Google Sheet




So final result:




All values that satisfy the condition → stored in True Sheet




All values that don’t satisfy → stored in False Sheet


