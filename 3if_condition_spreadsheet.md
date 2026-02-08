# 𖣘 𝐍8𝐍 – 𝐖𝐎𝐑𝐊𝐅𝐋𝐎𝐖 𝐒𝐄𝐓𝐔𝐏 𝐄𝐗𝐏𝐋𝐀𝐍𝐀𝐓𝐈𝐎𝐍 (Google Sheets + IF Condition)


## ➺STEP 1:


Open n8n and Sign Up / Sign In to your account.



## ➺STEP 2:


Click “Add first step” to start creating your workflow.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_40_50" src="https://github.com/user-attachments/assets/d060834c-045b-4068-b555-fa024482c0f6" />


## ➺STEP 3:


+ Search for “Manual Trigger” and add it.
  
<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_44_52" src="https://github.com/user-attachments/assets/cf44f824-1267-47d9-b38f-f4e1fbc50ae6" />

+ 🟢 This trigger allows you to run the workflow manually for testing.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_46_49" src="https://github.com/user-attachments/assets/7bc12608-c313-438e-bc33-cf779f254df8" />


## ➺STEP 4:


+ Click on “+ Add node” again 
→ search for “Google Sheets”

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_48_14" src="https://github.com/user-attachments/assets/a0d3f04e-174e-4d12-9298-b76cfd1ff6ff" />


→ select “Getrow” operation and connect it to the Manual Trigger node.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_48_49" src="https://github.com/user-attachments/assets/febc387e-db10-40e3-982b-4ba2586f3c5c" />


## ➺STEP 5:


+ On the Google Sheets node, you will see the following parameters:




+ Credentials to connect with



+ Resource




+ Operation




+ Document




+ Sheet


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_49_57" src="https://github.com/user-attachments/assets/1b9fd9b9-5942-4def-8a14-56e878af1645" />



## ➺STEP 6:


+ Fill the parameters one by one:


🔹 Credentials – Connect your Google account so n8n can access your Google Sheets.


🔹 Resource – Select what you want to work with:




+ Document




+ Sheet

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_51_25" src="https://github.com/user-attachments/assets/25ffe32b-d0d8-4139-b1e2-36a29eb918a9" />



🔹 Operation – Choose what action you want to perform:




+ Append




+ Delete




+ Create




+ Update, etc.


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_53_40" src="https://github.com/user-attachments/assets/2bf11102-2351-4d55-80b9-dfe04272dfce" />


🔹 Document – Select document using:



+ From list


+ By ID




+ By URL


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_54_26" src="https://github.com/user-attachments/assets/2bd0ca26-ec01-4907-934f-0c75bdcca8ec" />



## ➺STEP 7:


+ Select Sheet using one of the following:




+ From list




+ By URL




+ By ID




+ By Name


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_55_00" src="https://github.com/user-attachments/assets/5ab43772-c73c-43b3-91cb-a69053d8ce99" />



## ➺STEP 8:
+ Click Execute step 


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_56_09" src="https://github.com/user-attachments/assets/76bdc236-9f95-495f-86ef-3a8a861b4375" />



# ♨ 𝐍𝐎𝐖 𝐀𝐃𝐃𝐈𝐍𝐆 𝐓𝐇𝐄 🅘🅕 𝐂𝐎𝐍𝐃𝐓𝐈𝐎𝐍 𝐓𝐎 𝐍𝐎𝐃𝐄:


## ➺STEP 9:


+ Click “Add node” again → search “IF (Condition)” and add it.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_57_56" src="https://github.com/user-attachments/assets/1044989c-44ef-42ac-9f4d-5275762b5e65" />


## ➺STEP 10:


+ The IF node will display Conditions.

+ Choose one type depending on your data:


+ String


+ Number


+ Date & Time


+ Boolean


+ Array


+ Object


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_58_41" src="https://github.com/user-attachments/assets/62102b02-7da3-4fd5-afdc-75dd429c5f09" />



## ➺STEP 11:


+ After choosing the type, select a specific condition.

+ Example:




+ Equals




+ Contains




+ Greater than




+ Less than, etc.


<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 09_59_24" src="https://github.com/user-attachments/assets/83bd46d8-6955-4664-a3fb-8f6960242f19" />


## ➺STEP 12:


+ Enter the value for the condition based on what you want to compare.

+ Example: If marks > 40 or if name = “John”, etc.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_00_03" src="https://github.com/user-attachments/assets/060ec313-e3c7-4811-be76-efca3e3b59ad" />


## ➺STEP 13:


+ Click Execute Node to run the IF condition.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_00_50" src="https://github.com/user-attachments/assets/4dffddba-2ccd-4d61-bb5f-b93cc26431e0" />


## ➺STEP 14:


+ After execution if incase you want , the IF node separates the output into:




+ True




+ False



<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_02_41" src="https://github.com/user-attachments/assets/0214657b-6c13-4dbc-98c7-cda751ddb41e" />


## ➺STEP 15:

+ now you have to add "append row " to both true and false buttons .

+ search append row and add it to true button .

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_04_13" src="https://github.com/user-attachments/assets/f401ce38-52ef-420c-af1b-2ce8fea4d61c" />


+ it shows some parameters same like above get row parameters .

 <img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_05_58" src="https://github.com/user-attachments/assets/bd3cbb99-39d3-438e-8473-43f6a913a3b6" />



+ give same sheets what you was gave above get operation.

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_07_31" src="https://github.com/user-attachments/assets/4ad3377f-4971-4d0c-9419-f68d79a6e285" />


+after you on map automatically.

## ➺STEP 16 :

+ Click Execute step

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_13_10" src="https://github.com/user-attachments/assets/8ca445f2-454d-41af-9dfd-ecbb334eff06" />


## ➺STEP 17 :

+ now you have do same process for false button 

+ add append , give same sheets and click  Execute step 

<img width="1920" height="1032" alt="Editing n8n_if_condition_spreadsheet md at main · lodagalarajesh_n8n - Google Chrome 23-11-2025 10_15_21" src="https://github.com/user-attachments/assets/2c6b6304-6a06-4a39-a39c-d1a28ab6fec0" />


+ So final result:




+ All values that satisfy the condition → stored in True Sheet




+ All values that don’t satisfy → stored in False Sheet

# ☯ 𝐅𝐈𝐍𝐀𝐋  𝐖𝐎𝐑𝐊𝐅𝐋𝐎𝐖 𝐖𝐈𝐋𝐋 𝐁𝐄 𝐋𝐎𝐎𝐊𝐈𝐍𝐆 𝐋𝐈𝐊𝐄 𝐓𝐇𝐈𝐒 ࿐:

<img width="1920" height="1032" alt="▶️ My workflow 3 - n8n - Google Chrome 23-11-2025 10_16_16" src="https://github.com/user-attachments/assets/9f8b4210-14e9-475e-88af-b350dc7a823f" />

