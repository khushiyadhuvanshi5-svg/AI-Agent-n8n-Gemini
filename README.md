# 🤖 AI Agent Automation using n8n & Google Gemini

## 📌 Project Overview

This project demonstrates the development of an **AI-powered conversational agent using n8n and Google Gemini**. The workflow receives user messages through a chat interface, processes them using an AI Agent, and generates relevant responses using the Google Gemini Chat Model.

The AI Agent is enhanced with **Simple Memory, SerpAPI, and Calculator** tools, allowing it to maintain conversation context, perform web searches, and handle mathematical calculations when required.

This project was developed as a practical implementation of **AI Agents, workflow automation, API integration, and tool-based AI systems**.

---

## 🎯 Project Objectives

The main objectives of this project are:

* Build an AI-powered conversational agent using n8n.
* Integrate Google Gemini as the primary AI Chat Model.
* Implement conversational memory using Simple Memory.
* Enable web-search capabilities using SerpAPI.
* Perform mathematical calculations using the Calculator tool.
* Understand how AI Agents interact with external tools.
* Gain practical experience with workflow automation and API integration.

---

## 🛠️ Technologies & Tools Used

| Technology / Tool | Purpose                                                          |
| ----------------- | ---------------------------------------------------------------- |
| **n8n**           | Workflow automation and AI Agent orchestration                   |
| **Google Gemini** | AI language model for processing and generating responses        |
| **Simple Memory** | Maintains conversation context                                   |
| **SerpAPI**       | Provides web-search functionality                                |
| **Calculator**    | Performs mathematical calculations                               |
| **APIs**          | Enables communication between the workflow and external services |

---

## 🔄 Workflow Architecture

The workflow follows this general architecture:

```text
User Message
     │
     ▼
When Chat Message Received
     │
     ▼
   AI Agent
     │
     ├──────────────► Google Gemini Chat Model
     │
     ├──────────────► Simple Memory
     │
     ├──────────────► SerpAPI
     │
     └──────────────► Calculator
     │
     ▼
Final Response
```

The **AI Agent** acts as the central component of the workflow. It receives the user's message, uses Google Gemini to understand the request, accesses conversation memory, and selects the appropriate tool when necessary.

---

## 🧩 Workflow Components

### 1. When Chat Message Received

This node acts as the trigger for the workflow. It starts the workflow whenever a user sends a new message through the chat interface.

The received message is passed to the AI Agent for further processing.

### 2. AI Agent

The AI Agent is the central component responsible for processing user queries and generating appropriate responses.

It uses Google Gemini as the language model and can access connected tools such as Simple Memory, SerpAPI, and Calculator depending on the user's request.

### 3. Google Gemini Chat Model

Google Gemini is used as the primary language model for the AI Agent.

It understands user queries, processes the provided context, and generates natural-language responses.

### 4. Simple Memory

Simple Memory helps the AI Agent maintain conversation context during a chat session.

It allows the agent to consider previous messages when responding to follow-up questions, creating a more continuous conversational experience.

### 5. SerpAPI

SerpAPI is integrated as a tool to provide web-search functionality.

When a query requires external or online information, the AI Agent can use SerpAPI to retrieve relevant search results and use that information while generating the response.

### 6. Calculator

The Calculator tool allows the AI Agent to perform mathematical operations accurately.

It can be used whenever the user's request requires calculations or numerical processing.

---

## ⚙️ How the Workflow Works

1. A user sends a message through the n8n chat interface.
2. The **When Chat Message Received** node triggers the workflow.
3. The user's message is passed to the **AI Agent**.
4. The AI Agent uses **Google Gemini** to understand and process the request.
5. **Simple Memory** provides relevant conversation context.
6. If required, the AI Agent uses **SerpAPI** for web searches.
7. If a mathematical operation is required, the AI Agent uses the **Calculator** tool.
8. The AI Agent processes the information and generates the final response.
9. The response is returned to the user through the chat interface.

---

## 🔐 API & Credential Security

API credentials are configured securely through the n8n credential system.

**No API keys, passwords, tokens, or other sensitive credentials are included in this repository.**

> ⚠️ Never upload real API keys or secret credentials to GitHub.

If credentials are accidentally exposed, they should be revoked immediately and replaced with new credentials.

---

## 🚧 Challenge Faced During Development

During the initial development, the workflow used the **OpenAI Chat Model**. However, the OpenAI API account reached its available API credit limit, which prevented further API requests from being processed.

To resolve this issue without changing the overall workflow architecture, the OpenAI Chat Model was replaced with the **Google Gemini Chat Model**.

The AI Agent, memory, and connected tools were retained while the chat model was changed to Gemini.

---

## 📚 Key Learning Outcomes

Through this project, I gained practical experience in:

* Building AI Agent workflows using n8n.
* Integrating and configuring Google Gemini.
* Working with API-based services.
* Connecting AI Agents with external tools.
* Implementing conversational memory.
* Using web-search APIs with AI workflows.
* Understanding tool-based AI Agent architecture.
* Testing and troubleshooting AI workflows.
* Managing API credentials securely.

---

## 🚀 Future Scope

The project can be further enhanced by:

1. Integrating a database for persistent conversation history.
2. Adding long-term memory capabilities.
3. Integrating additional APIs and external tools.
4. Adding authentication and user access control.
5. Implementing advanced monitoring and logging.
6. Automating tasks such as email sending and report generation.
7. Integrating document processing and knowledge bases.
8. Deploying the AI Agent as a production-ready application.

---

## 📂 Repository Structure

```text
AI-Agent-n8n-Gemini/
│
├── README.md
│
├── workflow/
│   └── ai-agent-gemini.json
│
├── screenshots/
│   ├── 01-workflow.png
│   ├── 02-ai-agent.png
│   ├── 03-gemini.png
│   ├── 04-memory.png
│   ├── 05-serpapi.png
│   ├── 06-calculator.png
│   └── 07-successful-execution.png
│
└── documentation/
    └── AI_Agent_Project_Report.pdf
```

---

## 👩‍💻 Author

 KHUSHI YADAV

BCA | Cybersecurity Enthusiast | AI & Automation Learner

This project was developed as part of my hands-on learning and practical exploration of **AI Agents, workflow automation, API integration, and cybersecurity-related technologies**.

---

## ⭐ Acknowledgements

I would like to acknowledge the documentation, learning resources, and community tutorials that helped me understand AI Agent workflows and n8n during the development of this project.

---

## 📄 License

This project is created for **educational and learning purposes**.

