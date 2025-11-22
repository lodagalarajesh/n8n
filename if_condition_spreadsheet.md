# N8N – Workflow Setup Explanation (Google Sheets + IF Condition)


## ➺STEP 1:


Open n8n and Sign Up / Sign In to your account.



## ➺STEP 2:


Click “Add first step” to start creating your workflow.



## ➺STEP 3:


+ Search for “Manual Trigger” and add it.

+ 🟢 This trigger allows you to run the workflow manually for testing.



## ➺STEP 4:


+ Click on “+ Add node” again 
→ search for “Google Sheets” 
→ select “Getrow” operation and connect it to the Manual Trigger node.



## ➺STEP 5:


+ On the Google Sheets node, you will see the following parameters:




+ Credentials to connect with




+ Resource




+ Operation




+ Document




+ Sheet





## ➺STEP 6:


+ Fill the parameters one by one:


🔹 Credentials – Connect your Google account so n8n can access your Google Sheets.


🔹 Resource – Select what you want to work with:




+ Document




+ Sheet




🔹 Operation – Choose what action you want to perform:




+ Append




+ Delete




+ Create




+ Update, etc.




🔹 Document – Select document using:




+ From list




+ By ID




+ By URL





## ➺STEP 7:


+ Select Sheet using one of the following:




+ From list




+ By URL




+ By ID




+ By Name





## ➺STEP 8:
+ Click Execute step 





# 🔀 Now Adding the 🅘🅕 Condition Node


## ➺STEP 9:


+ Click “Add node” again → search “IF (Condition)” and add it.



## ➺STEP 10:


+ The IF node will display Conditions.

+ Choose one type depending on your data:




+ String




+ Number




+ Date & Time




+ Boolean




+ Array




+ Object





## ➺STEP 11:


+ After choosing the type, select a specific condition.

+ Example:




+ Equals




+ Contains




+ Greater than




+ Less than, etc.





## ➺STEP 12:


+ Enter the value for the condition based on what you want to compare.

+ Example: If marks > 40 or if name = “John”, etc.



## ➺STEP 13:


+ Click Execute Node to run the IF condition.



## ➺STEP 14:


+ After execution if incase you want , the IF node separates the output into:




+ True




+ False





## ➺STEP 15:

+ now you have to add "append row " to both true and false buttons 

+ search append row and add it to true button .

+ it shows some parameters same like above get row parameters .

+ give same sheets what you was gave above get operation.

+after you on it manually 

## ➺STEP 16 :

+ Click Execute step 

## ➺STEP 17 :

+ now you have do same process for false button 

+ add append , give same sheets and click  Execute step 


+ So final result:




+ All values that satisfy the condition → stored in True Sheet




+ All values that don’t satisfy → stored in False Sheet

# FINAL WORKFLOW WILL BE LOOKING LIKE THIS:


