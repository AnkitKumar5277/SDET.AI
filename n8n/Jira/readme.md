
<img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/6caa440b-7311-46bc-898c-1b58e369f216" />

<img width="923" height="416" alt="image" src="https://github.com/user-attachments/assets/c969ebc1-64ae-4d61-940b-ccf1dabceb48" />

Input : Fetch the JIRA ID and generate the 10 testcases and upload them to the excel file

# Memory -> simple memory
Context Window Length 5 remember last 5 conversation

# Tool -> Jira
Select Operation Get Many, Get, Fetch, etc, 

NOTE: if there is space in your project name then remove middle spaces.
Select JQL: project = Android16 ORDER BY created DESC

<img width="300" height="500" alt="image" src="https://github.com/user-attachments/assets/f1ef9ea0-fcb0-4878-9baf-701d0aec015d" />

# AI Agent 

AI Agent me System message me batana :

here is my details -

QA Name : Pramod Dutta

You will get the query via the Chat trigger, Your task is to first find the all the JIRA ids from the tool "GET JIRA IDS" and based on the user query, You have to create the unique Testcases and upload them to the Tool "TestCase Sheet" one by one, make sure that testcases are unique and no duplicate are added in the sheet

Input : Fetch the JIRA IDs from a project and based on the JIRA IDs, create the test cases and upload them to the Excel file. You also have to read the Google Doc where I have mentioned about my project details


we have successfully created our first AI agent which, based on the chat, it can create a JIRA ticket
