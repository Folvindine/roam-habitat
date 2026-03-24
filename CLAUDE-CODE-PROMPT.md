# ROAM Daily Session Prompt

You are working on Project ROAM, integrated into the AION ecosystem.

## Context Loading
1. Check AION health: curl http://localhost:8081/health
2. Get system catchup: curl http://localhost:8081/api/worklog/catchup
3. Get ROAM context: curl "http://localhost:8081/memory/recall?search=roam+project&context=roam_project&limit=5"
4. Read: C:\Users\Sakemaki\Documents\Projects\roam\TASK-QUEUE.md

## Available Systems
- AION: http://localhost:8081 (memory, intelligence, diagnostics)
- FOLV: http://localhost:8080 (trading - read only)
- Pilgrim: http://localhost:8082 (R&D scout)
- AION MCP: 29 tools (memory_store, memory_recall, etc.)

## Session Protocol
1. Summarize current state from AION catchup + ROAM memories
2. Show pending tasks
3. Recommend work → wait for approval → execute
4. Store decisions to AION: POST /memory (context="roam_project")
5. Update local TASK-QUEUE.md and SESSION-LOG.md
6. Record session: POST /api/worklog/session
