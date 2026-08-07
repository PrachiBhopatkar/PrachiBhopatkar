<h1>Hi, I'm Prachi 👋</h1>

**Engineer turned product leader.** 12+ years across engineering and product management, currently leading agentic products at AWS.

I use the latest technology to solve real customer problems. As a product manager, I put myself in the user's shoes to understand their workflows and identify the real problem, then build products that solve it at scale.

---

## What interests me

**Using generative AI and agents to rethink workflows rather than merely automating existing manual steps.** Applied well, agents accelerate throughput and eliminate work humans shouldn't be doing at all — releasing that bandwidth for the decisions where human judgment and strategic thinking are what actually matter.

My experience lies in:

- **Data products at scale** — building applications that process trillions of line items into actionable insight.
- **Platform and API products** — foundational services and APIs that other teams and partners build on, designed for permissions, governance, and scale from the start.
- **Zero-to-one product development** — taking products from first customer conversation to launch, then scaling them across an enterprise customer base.
- **Building applications myself** — I design, build, and ship complete applications outside of work: native macOS apps, RAG systems, mobile-first web apps. Rapid prototyping with coding agents keeps discovery fast and puts working software in front of customers early.

---

## 🤖 Working with AI agents

- **Goal-oriented agent orchestration** — specialized agents working together toward a business outcome, with task decomposition and clean context handoff across the chain rather than isolated single-task execution.
- **Agent observability** — action logging, tracing, and operational controls: what the agent did, under whose authority, and where it diverged from the expected path.
- **Evaluation and guardrails** — evaluation sets that measure agent quality against ground truth, plus permission scoping, access boundaries, and action-level controls before agents touch production systems.
- **Chat-based and autonomous agents** — human-in-the-loop conversational interfaces and goal-driven autonomous execution. Which one a workflow calls for is a design decision, not a default.
- **Agent platform foundations** — throughput and scale, access permissions, governance, and the operational controls that determine whether an agent portfolio survives production.

---

## 💼 Experience

**AWS** · Feb 2020 – Present
- **Product Lead** · Aug 2024 – Present — AWS Partner Central agents, AWS Partner account connections, partner onboarding and journey.
- **Product Lead** · Feb 2020 – Aug 2024 — AWS Cost Explorer, and access controls for Billing and Cost Management products.

**ADP (Lifion by ADP)** · Jul 2016 – Feb 2020
- **Lead Engineer and Product Manager** — ADP integrations and next-generation compliance products.

**Deloitte Consulting** · Jun 2011 – Oct 2013
- **Technology Consultant** — enterprise SAP transformations.

---

## 🚀 Applications I've Built

### 🎙️ [CrispVoice](https://github.com/PrachiBhopatkar/CrispVoice)
**Read it there. Say your response. Send it there.**

A native macOS app that brings AI-assisted message formatting into whatever application you're already in. Read a message in Slack, Outlook, Mail, or Teams, press a global hotkey, speak your response naturally, and pick a polished version — CrispVoice inserts it back into the same app. No separate drafting window, no per-platform integration, no switching away from the conversation.

The native app already holds the best context — attachments, formatting, earlier messages, reactions. Pulling a conversation into a separate AI tool to draft a reply throws that context away and adds friction, and plain dictation doesn't solve it either, since raw speech arrives full of filler and false starts.

**Install it from Terminal:**

```bash
curl -fsSL https://raw.githubusercontent.com/PrachiBhopatkar/CrispVoice/main/scripts/install.sh | /bin/bash
```

Downloads the latest GitHub Release, verifies its checksum, universal architecture, bundle identity, and pinned self-signed certificate, then installs to `~/Applications/CrispVoice.app` — no `sudo`. Afterwards, grant Microphone, Speech Recognition, and Accessibility permissions, add your Anthropic API key in Settings, and press `Control + Option + C` to dictate.

`Swift` `SwiftUI` `macOS` `Claude API` `Speech-to-text`

### 🛋️ [Airport Lounge RAG Assistant](https://github.com/PrachiBhopatkar/rag-knowledge-assistant)
**Which lounges can I actually get into, right now, with this card?**

**▶️ Use the application here: [rag-knowledge-assistant-lake.vercel.app](https://rag-knowledge-assistant-lake.vercel.app/)**

A production RAG application that answers natural-language questions about airport lounge access for the top US travel credit cards, including real-time filtering for lounges that are currently open. Combines live-scraped Priority Pass data, static card policy rules, and LLM reasoning to return specific answers instead of generic ones.

The information travelers need is scattered across issuer sites, the Priority Pass app, and airport-specific pages — and none of it tells you what's open right now at your gate. Getting to a correct answer meant solving the production RAG problems: two-stage retrieval (ChromaDB vector search over the top 20 candidates, then Cohere reranking down to 8), and metadata filtering on `airport_code` to stop chunks from one airport contaminating a query about another.

**Evaluation is the part that made it trustworthy.** A hand-curated gold dataset scores every answer across four dimensions: were the correct airport documents retrieved, are the required facts present, is the expected table format used, and does the answer correctly say "no access" when the card doesn't grant any. Cases deliberately cover the failure-prone ones — no-access cards, open-now queries, multi-airport questions.

The lesson that generalizes: **RAG evals expose retrieval failures that output quality masks.** An LLM will produce a fluent, confident answer from entirely the wrong chunks, and no amount of reading the response reveals it. Only scoring retrieved documents against the ones the question actually required catches it.

`Python` `RAG` `ChromaDB` `Cohere rerank` `Evals` `Next.js` `Vercel`

### 💸 TogetherTab
**Split bills with friends — no awkward IOUs.**

A mobile-first expense splitting app for tracking shared costs with friends, whether it's a trip, a dinner, or any group expense. Runs in any browser but is designed to feel like a native iOS app.

Group expenses into **Activities** (trips, events, dinners) and see total spend at a glance. Split any expense equally across any combination of participants — pulled from your friends list or added by phone number, with real-time lookup that detects whether someone's already on the app. If they aren't, TogetherTab generates an invite link automatically and links their share to their account the moment they join. A dashboard shows your net balance, what you're owed, and what you owe; a notifications inbox collects connection requests and outstanding balances with a **Remind** button to nudge friends. When the payer marks an expense received it settles instantly, and once every expense in an Activity is settled the whole Activity archives itself.

`React 19` `TypeScript` `Tailwind` `Framer Motion` `Firebase Auth` `Supabase` `Capacitor` `iOS`

> 📸 Screenshots coming soon.

---

## 🎓 Education

**New York University** — *M.S. Computer Science*, May 2016
GPA 3.9/4.0 · NYU merit-based scholarship

**Pune University**, India — *B.E. Computer Science*, Jun 2011 · Distinction

---

## 🧰 Toolkit

**Product:** Product strategy & roadmap · Customer research · Zero-to-one development · Cross-functional execution · Rapid prototyping

**AI & Agents:** Agent orchestration · MCP servers · Agent observability & evals · RAG · Prompt and context engineering · Coding agents (Claude Code, Kiro, Codex)

**Technical:** API product development · Data modeling · SQL · Python · TypeScript / React · Swift · Next.js · Supabase · Vercel

---

## 🤝 Let's connect

I'd love to talk about AI agents, product, or anything you're building.

<p align="left">
  <a href="https://www.linkedin.com/in/prachibhopatkar"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
</p>
