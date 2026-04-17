# Lab 8 — Report

## Task 1A — Bare agent

**Q: What is the agentic loop?**
```
The agentic loop is the core cycle that enables an AI agent to autonomously
achieve goals through repeated observation, decision-making, and action. Here's
a simplified breakdown:

1. Observe: Gather information (user input, environment state, tool outputs).
2. Reason: Analyze the situation and decide the best next step.
3. Act: Execute a tool call, command, or action.
4. Observe Results: Evaluate the outcome.
5. Repeat: Use new insights to refine the next step.

This loop allows me (nanobot) to handle complex tasks dynamically, adapting as
new information emerges. For example, if you ask me to "write a report," I might:
• Search the web for templates (web_search),
• Read a file for context (read_file),
• Write the report (write_file),
• And iterate based on your feedback.
```

**Q: What labs are available in our LMS?**
(Note: At this point MCP tools are not yet configured, so the agent answered from general knowledge.)
```
I don't have real-time access to your LMS system. However, based on typical
Software Engineering curriculum, common labs include:
- Lab 01: Products, Architecture & Roles
- Lab 02: Backend Service (Run, Fix, Deploy)
- Lab 03: Backend API (Explore, Debug, Implement, Deploy)
- Lab 04: Testing, Front-end, and AI Agents
- Lab 05: Data Pipeline and Analytics Dashboard
- Lab 06: Build Your Own Agent
- Lab 07: Build a Client with an AI Coding Agent
- Lab 08: Advanced Topics

Note: This is a general answer since I cannot query your live LMS backend.
```

**PASS** - Agent responds to general questions via OpenRouter free model.

---

## Task 1B — Agent with LMS tools

MCP tools registered in config:
- lms_health
- lms_labs
- lms_learners
- lms_pass_rates
- lms_timeline
- lms_groups
- lms_top_learners
- lms_completion_rate
- lms_sync_pipeline

**Q: What labs are available?**
```
Here are the available labs:

1. **Lab 01** – Products, Architecture & Roles
2. **Lab 02** — Run, Fix, and Deploy a Backend Service
3. **Lab 03** — Backend API: Explore, Debug, Implement, Deploy
4. **Lab 04** — Testing, Front-end, and AI Agents
5. **Lab 05** — Data Pipeline and Analytics Dashboard
6. **Lab 06** — Build Your Own Agent
7. **Lab 07** — Build a Client with an AI Coding Agent
8. **Lab 08** — lab-08

Let me know if you'd like details about a specific lab!
```

**Q: Is the LMS backend healthy?**
(Agent used lms_health tool to verify backend connectivity.)

**PASS** - Agent now returns real backend data via MCP tools.

---

## Task 1C — Skill prompt

Created `nanobot/workspace/skills/lms/SKILL.md` with:
- Tool descriptions and when to use each
- Strategy for asking about labs without specifying one
- Output formatting guidelines

**Q: Show me the scores for Lab 01**
```
Here are the scores for Lab 01 – Products, Architecture & Roles:

Task Scores (Average Score / Attempts):

• Lab setup: 97.2% (119 attempts)
• Optional: Add a CI check: 25.0% (4 attempts)
• Optional: Create a release: 50.0% (2 attempts)
• Optional: Plan skill development: 0.0% (1 attempt)
• Optional: Resolve a merge conflict: 41.7% (6 attempts)
• Task 0: Practice the Git workflow: 65.2% (214 attempts)
• Task 1: Product & architecture description: 59.4% (90 attempts)
• Task 2: Roles and skills mapping: 53.9% (42 attempts)

Summary:
• The lab setup task has the highest average score at 97.2%
• Task 0 (Git workflow) has the most attempts at 214
• The optional "Plan skill development" task has the lowest average score at 0.0%
• Most tasks have average scores in the 50-65% range

Would you like me to get any other statistics for Lab 01, such as completion rates, group performance, or top learners?
```

**PASS** - Skill prompt guides agent to ask for lab name when not specified, and format results nicely.

---

## System Configuration

**LLM Provider**: OpenRouter (free tier)
- Model: `openrouter/free` (auto-selects best available free model)
- API Base: `https://openrouter.ai/api/v1`
- Context window: 200,000 tokens

**Backend**: Running on 127.0.0.1:42001
- LMS API Key: `mariachizhikova08`
- Database: Connected to postgres (Lab 8)

**Issue Fixed**: Qwen Code API OAuth free tier was discontinued (2026-04-15). Switched to OpenRouter free models.

---

## Task 2A — Deployed agent

<!-- TODO: Docker deployment -->

## Task 2B — Web client

<!-- TODO: Flutter web app screenshot -->

## Task 3A — Structured logging

<!-- TODO -->

## Task 3B — Traces

<!-- TODO -->

## Task 3C — Observability MCP tools

<!-- TODO -->

## Task 4A — Multi-step investigation

<!-- TODO -->

## Task 4B — Proactive health check

<!-- TODO -->

## Task 4C — Bug fix and recovery

<!-- TODO -->