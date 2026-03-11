# AI Learning Path Generator (n8n AI Agent)

An AI-powered automation workflow that generates personalized learning paths, creates structured Google Docs, and schedules study sessions in Google Calendar.

This project uses **n8n AI Agents** with **Mistral AI** and external tools to automate the creation of learning plans.

---

## Features

- Generates day-wise learning paths
- Automatically searches learning resources
- Creates a Google Docs learning plan
- Schedules Google Calendar study sessions
- Fully automated AI agent workflow
- Uses external tools through MCP integrations

---

## Example Input

2 day Java learning path

---

## Example Output

Learning Path Complete!

Document: https://docs.google.com/...

Calendar: 2 events scheduled starting from 2026-03-12 at 11:00 AM.

Your 2-day Java learning journey is ready!

---

## Workflow Architecture

User Input  
↓  
AI Agent (Mistral AI)  
↓  
Web Search Tool (SerpAPI)  
↓  
Google Docs Tool  
↓  
Google Calendar Tool  
↓  
Final Learning Plan Output  

---

## Tech Stack

- n8n
- Mistral AI
- SerpAPI
- Google Docs API
- Google Calendar API
- Composio MCP

---

## How It Works

1. User provides a learning goal such as "2 day Python learning path".
2. The AI agent generates a day-wise curriculum.
3. The agent searches for useful learning resources.
4. A Google document is created with the learning plan.
5. Calendar events are scheduled for each study day.
6. The workflow returns the final learning path summary.

---

## Setup Instructions

### 1. Install n8n

Install n8n globally:

npm install -g n8n

Run n8n:

n8n

---

### 2. Import the Workflow

Open n8n in your browser and import the workflow file:

workflow/learning-path-agent.json

---

### 3. Configure Credentials

Add the following API credentials inside n8n:

- Mistral AI API Key
- SerpAPI Key
- Google Docs API
- Google Calendar API
- Composio MCP API Key

---

### 4. Run the Workflow

Trigger the chat workflow and enter a request such as:

3 day Python learning path

The AI agent will generate a complete learning plan.

---

## Screenshots

Workflow Canvas

<img width="1319" height="580" alt="Screenshot 2026-03-11 162654" src="https://github.com/user-attachments/assets/5e07cf9e-2a58-41bf-a91b-e16c05793a2e" />
<img width="1310" height="574" alt="Screenshot 2026-03-11 162802" src="https://github.com/user-attachments/assets/af10535c-3aeb-4387-9598-b8cbb6ca9b3e" />


Chatbot Demo


<img width="1310" height="578" alt="Screenshot 2026-03-11 162839" src="https://github.com/user-attachments/assets/f82b0ca3-3cf4-464a-97de-c4260c279572" />

---

## Project Structure

ai-learning-path-agent  
│  
├── workflow  
│   └── learning-path-agent.json  
│  
├── screenshots  
│   ├── workflow.png  
│   └── chat-demo.png  
│  
├── README.md  
│  
└── .gitignore  

---

## Author

Vishnu Vardhan

---

## License

MIT License
