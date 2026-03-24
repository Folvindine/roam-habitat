# ROAM Revised Architecture

## Key Decision (2026-03-24)
AION already IS the central vault. No separate roam-vault needed.

## How ROAM Uses AION
- Memory storage: `POST /memory` with `context="roam_project"`
- Memory recall: `GET /memory/recall?context=roam_project`
- Blueprint: `BLUEPRINT:ROAM:INTEGRATION` canonical key
- Pilgrim: Researches ROAM topics in daily rotation
- Laila: `[ACTION:ROAM:NOTE/STATUS/IDEAS]` action tags

## File Strategy
```
C:\Users\Sakemaki\Documents\Projects\roam\
├── website/          (GitHub Pages deployment)
├── docs/             (project documentation)
├── simulation/       (future ROS2 work)
├── TASK-QUEUE.md     (active task tracking)
├── SESSION-LOG.md    (session history)
└── README.md         (project overview)
```

## Future Expansion
- Navigation AI in simulation/ (ROS2 + Gazebo)
- Hardware firmware in firmware/ (Raspberry Pi 5)
- Habitat design in habitat/ (CAD files, 3D print models)
