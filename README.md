# FinFlow — Main Repo

Umbrella repository for **FinFlow**: personal finance / subscription tracking. It wires the **frontend** and **backend** as **[Git submodules](https://git-scm.com/book/en/v2/Git-Tools-Submodules)** so you keep three separate GitHub repos while still cloning everything in one tree.

| Piece | GitHub | Role |
|--------|--------|------|
| This repo | **[FinFlow — Main Repo](https://github.com/ChamathDilshanC/FinFlow---Main-Repo)** | Wrapper + submodule pointers |
| Frontend | **[FinFlow — Frontend](https://github.com/ChamathDilshanC/FinFlow---Frontend)** | Client UI |
| Backend | **[FinFlow — Backend](https://github.com/ChamathDilshanC/FinFlow---Backend)** | FastAPI + PostgreSQL |

Display names use spaces (“FinFlow - …”); GitHub turns them into repo paths like `FinFlow---Frontend` (hyphens). Always copy URLs from the repository **Code** button on GitHub.

## Clone with submodules

```bash
git clone --recurse-submodules https://github.com/ChamathDilshanC/FinFlow---Main-Repo.git
cd FinFlow---Main-Repo
```

If you already cloned without submodules:

```bash
git submodule update --init --recursive
```

## Pull updates (frontend & backend)

```bash
git pull
git submodule update --remote --merge
```

Or enter each submodule and `git pull` as usual.

## Local layout

```
.
├── README.md          # this file
├── .gitmodules        # submodule URLs (managed by Git)
├── frontend/          # submodule → FinFlow — Frontend
└── backend/           # submodule → FinFlow — Backend
```

## Working on code

- **Backend:** see [`backend/README.md`](backend/README.md) — venv, `.env` from `.env.example`, `alembic upgrade head`, `uvicorn`.
- **Frontend:** see [`frontend/README.md`](frontend/README.md).

Secrets (`.env`, API keys) stay **uncommitted** inside each submodule per their `.gitignore`.

## GitHub CLI reference

Repos were created with [GitHub CLI](https://cli.github.com/) (`gh`), for example:

```bash
gh repo create "FinFlow - Backend" --private --source=. --remote=origin --push
```

Use the same pattern for new environments or forks (adjust names/remotes).

## Contributing & attribution

**Maintainer:** [ChamathDilshanC](https://github.com/ChamathDilshanC).  

IDE and automation tools (including **Cursor** / “Cursor Agent”) are **not** listed as project contributors; they are tooling only.

## License

Add a `LICENSE` here or in each submodule when you publish.
