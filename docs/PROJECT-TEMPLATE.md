# ROAM Project Template

## Adding a New ROAM Component

### 1. Create the component folder
```
roam/<component_name>/
├── README.md          (component overview)
├── requirements.txt   (if Python)
└── src/               (source code)
```

### 2. Store in AION memory
```bash
curl -X POST http://localhost:8081/memory -H "Content-Type: application/json" -d '{
  "action": "ROAM component: <name>",
  "details": "<what it does, key decisions>",
  "context": "roam_project",
  "importance": 7,
  "memory_type": "procedural"
}'
```

### 3. Update TASK-QUEUE.md
Add relevant tasks to the queue.

### 4. Update SESSION-LOG.md
Log what was built and why.

## Convention
- All ROAM memories: `context="roam_project"`
- All ROAM blueprints: `BLUEPRINT:ROAM:*` canonical keys
- All ROAM Pilgrim research: stored with `context="roam_project"`
