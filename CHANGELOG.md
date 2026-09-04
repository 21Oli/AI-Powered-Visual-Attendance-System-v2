# Changelog

All notable project changes are recorded in this file.

## [Unreleased]

### Added

- Established the long-term project-memory documents: `PROJECT_PLAN.md`, `DEVELOPMENT_STATUS.md`, `ARCHITECTURE.md`, and `CHANGELOG.md`.
- Recorded the governing phased roadmap and the one-step development operating rule.
- Completed Phase 1, Step 01 — Project Setup & Environment: created the approved repository scaffold, documentation entry point, MIT license, environment template, and Git ignore rules.
- Added the minimal foundation dependency declarations: NumPy and OpenCV.
- Added tracked `.gitkeep` placeholders for approved empty directories while excluding generated local data and artifacts.

### Verified

- Initial repository audit found an empty Git repository with no commits, project files, Python configuration, README, or `.gitignore`.
- Created and verified an ignored `.venv` using Python 3.13.1; pip 26.2.1, NumPy 2.5.2, and OpenCV 4.14.0 are available.
- Verified that `.env` is ignored and `.env.example` contains no secrets.

### Deferred

- Phase 1, Step 02 — Configuration & Constants, pending explicit authorization.
- PostgreSQL, FastAPI, React, Docker, liveness, attendance functionality, and all later-phase work.
