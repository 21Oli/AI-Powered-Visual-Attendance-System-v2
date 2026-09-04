# Visual Attendance System — Project Plan

## Purpose

Visual Attendance System is a long-term, production-oriented computer-vision project for portfolio use, with an architecture that can later be adapted for business or government environments.

## Development operating rule

Every roadmap step follows this sequence exactly:

1. Implement
2. Run
3. Verify
4. Fix
5. Document
6. Commit
7. Proceed to the next step

Only the active step may be implemented. Do not begin a later step or phase until the active one is complete, verified, documented, and committed.

## Roadmap

### Phase 1 — Computer Vision Core

1. Project structure & environment
2. Configuration & constants
3. Employee data model
4. Live camera service
5. Face detection
6. Face quality assessment
7. Multi-image face enrollment
8. Face embedding generation
9. Embedding storage
10. Face recognition
11. Temporal / multi-frame verification
12. Unknown-face handling
13. Attendance event engine
14. Testing & evaluation
15. Phase 1 integration demo

### Later phases (out of scope until Phase 1 is complete)

- Phase 2 — Attendance and business rules
- Phase 3 — PostgreSQL and FastAPI
- Phase 4 — Web dashboard
- Phase 5 — Security, RBAC, and audit
- Phase 6 — Docker and deployment
- Phase 7 — Advanced liveness, optimization, and production improvements

## Current scope

**Active phase:** Phase 1 — Computer Vision Core
**Most recently completed step:** Step 01 — Project Setup & Environment
**Status:** COMPLETED — awaiting explicit authorization for Step 02

## Explicit deferrals

Do not create or implement PostgreSQL, FastAPI, React, Docker, liveness, attendance functionality, or any later-phase capability during Step 01.
