# Innocent Mariti

**AI Automation Engineer.** Johannesburg, South Africa.

I build LLM-powered workflow systems that talk to real customers and touch real money, and I run them in production on infrastructure I administer myself.

Twelve years selling and structuring vehicle finance deals is where the problems come from. I got tired of watching good enquiries die overnight because nobody was there to answer them, so I learned to build the thing that answers.

No computer science degree. The systems are live. Here is the evidence.

---

### In production right now

| | |
|---|---|
| Active workflows | **12** live, 54 authored, 2,172 nodes |
| Executions (last 7 days) | **2,581**, one hard failure |
| Server uptime | **128 days** continuous |
| Largest single workflow | **489 nodes** |

*Verified against the production box on 2026-08-20.*

---

### What I actually do

**Conversational AI on WhatsApp and Telegram.** Multi-turn context, intent routing, human approval gates before anything reaches a customer, and delivery proven against provider message IDs instead of trusting a green tick.

**LLM integration and cost control.** Anthropic Claude, OpenAI, DeepSeek. I cut full-price input tokens per conversation turn from 12,874 to 2,801, a 78% reduction, by restructuring prompt-cache breakpoints around what was genuinely volatile per turn rather than what a code comment claimed was volatile.

**Correctness where it costs money.** I found a finance calculation quoting 30 to 33% light across 23 vehicle derivatives, fixed it, and then built a guardrail that refuses to release any figure it cannot tie to a specific model. Verified across 28 of 28 production cases and 17 of 17 adversarial cases.

**Reliability engineering.** Health checks, drift detection between duplicated logic, a dead man switch on a five-minute cron, systemd self-healing, and a snapshot plus rollback point before every production change.

**A habit I would bring to any team:** a guard you have never seen go red is not a guard. I found three of mine passing regardless of the state they claimed to check. Now every check has to fail on purpose before I trust it green.

---

### Stack

`n8n (self-hosted)` `Python` `JavaScript` `TypeScript` `SQL` `Bash`
`Anthropic Claude` `OpenAI` `DeepSeek` `prompt caching` `structured extraction` `output guardrails`
`RAG` `embeddings` `vector search` `chunking strategies` `retrieval evals`
`WhatsApp Cloud API` `Telegram Bot API` `Meta Graph` `Google Workspace OAuth2` `Twilio` `REST` `webhooks`
`Linux VPS` `Docker` `nginx` `Redis` `SQLite` `Cloudflare Tunnel & Zero Trust` `systemd` `Git`

---

### Selected work

- **[AI Sales Assistant](https://github.com/JuiceMatute356/ai-sales-assistant)** - a live WhatsApp assistant that answers vehicle enquiries, books test drives, and runs a finance application to completion. Case study, verification results, and the engineering decisions behind it.
- **[Try the assistant yourself](https://northgate-motors-sales-assistant-fbhi8i.v2.appdeploy.ai/)** - a sandboxed build against a fictional dealership. Try to talk it into quoting a price it cannot justify. It will refuse, and tell you why.
- **[grounded-rag](https://github.com/JuiceMatute356/grounded-rag)** - a retrieval system that refuses to answer what its documents do not support, with an eval harness that measures the refusal. Local embeddings, SQLite, no framework. Publishes its failures, not just its wins.
- **[CV](https://github.com/JuiceMatute356/ai-sales-assistant/blob/main/cv/Innocent_Mariti_CV_AI_Automation_Engineer.pdf)** - full detail, evidence-backed.

---

### Reach me

- **Email:** innocentmariti@gmail.com
- **LinkedIn:** [innocent-mariti](https://www.linkedin.com/in/innocent-mariti-27a4b552)
- **Site:** [maritico.co.za](https://maritico.co.za)

Open to AI automation engineering and forward-deployed / solutions engineering roles, remote or Gauteng.
