# Lab 8 — Report

## Task 1A — Bare agent

**Q: What is the agentic loop?**

```
🐈 nanobot
The agentic loop is a conceptual model for how an autonomous AI (or any
intelligent agent) continuously interacts with its environment to achieve goals.
It can be broken down into four recurring steps:

1. Perceive / Observe – The agent gathers information from its surroundings
   (e.g., sensor data, user input, API responses, file system state).
2. Reason / Plan – It processes that information, updates its internal model,
   and decides what to do next (selects actions, forms sub‑goals, or generates a
   plan).
3. Act / Execute – The agent carries out the chosen action(s) – sending a
   command, calling a tool, modifying a file, making a network request, etc.
4. Learn / Update – After acting, the agent receives feedback (success/failure
   signals, new observations, reward signals) and uses it to refine its model or
   policy, improving future decisions.

The loop repeats indefinitely, allowing the agent to adapt, correct mistakes,
and make progress toward its objectives. In practice, especially with tool‑using
LLMs like nanobot, the loop looks like:

while not goal_met:
    observe (read files, query APIs, get user input)
    think (determine next tool call or response)
    act   (call exec, read_file, edit_file, etc.)
    learn (interpret tool output, update internal state)

Key points:

• Closed‑feedback: Each action's result directly influences the next perception
  step, creating a tight feedback cycle.
• Goal‑driven: The loop is guided by an explicit or implicit objective (e.g.,
  "fetch the latest lab scores" or "schedule a reminder").
• Tool integration: For LLM agents, the "act" stage often means invoking
  external tools; the loop's power comes from being able to observe tool
  outputs and reason about them.
• Safety & alignment: Because the loop can keep iterating autonomously,
  safeguards (hard limits, human‑in‑the‑loop checks, tool‑access policies) are
  critical to prevent runaway behavior.
```

**Status**: PASS - Agent responds via OpenRouter free model.

---

## Task 1B — Agent with LMS tools

MCP tools registered:
- lms_health, lms_labs, lms_learners, lms_pass_rates, lms_timeline, lms_groups, lms_top_learners, lms_completion_rate, lms_sync_pipeline

**Q: What labs are available?**

```
🐈 nanobot
Hereare the available labs:                                                     

 1 Lab 01 – Products, Architecture & Roles                                      
 2 Lab 02 — Run, Fix, and Deploy a Backend Service                              
 3 Lab 03 — Backend API: Explore, Debug, Implement, Deploy                      
 4 Lab 04 — Testing, Front-end, and AI Agents                                   
 5 Lab 05 — Data Pipeline and Analytics Dashboard                               
 6 Lab 06 — Build Your Own Agent                                                
 7 Lab 07 — Build a Client with an AI Coding Agent                              
 8 lab-08 (no title specified)                                                  

Would you like more details about any specific lab?                             
```

**Status**: PASS - Agent returns real backend data via MCP tools.

---

## Task 1C — Skill prompt

Created `nanobot/workspace/skills/lms/SKILL.md` with tool usage strategy.

**Q: Show me the scores for Lab 01**

```
🐈 nanobot
I'll help you get the scores for Lab 01. Let me first check what labs are       
available and then get the pass rates for Lab 01.                              

🐈 nanobot
Here are the scores for Lab 01 – Products, Architecture & Roles:                

Lab 01 Pass Rates:                                                              

 • Lab setup: 97.2% (119 attempts)                                              
 • Optional: Add a CI check: 25.0% (4 attempts)                                 
 • Optional: Create a release: 50.0% (2 attempts)                               
 • Optional: Plan skill development: 0.0% (1 attempt)                           
 • Optional: Resolve a merge conflict: 41.7% (6 attempts)                       
 • Task 0: Practice the Git workflow: 65.2% (214 attempts)                      
 • Task 1: Product & architecture description: 59.4% (90 attempts)              
 • Task 2: Roles and skills mapping: 53.9% (42 attempts)                        

Summary:                                                                        

 • Highest score: Lab setup (97.2%)                                             
 • Lowest score: Optional: Plan skill development (0.0%)                        
 • Most attempts: Task 0: Practice the Git workflow (214)                       

Would you like me to analyze specific trends or focus on any particular section?
```

**Status**: PASS - Skill prompt guides agent to ask for lab name and format results nicely.

---

## System Configuration

- **LLM Provider**: OpenRouter (free tier) - model: `openrouter/free`
- **Backend**: 127.0.0.1:42001, API Key: `mariachizhikova08`
- **Database**: Connected to postgres (Lab 8)
- **Issue Fixed**: Qwen OAuth free tier discontinued (2026-04-15) → switched to OpenRouter

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