# Lab 8 — Report

## Task 1A — Bare agent

**Q: What is the agentic loop?**
```
The **agentic loop** is the core cycle that an autonomous AI agent follows to accomplish tasks. It's the fundamental pattern that separates an agent from a simple chatbot.

 1 Observe — The agent reads the user's request and the current state (files, tools, context).
 2 Reason — The agent decides what to do next. Should I call a tool? Read a file? Search the web? Ask for clarification?
 3 Act — The agent executes the chosen action (e.g., call a tool, run a command, write a file).
 4 Observe Results — The agent reads the output of its actions and evaluates whether it succeeded or needs to adjust.
 5 Repeat — Based on the results, the agent loops back: it may take another action, revise its plan, or conclude the task and report back to the user.

Unlike a simple chatbot that just responds once, an agent iterates — it can retry failed actions, chain multiple tools together, self-correct, and continue working until the task is truly complete.
```

**Q: What labs are available in our LMS?**
```
Here are the labs available in your LMS:

 #  Lab Title
 ──────────────────────────────────────────────────────────
 1   Lab 01 – Products, Architecture & Roles
 2   Lab 02 — Run, Fix, and Deploy a Backend Service
 3   Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4   Lab 04 — Testing, Front-end, and AI Agents
 5   Lab 05 — Data Pipeline and Analytics Dashboard
 6   Lab 06 — Build Your Own Agent
 7   Lab 07 — Build a Client with an AI Coding Agent
 8   lab-08

There are 8 labs in total. Would you like me to pull any analytics for a specific lab (pass rates, completion rates, group performance, timeline, top learners)?
```

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
Here are the available labs:

 1 Lab 01 – Products, Architecture & Roles
 2 Lab 02 — Run, Fix, and Deploy a Backend Service
 3 Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4 Lab 04 — Testing, Front-end, and AI Agents
 5 Lab 05 — Data Pipeline and Analytics Dashboard
 6 Lab 06 — Build Your Own Agent
 7 Lab 07 — Build a Client with an AI Coding Agent
 8 Lab 08 — lab-08

Want me to pull any stats on a specific lab (pass rates, completion, top learners, etc.)?
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
Here are the available labs:

 1 Lab 01 – Products, Architecture & Roles
 2 Lab 02 — Run, Fix, and Deploy a Backend Service
 3 Lab 03 — Backend API: Explore, Debug, Implement, Deploy
 4 Lab 04 — Testing, Front-end, and AI Agents
 5 Lab 05 — Data Pipeline and Analytics Dashboard
 6 Lab 06 — Build Your Own Agent
 7 Lab 07 — Build a Client with an AI Coding Agent
 8 Lab 08 — lab-08

Which lab would you like to see the scores for? Or would you like me to show an overview of all of them?
```

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