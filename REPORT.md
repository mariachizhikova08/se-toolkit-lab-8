# Lab 8 — Report

Paste your checkpoint evidence below. Add screenshots as image files in the repo and reference them with `![description](path)`.

## Task 1A — Bare agent

**Q: What is the agentic loop?**
```
I've completed processing but have no response to give.
```

**Q: What labs are available in our LMS?**
```
I've completed processing but have no response to give.
```

*Note:* The Qwen Code API model (qwen-coder) returns a `get_items` tool call for EVERY request regardless of the prompt or tools provided. This appears to be a model/endpoint configuration issue - the model always returns `tool_calls: [{name: "get_items", arguments: {}}]` with no content.

## Task 1B — Agent with LMS tools

**Q: What labs are available?**
```
I've completed processing but have no response to give.
```

**Q: Is the LMS backend healthy?**
```
I've completed processing but have no response to give.
```

*Note:* MCP tools are registered correctly (9 tools: lms_health, lms_labs, lms_learners, lms_pass_rates, lms_timeline, lms_groups, lms_top_learners, lms_completion_rate, lms_sync_pipeline). The LMS backend is healthy (verified: `status='healthy' item_count=56`). The issue is the Qwen model's response format.

## Task 1C — Skill prompt

LMS skill prompt was created at `nanobot/workspace/skills/lms/SKILL.md`.

**Q: Show me the scores**
```
I've completed processing but have no response to give.
```

## Task 2A — Deployed agent

<!-- Paste a short nanobot startup log excerpt showing the gateway started inside Docker -->

## Task 2B — Web client

<!-- Screenshot of a conversation with the agent in the Flutter web app -->

## Task 3A — Structured logging

<!-- Paste happy-path and error-path log excerpts, VictoriaLogs query screenshot -->

## Task 3B — Traces

<!-- Screenshots: healthy trace span hierarchy, error trace -->

## Task 3C — Observability MCP tools

<!-- Paste agent responses to "any errors in the last hour?" under normal and failure conditions -->

## Task 4A — Multi-step investigation

<!-- Paste the agent's response to "What went wrong?" showing chained log + trace investigation -->

## Task 4B — Proactive health check

<!-- Screenshot or transcript of the proactive health report that appears in the Flutter chat -->

## Task 4C — Bug fix and recovery

<!-- 1. Root cause identified
     2. Code fix (diff or description)
     3. Post-fix response to "What went wrong?" showing the real underlying failure
     4. Healthy follow-up report or transcript after recovery -->