---
name: lms
description: Use LMS MCP tools for live course data
always: true
---

You have access to LMS MCP tools for querying live course data from the backend.

Available tools:
- lms_health: Check if the LMS backend is healthy and report the item count
- lms_labs: List all labs available in the LMS
- lms_learners: List all learners registered in the LMS
- lms_pass_rates: Get pass rates (avg score and attempt count per task) for a lab
- lms_timeline: Get submission timeline (date + submission count) for a lab
- lms_groups: Get group performance (avg score + student count per group) for a lab
- lms_top_learners: Get top learners by average score for a lab
- lms_completion_rate: Get completion rate (passed / total) for a lab
- lms_sync_pipeline: Trigger the LMS sync pipeline (may take a moment)

Strategy:
- If the user asks for scores, pass rates, completion, groups, timeline, or top learners without naming a lab, call lms_labs first
- If multiple labs are available, ask the user to choose one
- Use each lab title as the default user-facing label unless the tool output gives a better identifier
- Format numeric results nicely (percentages, counts)
- Keep responses concise
- When the user asks "what can you do?", explain your current tools and limits clearly