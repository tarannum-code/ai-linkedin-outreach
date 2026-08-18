# 🤖 AI-Powered LinkedIn Outreach & Lead Intelligence

An AI-assisted lead generation and LinkedIn outreach system that identifies ICP-aligned prospects, researches and qualifies leads, stores structured lead intelligence in Airtable, generates personalized outreach messages, and supports automated LinkedIn connection workflows.

The project combines **Claude/Cowork-based AI research**, **Tavily for web research**, **Airtable for lead management**, and a **Node.js + Playwright outreach automation layer**.

---

## 🎥 Demo

📺 **Watch the full demo video**

https://drive.google.com/file/d/1ii-t7Uo9ThuTFXniSSrRNUKSFxsofA-I/view?usp=drive_link

The demo shows the lead research process, Airtable lead creation, and the LinkedIn outreach workflow.

---

## 🖼️ Project Screenshots

### AI Agent Instructions

![AI Agent Instructions](screenshots/ai-agent-instructions.png)

The AI agent is configured to discover, verify, qualify, score, and save relevant prospects into Airtable.

### AI Lead Research

![Lead Research](screenshots/lead-research.png)

The research workflow uses Tavily to investigate relevant prospects and their companies before adding qualified leads to Airtable.

### Airtable Lead Record

![Airtable Lead Record](screenshots/airtable-lead-record.png)

Qualified lead information is stored in Airtable, including professional details, company information, LinkedIn profile, lead score, qualification reason, and personalized outreach message.

### Lead Fields

![Lead Fields](screenshots/lead-fields.png)

Structured fields organize the lead intelligence collected by the research workflow.

### LinkedIn Outreach Automation

![Outreach Automation](screenshots/outreach-automation.png)

The outreach layer reads eligible leads from Airtable, analyzes the LinkedIn profile, finds the connection workflow, sends the prepared personalized message, and updates the lead status.

---

## ⚙️ How It Works

The project consists of two connected automation layers.

### 1. AI Lead Research & Qualification

```text
Services / ICP
      ↓
AI Lead Research
      ↓
Tavily Web Research
      ↓
Profile & Company Analysis
      ↓
Lead Qualification
      ↓
Personalized Message
      ↓
Airtable

The research agent identifies relevant prospects based on the target ICP, researches available information, evaluates the prospect and company context, and stores qualified leads in Airtable.

2. LinkedIn Outreach
Airtable
      ↓
Eligible Lead
      ↓
LinkedIn Profile Analysis
      ↓
Find Connection Option
      ↓
Personalized Connection Request
      ↓
Airtable Status Update

The Node.js outreach system retrieves eligible leads from Airtable and uses Playwright for browser-based LinkedIn interaction.

🧠 AI Lead Intelligence

The research layer turns an ICP into structured, actionable lead information.

For qualified prospects, the system can store information such as:

Name
Position
Company
Website
LinkedIn profile
Industry
Relevant use case
Intent signals
Lead score
Qualification reason
Personalized outreach message
Outreach status

The overall flow is:

Prospect Discovery → Research → Qualification → Personalization → Outreach Preparation

🔄 End-to-End Architecture
             ICP / Service Requirements
                       ↓
                 Claude / AI Agent
                       ↓
                  Tavily Research
                       ↓
               Prospect Qualification
                       ↓
                Personalized Message
                       ↓
                    Airtable
                       ↓
               Node.js Outreach Agent
                       ↓
                    Playwright
                       ↓
              LinkedIn Profile Review
                       ↓
           Personalized Connection Request
                       ↓
                 Airtable Update

Airtable acts as the shared lead-management layer between the research and outreach workflows.

🛠️ Tech Stack
Layer	Technology
AI / Agent	Claude / Claude Code / Cowork
Research	Tavily
Lead Management	Airtable
Backend / Automation	Node.js
Browser Automation	Playwright
Language	JavaScript
Configuration	dotenv
✨ Key Features
ICP-based prospect discovery
AI-assisted lead research
Tavily-powered web research
Prospect and company analysis
Lead qualification and scoring
Structured Airtable lead management
Personalized outreach message generation
LinkedIn profile analysis
Browser-based outreach workflow
Airtable status synchronization
Modular automation architecture
📁 Project Structure
ai-linkedin-outreach/
│
├── architecture/
│   └── workflow-overview.png.png
│
├── demo/
│   └── demo_linkedin-outreach.mp4
│
├── screenshots/
│   ├── ai-agent-instructions.png
│   ├── airtable-lead-record.png
│   ├── lead-fields.png
│   ├── lead-research.png
│   └── outreach-automation.png
│
└── README.md
🔐 Security & Privacy

Sensitive information should remain outside the public repository.

Do not commit:

API keys
Airtable tokens
LinkedIn credentials
Browser session data
Private cookies
Private company credentials
Unnecessary personal lead information

Use environment variables and local configuration for secrets.

Screenshots included in the public repository should be sanitized to avoid exposing private prospect information.

🎯 What This Project Demonstrates

AI Agents · LLM Workflows · Web Research · ICP Qualification · Lead Intelligence · Airtable Automation · Node.js · Playwright · Browser Automation · API Integration · Workflow Design

💡 Project Value

The system connects two normally separate tasks:

Finding the right prospects and preparing personalized outreach.

The research layer reduces manual prospect research and qualification, while the outreach layer connects qualified Airtable leads with a personalized LinkedIn outreach workflow.

This creates a complete pipeline:

Research → Qualify → Store → Personalize → Outreach → Update CRM

👤 Author

Tarannum Khan

AI Automation Engineer
