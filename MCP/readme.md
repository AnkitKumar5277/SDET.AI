# What is MCP?

Model Context Protocol (MCP) is an open standard that allows AI models like ChatGPT, Claude, and other LLMs to securely connect with external tools, APIs, databases, and local files.

# When Should You Use MCP?

Use MCP when your AI needs to:

- Access databases
- Read or write files
- Call REST APIs
- Control a browser
- Use external tools
- Integrate with GitHub, Jira, Slack, etc.

# Without MCP

```text
AI → Gmail API
AI → GitHub API
AI → Database API
AI → File System API
AI → Slack API
```

# With MCP

```text
           AI
            │
        MCP Client
            │
    --------------------
    │    │    │    │
 Gmail GitHub SQL Files
   MCP    MCP   MCP  MCP
 Server Server Server Server
```

# MCP Architecture

```text
+----------------------+
|      AI Model        |
| (ChatGPT/Claude)     |
+----------+-----------+
           |
       MCP Client
           |
------------------------------
|            |               |
MCP Server  MCP Server   MCP Server
(Database)  (GitHub)      (Files)
```

# Main Components

## 1. MCP Client

The application that talks to the AI.

Examples:

- Claude Desktop
- VS Code
- Cursor
- AI Agent

## 2. MCP Server

Provides tools to the AI.

Example:

- Weather Tool
- Database Tool
- Calculator Tool
- File Reader

## 3. Tools

Functions the AI can call.

Example:

```python
search_products()
get_weather()
create_user()
read_file()
```

## Resources

Data exposed to AI.

Example:

- README.md
- config.json
- database records

## Prompts

Reusable prompt templates.

Example:

- Summarize this file.
- Explain this code.
- Generate test cases.

# Real Example

User asks:

> Show all employees from the HR department.

Without MCP

```text
AI
↓

"I cannot access your database."
```

With MCP

```text
User

↓

AI

↓

MCP Client

↓

SQL MCP Server

↓

SELECT * FROM employees
WHERE department='HR';

↓

Database

↓

Results

↓

AI Response
```

# What can an MCP Server do?

It can expose:

- ✅ APIs
- ✅ Database
- ✅ Local files
- ✅ GitHub
- ✅ Google Drive
- ✅ Gmail
- ✅ Slack
- ✅ Jira
- ✅ Playwright
- ✅ Docker

Almost anything.

# Playwright MCP Example

```text
User

↓

Open amazon.com

↓

Playwright MCP

↓

Browser Opens

↓

Take Screenshot

↓

Return Image
```

# GitHub Example

```text
AI

↓

List my repositories

↓

GitHub MCP Server

↓

GitHub API

↓

Repository List
```

Guide:
install nodejs nodejs.org/en/download

mcp server github.com/microsoft/playwright-mcp

Agenda

What is AI Agent?

What is the MCP Server and How this MCP help an LLM to be superman.

AI Agent that perform Web browser Testing using Selenium, Playwright.

Task 1 - Basic Task

Task 2 - Medium Task

Task 3 - Advance Stuff

Github MCP Server – Push code via Prompts (like 5th grade)

<img width="1398" height="865" alt="image" src="https://github.com/user-attachments/assets/3eb2d6e9-afce-4bb0-b2e1-01117c85d897" />

<img width="965" height="539" alt="image" src="https://github.com/user-attachments/assets/07a12946-8060-488d-97e1-f4782d322db4" />

