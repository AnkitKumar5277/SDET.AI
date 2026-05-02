<img width="742" height="431" alt="image" src="https://github.com/user-attachments/assets/32f20c84-32ad-4be6-bc90-b845e2974c4f" />

<img width="923" height="416" alt="image" src="https://github.com/user-attachments/assets/7b931ba3-82b3-4995-b2bd-cb6dd2034b7e" />

Input : Fetch the JIRA ID and generate the 10 testcases and upload them to the excel file

# Memory -> simple memory
Context Window Length 5 remember last 5 conversation

# Tool -> Jira
Select Operation Get Many, Get, Fetch, etc, 

NOTE: if there is space in your project name then remove middle spaces.
Select JQL: project = Android16 ORDER BY created DESC

<img width="324" height="531" alt="image" src="https://github.com/user-attachments/assets/1347b3a0-1e08-4e1e-ae68-fb94aeadff29" />

# AI Agent 

AI Agent me System message me batana :

here is my details -

QA Name : Pramod Dutta

You will get the query via the Chat trigger, Your task is to first find the all the JIRA ids from the tool "GET JIRA IDS" and based on the user query, You have to create the unique Testcases and upload them to the Tool "TestCase Sheet" one by one, make sure that testcases are unique and no duplicate are added in the sheet

Input : Fetch the JIRA IDs from a project and based on the JIRA IDs, create the test cases and upload them to the Excel file. You also have to read the Google Doc where I have mentioned about my project details


we have successfully created our first AI agent which, based on the chat, it can create a JIRA ticket
