# Visual Attendance System — Architecture

## Architecture status

Architecture is intentionally not implemented yet. This document records the agreed boundaries so the initial setup does not prematurely create later-phase systems.

## Phased architecture boundary

| Phase | Responsibility | Current state |
| --- | --- | --- |
| Phase 1 | Local computer-vision core: camera input, face processing, recognition, verification, unknown handling, attendance events, evaluation | Planned |
| Phase 2 | Attendance and business rules | Deferred |
| Phase 3 | PostgreSQL persistence and FastAPI services | Deferred |
| Phase 4 | Web dashboard | Deferred |
| Phase 5 | Security, RBAC, and audit | Deferred |
| Phase 6 | Docker packaging and deployment | Deferred |
| Phase 7 | Advanced liveness, performance optimization, and production hardening | Deferred |

## Phase 1 logical flow (planned)

```text
Camera input
  → Face detection
  → Face quality assessment
  → Face embedding / recognition
  → Temporal multi-frame verification
  → Known or unknown decision
  → Attendance event engine
```

Enrollment is a separate Phase 1 flow:

```text
Multiple employee face images
  → Quality assessment
  → Embedding generation
  → Embedding storage
```

## Current implementation constraints

- Step 01 — Project Setup & Environment is complete; no application architecture or behavior has been created.
- Do not introduce database, API, dashboard, containerization, liveness, or attendance implementations before their scheduled phases or steps.
- Design decisions made during Phase 1 must preserve clean separation between computer-vision concerns and later persistence, API, UI, security, and deployment layers.
