# FinFlow Mobile Platform - Main Repository

This is the umbrella repository for the FinFlow mobile product. It manages both the frontend and backend as Git submodules, so the full app can be cloned and developed from one place.

## Product Repositories

| Product Area | Repository | Purpose |
|---|---|---|
| Main | [FinFlow - Main Repo](https://github.com/ChamathDilshanC/FinFlow---Main-Repo) | Root workspace and submodule management |
| Frontend | [FinFlow - Frontend](https://github.com/ChamathDilshanC/FinFlow---Frontend) | Mobile UI built with React Native + Expo |
| Backend | [FinFlow - Backend](https://github.com/ChamathDilshanC/FinFlow---Backend) | REST API and business logic |

## Technology Stack

| Layer | Technologies (Name + Icon) |
|---|---|
| Frontend | ![Expo](https://img.shields.io/badge/Expo-000020?logo=expo&logoColor=white) ![React Native](https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white) ![NativeWind](https://img.shields.io/badge/NativeWind-06B6D4?logo=tailwindcss&logoColor=white) ![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?logo=supabase&logoColor=white) |
| Backend | ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?logo=sqlalchemy&logoColor=white) ![Alembic](https://img.shields.io/badge/Alembic-4B5563?logo=databricks&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white) |
| Main / DevOps | ![Git](https://img.shields.io/badge/Git-F05032?logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white) ![Git Submodules](https://img.shields.io/badge/Git%20Submodules-222222?logo=git&logoColor=white) |

## Quick Start

```bash
git clone --recurse-submodules https://github.com/ChamathDilshanC/FinFlow---Main-Repo.git
cd FinFlow
```

If already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Update Submodules

```bash
git pull
git submodule update --remote --merge
```

## Project Structure

```text
.
|-- README.md
|-- .gitmodules
|-- frontend/
`-- backend/
```

## Development Notes

- Frontend setup guide: `frontend/README.md`
- Backend setup guide: `backend/README.md`
- Keep secrets such as `.env` files out of version control.

## Maintainer

[ChamathDilshanC](https://github.com/ChamathDilshanC)
