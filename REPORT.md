# Lab 8 — Report

## Task 1A — Bare agent

**Q: What is the agentic loop?**
```
The agentic loop is the core cycle that an AI agent goes through to accomplish tasks autonomously. Instead of just generating a single response to a prompt (like a standard chatbot), an agent repeatedly cycles through a series of steps to achieve a goal.

Here's the typical flow:

 1 Perception (Observe)
   The agent gathers information from its environment — user input, tool outputs, file contents, API responses, or sensor data. It builds a current understanding of the state of the world.
 2 Planning (Reason)
   Based on the observed state and the goal, the agent decides what to do next.
 3 Action (Execute)
   The agent carries out the planned step, calling tools, sending messages, or triggering processes.
 4 Reflection (Evaluate & Learn)
   After acting, the agent observes the result and decides whether to loop back or terminate.

This loop transforms AI from a reactive text generator into an autonomous problem-solver.
```

**Q: What labs are available in our LMS?**
```
Here are the labs available in your LMS:

 1 Lab 01 – Products, Architecture & Roles
 2 Lab 02 — Run, Fix, and Deploy a Backend Service
 3 Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4 Lab 04 — Testing, Front-end, and AI Agents
 5 Lab 05 — Data Pipeline and Analytics Dashboard
 6 Lab 06 — Build Your Own Agent
 7 Lab 07 — Build a Client with an AI Coding Agent
 8 lab-08

Would you like more details about any specific lab?
```
Note: The bare agent accessed this information by searching local repo files (inspecting documentation) — not via live LMS backend access.

## Task 1B — Agent with LMS tools

MCP tools are registered:
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
Here are the 8 labs available in your LMS:

 #  Lab Title
 ──────────────────────────────────────────────────────────
 1  Lab 01 – Products, Architecture & Roles
 2  Lab 02 — Run, Fix, and Deploy a Backend Service
 3  Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4  Lab 04 — Testing, Front-end, and AI Agents
 5  Lab 05 — Data Pipeline and Analytics Dashboard
 6  Lab 06 — Build Your Own Agent
 7  Lab 07 — Build a Client with an AI Coding Agent
 8  lab-08

Would you like me to pull any stats on a specific lab (pass rates, completion rate, top learners, group performance, or submission timeline)?
```

**Q: Is the LMS backend healthy?**
```
Yes, the LMS backend is healthy! It currently has 56 items stored.
```

## Task 1C — Skill prompt

Created `nanobot/workspace/skills/lms/SKILL.md` with:
- Tool descriptions and when to use each
- Strategy for asking about labs without specifying one
- Output formatting guidelines

**Q: Show me the scores**
```
I'll check what labs are available in the LMS first.

There are 8 labs available. Which lab would you like to see scores for?

 1 Lab 01 – Products, Architecture & Roles
 2 Lab 02 — Run, Fix, and Deploy a Backend Service
 3 Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4 Lab 04 — Testing, Front-end, and AI Agents
 5 Lab 05 — Data Pipeline and Analytics Dashboard
 6 Lab 06 — Build Your Own Agent
 7 Lab 07 — Build a Client with an AI Coding Agent
 8 Lab 08 — lab-08

Or I can pull scores for all of them if you'd like a full overview.
```
Note: The skill prompts the agent to ask which lab when not specified, instead of making assumptions.

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