# My n8n AI Automation Workflows

A collection of 19 production-grade AI automation workflows built with **n8n**, integrating **GPT-4o/mini**, **Pinecone**, **LangChain**, and various APIs.

---

## Workflow List

| # | File | Description |
|---|------|-------------|
| 1 | `Airtable_to_mail.json` | Polls Airtable for new orders → GPT-4o generates email summary → sends via Gmail |
| 2 | `Sentiment_Analyse.json` | Form submission → GPT-4o-mini sentiment classification → logs to Google Sheets |
| 3 | `Rag_Bot.json` | RAG chatbot for Tesla Q3/Q4 financial reports using Pinecone + GPT-4o |
| 4 | `Sponsor_reply.json` | Auto-reply agent for sponsor inquiries |
| 5 | `Whatsapp_Test_Agent.json` | WhatsApp AI agent with Wikipedia, Gmail tools & per-user memory |
| 6 | `Telegram1.json` | Telegram AI agent with web search sub-workflow & calculator |
| 7 | `Telgram1_Sub_Workflow_Search.json` | Sub-workflow: searches Wikipedia, HackerNews & SerpAPI |
| 8 | `telegram2.json` | Advanced Telegram bot with voice transcription (Whisper), Gmail & Google Calendar tools |
| 9 | `Sub_Workflow_X_Posts__Twitter_.json` | AI agent that generates X/Twitter posts and saves to Google Sheets |
| 10 | `Sub_Calender_Agent.json` | Calendar agent: create, read, update, delete Google Calendar events via natural language |
| 11 | `Subworkflow_Contact_Agent.json` | Contact management agent — reads/adds contacts from Google Sheets |
| 12 | `Sub_Workflow_Mails.json` | Full email management agent: read, send, reply, draft, label, mark read/unread |
| 13 | `Error_Workflow_Trigger.json` | Global error handler — sends failure alerts via Gmail for any broken workflow |
| 14 | `Webhook_Flowise_Stock_Data_to_Sheets.json` | Receives stock data via webhook (Flowise) and appends to Google Sheets |
| 15 | `Telegram_Webhook.json` | Advanced Telegram webhook integration with multiple tools |
| 16 | `Goldsmith_to_Pinecone.json` | Watches Google Drive folder → chunks & embeds new docs into Pinecone vector store |
| 17 | `goldsmith_rag_app.json` | RAG chatbot for goldsmith business with lead capture to Google Sheets |
| 18 | `Scrape_HTML_to_Markdown.json` | Scrapes a webpage via HTTP request and converts HTML to Markdown |
| 19 | `Airtable.json` | Form submission → creates a record in Airtable (room booking) |

---

## Tech Stack

- **Automation:** n8n
- **LLMs:** OpenAI GPT-4o, GPT-4o-mini, Whisper (voice transcription)
- **Vector DB:** Pinecone
- **AI Framework:** LangChain (via n8n LangChain nodes)
- **Integrations:** Gmail · Google Sheets · Google Calendar · Google Drive · WhatsApp Business API · Telegram Bot API · Airtable · SerpAPI · HackerNews · Wikipedia

---

## How to Import

1. Open your n8n instance
2. Go to **Workflows → Import from File**
3. Select any `.json` file from this repo
4. Reconnect your own credentials (API keys, OAuth accounts)
5. Activate the workflow

---

*Built by [Aarya Vaidya](https://github.com/rajaaryan779) as part of AI/ML portfolio.*
