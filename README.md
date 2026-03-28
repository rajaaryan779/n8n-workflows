# ⚡ FlowMind — n8n AI Automation Workflow Suite

> 19 production-grade AI automation workflows built with **n8n**, integrating **GPT-4o/mini**, **Pinecone**, **LangChain**, and 10+ external APIs.

![n8n](https://img.shields.io/badge/n8n-Automation-orange?logo=n8n&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-412991?logo=openai&logoColor=white)
![Pinecone](https://img.shields.io/badge/Pinecone-Vector%20DB-green)
![LangChain](https://img.shields.io/badge/LangChain-AI%20Framework-blue)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## ✨ Highlights

- 🤖 **Multi-agent bots** for Telegram & WhatsApp with memory and tool use
- 🧠 **RAG pipelines** powered by Pinecone + OpenAI Embeddings
- 📧 **Full email management** via Gmail API (read, send, reply, draft, label)
- 📅 **Calendar agent** with full CRUD via natural language
- 🔊 **Voice transcription** using OpenAI Whisper
- 🛡️ **Error monitoring** with auto email alerts on workflow failure
- 📊 **Sentiment analysis** pipeline with Google Sheets logging

---

## 📁 Workflow List

### 🤖 AI Agents & Bots

| # | File | Description |
|---|------|-------------|
| 5 | `Whatsapp_Test_Agent.json` | WhatsApp AI agent with Wikipedia, Gmail tools & per-user memory |
| 6 | `Telegram1.json` | Telegram AI agent with web search sub-workflow & calculator |
| 7 | `Telgram1_Sub_Workflow_Search.json` | Sub-workflow: searches Wikipedia, HackerNews & SerpAPI |
| 8 | `telegram2.json` | Advanced Telegram bot with voice transcription (Whisper), Gmail & Google Calendar |
| 15 | `Telegram_Webhook.json` | Advanced Telegram webhook integration with multiple tools |
| 4 | `Sponsor_reply.json` | Auto-reply agent for sponsor inquiries |

### 🧠 RAG & Vector Pipelines

| # | File | Description |
|---|------|-------------|
| 3 | `Rag_Bot.json` | RAG chatbot for Tesla Q3/Q4 financial reports using Pinecone + GPT-4o |
| 16 | `Goldsmith_to_Pinecone.json` | Watches Google Drive → chunks & embeds docs into Pinecone vector store |
| 17 | `goldsmith_rag_app.json` | RAG chatbot for goldsmith business with live lead capture to Google Sheets |

### 📧 Email & Calendar Automation

| # | File | Description |
|---|------|-------------|
| 12 | `Sub_Workflow_Mails.json` | Full email agent: read, send, reply, draft, label, mark read/unread |
| 10 | `Sub_Calender_Agent.json` | Calendar agent: create, read, update, delete events via natural language |
| 11 | `Subworkflow_Contact_Agent.json` | Contact management — reads/adds contacts from Google Sheets |
| 1 | `Airtable_to_mail.json` | Polls Airtable for new orders → GPT-4o email summary → Gmail |

### 📊 Data & Analytics

| # | File | Description |
|---|------|-------------|
| 2 | `Sentiment_Analyse.json` | Form submission → GPT-4o-mini sentiment classification → Google Sheets |
| 9 | `Sub_Workflow_X_Posts__Twitter_.json` | Generates X/Twitter posts via AI and saves them to Google Sheets |
| 14 | `Webhook_Flowise_Stock_Data_to_Sheets.json` | Receives stock data via webhook and appends to Google Sheets |
| 18 | `Scrape_HTML_to_Markdown.json` | Scrapes a webpage via HTTP request and converts HTML to Markdown |

### 🛠 Utilities

| # | File | Description |
|---|------|-------------|
| 13 | `Error_Workflow_Trigger.json` | Global error handler — sends Gmail alerts on any workflow failure |
| 19 | `Airtable.json` | Form submission → creates a record in Airtable (room booking) |

---

## 🧰 Tech Stack

| Layer | Tools |
|-------|-------|
| **Automation** | n8n |
| **LLMs** | OpenAI GPT-4o, GPT-4o-mini, Whisper |
| **Vector DB** | Pinecone |
| **AI Framework** | LangChain (via n8n nodes) |
| **Messaging** | WhatsApp Business API, Telegram Bot API |
| **Google Suite** | Gmail, Google Sheets, Google Calendar, Google Drive |
| **Search** | SerpAPI, HackerNews, Wikipedia |
| **Databases** | Airtable |

---

## 🚀 How to Import

1. Open your n8n instance
2. Go to **Workflows → Import from File**
3. Select any `.json` file from this repo
4. Reconnect your own credentials (API keys, OAuth accounts)
5. Activate the workflow

> **Note:** All credential IDs have been removed. Set up your own connections after importing.

---

## 👤 Author

**Aarya Vaidya**
- GitHub: [@rajaaryan779](https://github.com/rajaaryan779)
- LinkedIn: [aarya-vaidya](https://www.linkedin.com/in/aarya-vaidya-013227211/)
