# Hi, I'm Reshma 👋

**AI/ML Engineer building production AI agents** — agentic RAG, multi-agent orchestration, and automation pipelines that ship and get used.

📍 Kochi, Kerala · 🌐 [Portfolio](https://rshmthomas-cyber.github.io/) · 💼 [LinkedIn](https://www.linkedin.com/in/reshma-thomas-nobel) · ✍️ [Medium](https://medium.com/@reshma.thomas.nobel)

---

## 🚀 What I'm building

### [Qatar Labour Law — Agentic RAG Assistant](https://hr-law-assistant.streamlit.app) · `live in production`

An agentic RAG system that answers Qatar labour law questions with the exact article cited — **live and used daily by a corporate HR team in Doha.**

The interesting part isn't the retrieval, it's that retrieval is a **tool the model chooses to use**. It searches, judges whether the results are sufficient, and re-queries for multi-step legal questions. Three purpose-built tools:

- `search_by_topic` — semantic search for open questions when you don't know the article
- `search_by_article_number` — exact lookup, because semantic search is unreliable for precise references
- `compare_articles` — pulls two articles side by side so the agent reasons *across* provisions

Every answer is grounded in retrieved source text with the article cited. In a legal context, a confident wrong answer is a liability — so the system doesn't guess.

`Claude Tool Use API` · `ChromaDB` · `PyMuPDF` · `Streamlit` · `Agentic RAG`

<!-- TODO: add repo link when public -->

---

### Saksham — Four-Agent Assistive Communication System

A multi-agent system that interprets need from live vision and speaks it in a personalized voice, built on Google's Agent Development Kit.

Four specialised agents: **perception** (OpenCV frame capture) → **need detection** (Gemini Vision) → **communication** (natural language generation) → **voice** (personalized TTS).

The architectural piece I'd point to is the **confidence gate**, which sits at detection — *before* anything gets phrased:

| Confidence | Action | Why |
|---|---|---|
| ≥ 0.70 | Proceed autonomously | Sure enough to act |
| < 0.70 | Escalate to a human | Not sure enough to speak on someone's behalf |
| < 0.50 | Loop back to **recapture** | At this point the *frame* is the problem, not the reasoning |

That last row is the design decision I'm proudest of. Re-interpreting a bad image just gives you the same bad answer — so recovery is routed to where the failure actually originates. The system is built to know when *not* to trust itself.

Validated against a 5-scenario eval suite: 100% task success at 93% average confidence. *(A smoke-test suite — expanding to adversarial and edge cases is the next step.)*

`Google ADK` · `Gemini Vision` · `MCP` · `OpenCV` · `Multi-Agent Orchestration` · `Human-in-the-Loop`

<!-- TODO: add repo link when public -->

---

## 🛠️ Tech

**Agentic AI & Automation**
`Claude Tool Use API` `Google ADK` `MCP` `Agentic RAG` `Multi-Agent Orchestration` `ChromaDB` `Vector Search` `Human-in-the-Loop Design`

**LLMs & GenAI**
`Claude API` `Gemini 1.5 Pro` `Gemini Vision` `OpenAI API` `Prompt Engineering` `RAG` `Fine-tuning` `Qwen 2.5 VLM`

**ML / CV / OCR**
`Python` `PyTorch` `TensorFlow` `Keras` `Scikit-learn` `OpenCV` `YOLO` `MobileNet` `PaddleOCR` `EasyOCR` `Roboflow`

**Backend & Deployment**
`FastAPI` `Flask` `Django` `Streamlit` `Docker` `REST APIs` `Git`

---

## 🎯 The unusual part of my background

Alongside the engineering, I've spent **8+ years as a Contributing Editor at Shalom Tidings**, coordinating 50+ contributors across 12 languages.

That's not a detour from the AI work — it's where I learned to ship on a deadline for other people, and it's where I built my first automation: content workflows processing **1,000+ documents annually across 12 languages, cutting processing time by 40%**.

🏆 Gold Award, Australian Religious Press Association (2020) · Best Magazine of the Year, Catholic Press Awards USA (2021, 2022, 2023)

---

## 💬 Currently

Building agentic systems and taking on **contract work** in GenAI, agentic AI, and workflow automation — with a particular interest in the GCC market.

Reach me on [LinkedIn](https://www.linkedin.com/in/reshma-thomas-nobel) or through my [portfolio](https://rshmthomas-cyber.github.io/).
