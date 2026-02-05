# AI Agent SDR

> **Status:** MVP / Work in progress  
> AI-powered SDR agent designed to autonomously qualify leads and route them to sales teams.

## 📌 Problem
Sales teams often waste time handling unqualified leads.
Manual lead qualification is slow, inconsistent and does not scale across messaging channels.

## 💡 Solution
This project implements an AI-driven SDR agent that interacts with leads,
collects key qualification information and classifies leads based on business rules.
Qualified leads are automatically routed to a human sales closer.

## ⚙️ How it works (high-level)
1. A lead sends a message through a messaging platform
2. The system normalizes the message (text or audio transcription)
3. The AI agent conducts the conversation following strict business rules
4. Lead identity, context and conversation state are stored
5. The agent qualifies or disqualifies the lead
6. Qualified leads are routed to a sales flow automatically

## 🧠 Core Features
- AI-powered conversational SDR agent
- Strict identity and qualification flow
- Stateful conversation memory
- Business rule-based lead classification
- Automated routing of qualified leads
- Error handling and fallback logic
- Message formatting and delivery control

## 🛠 Technologies & Tools
- n8n (workflow orchestration)
- OpenAI (LLM and audio transcription)
- Supabase (database and vector storage)
- WhatsApp API (Z-API)
- Webhooks and REST APIs
- VPS-based deployment

## 📷 Workflow & Architecture
Workflow diagrams and screenshots see available in the `/docs` folder.

## 🎯 Real-world Usage
This system was designed and deployed for a real business environment,
handling real leads and optimizing the sales qualification process.

## ⚠️ Known Limitations
- Qualification logic still requires tuning for different lead profiles
- Some edge cases may cause misclassification
- Observability and analytics can be improved
- Prompt and logic optimization is ongoing

## 🗺 Roadmap
- [ ] Improve lead qualification scoring
- [ ] Add better confidence handling for AI decisions
- [ ] Improve monitoring and logging
- [ ] Refine conversation flows based on real usage data
- [ ] Add admin-level insights or dashboard

## 🔒 Security & Privacy
Sensitive credentials, prompts and internal business logic are not included in this repository.
This is a sanitized version focused on architecture and system design.

## 🧠 What I learned
- Designing AI agents with strict business constraints
- Managing stateful conversations at scale
- Integrating AI with real-world business systems
- Thinking about automation reliability and failure modes
