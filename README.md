# Financial Advisory Multi-Agent System — n8n

Automated customer service system with 4 AI agents for financial advisory offices.

## How it works

The client sends a text or audio message via Telegram.
The main flow detects the input type and routes it to the correct agent.

Audio messages are automatically transcribed and structured by Gemini before routing.

## Agents

- **Sofia (Orchestrator):** reads the client's intent and triggers the right specialist
- **Leo (Support):** answers technical questions — Selic, FII, CDB, Treasury bonds
- **Bia (Financial):** queries the database, checks pending payments, sends invoice copies
- **Arthur (CS):** qualifies the client, understands their goal, and schedules a meeting on Google Calendar

The client never notices the handoff. The experience feels like a single, fluid interaction.

## Stack

- n8n
- Google Gemini
- Telegram
- Google Calendar
- Google Sheets

## How to use

1. Export the workflow JSON from your n8n instance
2. Import `workflow.json` into your n8n
3. Configure your credentials (Gemini, Telegram, Google Calendar, Google Sheets)
4. Activate the workflow

## Project context

Built as part of an n8n automation course by Hashtag Treinamentos.
