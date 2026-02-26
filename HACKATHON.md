# Hackathon: Build an AI Agent That Actually Helps Someone

> **DRAFT** — This document is a work in progress and may is going to before the hackathon.

## The Challenge

Build a working AI agent using the **OpenAI Agents SDK** and **AWS Bedrock** that solves a real problem for a specific user.

Your agent **must** use at least **2 of the following capabilities** you learned in class:

- **Tool calling** — custom function tools
- **RAG** — bring your own data via ChromaDB
- **Web search** — MCP / Exa
- **Guardrails** — input validation, topic enforcement
- **Memory** — multi-turn conversations
- **Multi-agent orchestration**

You may pick **any domain** — it does NOT have to be nutrition.

### Example ideas

- A travel planning agent that searches the web and remembers preferences
- A study buddy that answers questions from uploaded course notes (RAG)
- A personal finance advisor with guardrails against bad advice
- A customer support agent that routes to specialist sub-agents
- A fitness coach that looks up exercises and tracks your plan across turns

## Teams

- **5 teams of 4**
- Self-selected, but the instructor may rebalance

## Schedule (200 minutes total)

| Block               | Duration | What happens |
|----------------------|----------|--------------|
| Kickoff & teams      | 10 min   | Form teams, pick a topic, assign roles |
| Build sprint 1       | 60 min   | Get the core agent working with at least one tool |
| Check-in             | 5 min    | Quick stand-up: what works, what's blocked |
| Build sprint 2       | 55 min   | Add second capability, polish |
| Presentation prep    | 15 min   | Prepare a 5-minute live demo |
| Presentations        | 50 min   | 5 teams x 8 min (5 min demo + 3 min Q&A) |
| Wrap-up              | 5 min    | Feedback, pass criteria confirmation |

## What You Present (= Pass Criteria)

1. **Live demo** (5 min) — Show the agent running in Chainlit or a notebook. Walk us through a real conversation that demonstrates your 2+ capabilities.
2. **One slide** (optional) — What problem does it solve? Who is the user? What capabilities did you use?
3. **Q&A** (3 min) — Be ready to explain your architecture choices.

**You pass** if your agent runs, demonstrates at least 2 capabilities, and your team can explain what it does.

## Tips

- **Get something working first.** A basic agent with one tool in the first 60 minutes. Make it smarter in the second half.
- **Don't spend all your time on data.** A 50-row CSV or a short text file is plenty for RAG. See `notebooks/4_rag_setup.ipynb` for an example.
- **Start from the chatbot examples.** The `chatbot/` folder has a working agent skeleton — swap the domain and data.
- **Assign roles.** One person on agent logic, one on data/RAG, one on prompt engineering/testing, one on the presentation.
