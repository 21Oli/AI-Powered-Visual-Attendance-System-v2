# AI-Powered Visual Attendance System v2

A long-term, production-oriented computer-vision project for portfolio use and future adaptation to business or government environments.

## Current status

Phase 1 — Computer Vision Core, Step 01 — Project Setup & Environment is complete. The repository currently contains only the project foundation; no camera, face processing, enrollment, attendance, API, database, dashboard, liveness, or deployment capability has been implemented.

## Repository layout

```text
├── docs/                 # Future project documentation
├── notebooks/            # Exploratory notebooks (when approved)
├── src/                  # Application source (not yet implemented)
├── data/
│   ├── employees/        # Local employee data; not committed
│   ├── face_samples/     # Local face samples; not committed
│   ├── embeddings/       # Generated embeddings; not committed
│   └── logs/             # Generated local logs; not committed
├── models/               # Downloaded/generated model artifacts; not committed
├── reports/              # Generated reports; not committed
└── tests/                # Tests (not yet implemented)
```

Empty folders are retained with `.gitkeep` placeholders. Generated content in local data, logs, models, and reports folders is excluded by `.gitignore`.

## Setup

The setup was verified with Python 3.13.1. Use a virtual environment for all local development.

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

Verify the foundation dependencies:

```powershell
python -c "import cv2, numpy; print(f'OpenCV {cv2.__version__}; NumPy {numpy.__version__}')"
```

`.env` is reserved for local, sensitive configuration and is ignored by Git. `.env.example` is safe to commit and currently contains no configuration values because configuration is scheduled for Phase 1, Step 02.

## Development workflow

Follow the project rule for every approved roadmap step:

**ONE STEP → IMPLEMENT → RUN → VERIFY → FIX → DOCUMENT → COMMIT → NEXT STEP**

See [PROJECT_PLAN.md](PROJECT_PLAN.md), [DEVELOPMENT_STATUS.md](DEVELOPMENT_STATUS.md), and [ARCHITECTURE.md](ARCHITECTURE.md) before beginning work.

## License

This project is released under the [MIT License](LICENSE).
