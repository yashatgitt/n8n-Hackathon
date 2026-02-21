# 🤖 AI-Powered Telegram Assistant  
### Autonomous Multi-Tool Workflow Automation using n8n Cloud + Gemini

An intelligent Telegram-based assistant that converts natural language messages into real-world actions such as sending emails, scheduling calendar events, creating documents, and setting reminders.

This is not just a chatbot.  
It is an AI-driven execution agent built using workflow orchestration.

---

## 🚀 Overview

This project integrates:

- **Telegram Bot** (User Interface)
- **Gemini AI Model** (Intent Detection & Reasoning)
- **n8n Cloud** (Workflow Orchestration)
- **Gmail API** (Email Automation)
- **Google Calendar API** (Event Scheduling)
- **Google Docs / Sheets** (Notes & Logging)

Users simply send a message in Telegram, and the assistant interprets the intent, selects the correct tools, executes the task, and confirms the result.

---

## 🧠 How It Works

1. User sends a message on Telegram  
2. Telegram Trigger activates workflow  
3. Gemini analyzes message and returns structured JSON  
4. Switch node routes to the correct action  
5. Action node executes (Email / Calendar / Docs / Reminder)  
6. Confirmation is sent back to Telegram  

Architecture Flow:

```
Telegram → Gemini AI → Switch Router → Tool Execution → Telegram Response
```

---

## ✨ Core Features

### 📧 Email Automation
- Send emails via Gmail
- Extract recipient, subject, and body
- Confirmation before sending
- Notify user after success

### 📅 Calendar Management
- Create events using natural language
- Normalize date and time automatically
- Prevent incomplete scheduling

### 📝 Notes & Documents
- Create structured documents
- Save notes dynamically
- Maintain organized records

### ⏰ Reminders
- Parse future time (e.g., "tomorrow 6pm")
- Use delayed execution
- Send reminders back on Telegram

### 🧠 Conversation Memory
- Maintains context across interactions
- Supports follow-up commands

---

## 🔄 Autonomous Multi-Step Execution

The assistant can break complex goals into sequential steps.

Example:

> "Prepare meeting package for tomorrow"

Execution Plan:
- Fetch meeting details from Calendar
- Search Gmail history
- Summarize previous discussions
- Create meeting agenda document
- Draft follow-up email
- Notify user

This demonstrates:
- Planning
- Tool selection
- Sequential execution
- Final deliverable generation

---

## 🛡 Reliability & Error Handling

To prevent workflow failures:

- Strict JSON schema enforcement
- Confirmation before critical actions
- Validation of required parameters
- Logging of executions
- Clear failure notifications
- No guessing of missing data

---

## 🏗 Tech Stack

- **n8n Cloud** – Workflow orchestration
- **Google Gemini API** – AI reasoning & structured output
- **Telegram Bot API** – User interaction
- **Gmail API** – Email services
- **Google Calendar API** – Scheduling
- **Google Docs / Sheets API** – Documentation & logging

---

## 📸 Screenshots

### 1️⃣ Telegram Interaction
![Workflow demo](img2)
![Telegram Demo](img1)

### 2️⃣ Workflow Architecture in n8n
![Telegram Demo](flow)
---

## 🎯 Real World Impact

- Reduces app switching
- Centralizes productivity tools
- Saves time through automation
- Demonstrates AI-powered workflow orchestration
- Scalable for teams, students, and businesses

---

## 🔮 Future Improvements

- Advanced multi-action planning schema
- Priority-based task optimization
- Smart scheduling suggestions
- Analytics dashboard
- Tool auto-discovery system

---

## 📌 Conclusion

This project demonstrates how AI can move beyond conversation and become a real execution engine.  
By combining reasoning, automation, and API integrations, Telegram becomes a powerful productivity command center.

---

## 🛠 Setup (High Level)

1. Deploy n8n Cloud instance  
2. Create Telegram Bot and connect credentials  
3. Configure Gemini API key  
4. Set up Gmail & Google Calendar credentials  
5. Import workflow  
6. Activate and test  

---

## 📄 License

MIT License
