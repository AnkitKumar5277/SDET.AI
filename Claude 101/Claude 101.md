

# Claude 101 Study Guide – Simple Hinglish

## 1. Claude kya hai?

Claude ek AI Assistant hai jo Anthropic ne banaya hai.

Simple words mein:

* LLM = Brain → Questions samajhta aur answer deta hai.

* AI Agent = Brain + Memory + Tools → Sirf answer nahi deta, balki tools use karke kaam bhi kar sakta hai.

Claude ka main principle hai:

* Helpful → Help kare.

* Harmless → Harmful cheezein na kare.

* Honest → Jo pata hai wahi bole.

Claude ko chatbot se zyada thought partner samjho. Complex problems solve karne mein help karta hai.

Pasted markdown.md

### Claude kis kaam mein achha hai?

|
Kaam

|

Example

|
| --- | --- |
|

Writing

|

Email, report, social post

|
|

Research

|

Information collect aur analyze

|
|

Coding

|

Code likhna, debug karna

|
|

Problem solving

|

Complex issues solve

|
|

Learning

|

Kisi topic ko simple way mein samjhana

|

Claude ek conversation mein 200K+ tokens, yani roughly 500+ pages tak ka context handle kar sakta hai.

Pasted markdown.md

# 2. Effective Prompt kaise likhein?

Golden rule:

Claude se coworker ki tarah baat karo.

Prompt ke 3 parts yaad rakho:

## Stage + Task + Rules

### Stage (Context)

Claude ko batao:

* Tum kaun ho?

* Tumhara role kya hai?

* Background kya hai?

Example:

> Main QA Engineer hoon.

### Task

Exactly kya chahiye?

Example:

> Website ke liye test plan banao.

### Rules

Output kaisa chahiye?

Example:

* Professional tone

* Jira format

* Table format

### Simple Formula

> Context + Kaam + Expected Output

Example:

> Main QA Engineer hoon. Ek e-commerce website ke liye production-ready test plan banao. Jira-compatible table format mein do.

Ye vague prompt se kaafi better result deta hai.

Pasted markdown.md

# 3. Agar Claude galat answer de to?

Pehla answer final nahi hota.

Tum:

* Follow-up question pooch sakte ho.

* Specific feedback de sakte ho.

* Direction change kar sakte ho.

* New chat start kar sakte ho.

Bad feedback:

> Make it better.

Good feedback:

> First 2 paragraphs hatao aur conclusion ko action-oriented banao.

Specific feedback se better output milta hai.

Pasted markdown.md

# 4. AI Fluency – 4D Framework

Ye exam ke liye important hai.

## 4D = Delegation, Description, Discernment, Diligence

|
D

|

Simple Meaning

|
| --- | --- |
|

Delegation

|

Decide karna kaunsa kaam AI ko dena hai

|
|

Description

|

AI ko clearly instructions dena

|
|

Discernment

|

AI ke answer ko check karna

|
|

Diligence

|

AI ko responsibly use karna

|

### Easy Example (QA)

* Delegation: Test cases AI se banwao.

* Description: Clear requirements do.

* Discernment: Generated test cases review karo.

* Diligence: Sensitive data AI mein upload mat karo.

Memory trick:

> D-D-D-D = Decide, Describe, Detect, Do responsibly
>
> Pasted markdown.md

# 5. Claude Desktop App ke Modes

Claude ke 3 main modes hain.

## Chat

Best for:

* Quick questions

* Brainstorming

* Drafting

Example:

> Selenium wait explain karo.

## Cowork

Best for:

* Long projects

* Research

* Documents

Features:

* Folder access

* Scheduled tasks

* Browser use

* Plugins

Example:

> Is folder ke documents analyze karke report banao.

## Code

Best for developers.

3 modes:

* Ask → Suggestion deta hai.

* Code → Changes apply karta hai.

* Plan → Pehle plan batata hai.

|
Mode

|

Best For

|
| --- | --- |
|

Chat

|

Quick questions

|
|

Cowork

|

Research & documents

|
|

Code

|

Software development

|

Pasted markdown.md

# 6. Projects

Project ek dedicated workspace hota hai.

Iske andar:

* Apni memory

* Chats

* Files

* Instructions

Sab alag rehte hain.

### Example

Project Name: Jobsarathi QA

Upload:

* Requirement docs

* Test plan

* Bug templates

* API docs

Instruction:

> Hamesha QA expert ki tarah answer do.

Ab har chat mein same context use hoga.

Pasted markdown.md

### Project banane ke 3 steps

1. Project create karo.

2. Instructions likho.

3. Knowledge files upload karo.

# 7. RAG kya hai?

Jab Project mein bahut saare documents ho jaate hain, Claude sabko ek saath nahi padhta.

Instead:

1. Question samajhta hai.

2. Relevant documents find karta hai.

3. Sirf useful information use karta hai.

Isko RAG (Retrieval Augmented Generation) kehte hain.

Simple example:

100 PDFs hain.

Question:

> Login bug ke baare mein batao.

Claude sirf login-related docs retrieve karega.

Pasted markdown.md

# 8. Artifacts

Artifacts matlab Claude ka standalone output.

Chat ke andar buried nahi hota, alag window mein milta hai.

Examples:

* Document

* Code

* HTML page

* SVG

* Mermaid diagram

* React component

Example:

> Monthly expense tracker banao.

Claude interactive artifact create kar sakta hai.

Artifact ko:

* View

* Edit

* Copy

* Download

* Share

kar sakte ho.

Pasted markdown.md

# 9. Skills

Skills ko Claude ki specialized abilities samjho.

Jaise kisi employee ko SOP diya ho.

Skill mein ho sakta hai:

* Instructions

* Scripts

* Templates

* Resources

### Types

Anthropic Skills

Claude company ke predefined skills.

Examples:

* Excel file banana

* Word document

* PowerPoint

* PDF

Custom Skills

Tum khud bana sakte ho.

Example QA:

* Test Plan Generator

* Bug Report Generator

* Hotfix Validator

Ek baar skill bana diya to repeat kaam faster ho jata hai.

Pasted markdown.md

# Exam Quick Revision

Claude

AI assistant based on Constitutional AI.

Prompt Formula

Stage + Task + Rules.

4D Framework

Delegation, Description, Discernment, Diligence.

Chat

Quick questions and drafting.

Cowork

Complex research and long-running work.

Code

Software development with Ask, Code, and Plan modes.

Projects

Dedicated workspace with memory, files, and instructions.

RAG

Retrieves only relevant information from large knowledge bases.

Artifacts

Standalone outputs like documents, code, diagrams, and apps.

Skills

Reusable specialized workflows for repeat tasks.

## 30-Second Memory Trick

* Claude = AI thought partner

* Good Prompt = Context + Task + Rules

* 4D = Decide → Describe → Check → Responsible use

* Chat = Questions

* Cowork = Big work

* Code = Programming

* Project = Permanent workspace

* Artifact = Final reusable output

* Skill = Reusable expert workflow

Ye summary Claude 101 ke major concepts ko simple Hinglish mein cover karti hai aur revision ke liye useful hai.

Pasted markdown.md
