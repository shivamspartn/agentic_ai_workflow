# Agentic AI Course Enquiry Workflow (n8n)

An automated conversational AI agent built in **n8n** using **Google Gemini**, **Simple Memory**, and **Google Sheets** tools to answer course-related questions, look up FAQs, and manage course enquiries in real time.

---

## Architecture Overview

```text
[When chat message received]
             │
             ▼
        [AI Agent]
       /     |     \
      /      |      \
     ▼       ▼       ▼
[Google   [Simple   [Google Sheets Tools]
 Gemini    Memory]   ├── courses (read: sheet)
 Chat                ├── fnq (read: sheet)
 Model]              └── courses enquiry (read: sheet)
