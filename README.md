# DevOps Assignment – Version Control with Git & GitHub

## Project Description

This repository demonstrates core Git and GitHub workflows as part of a DevOps assignment. It covers:

- Initializing a local Git repository
- Connecting to a remote GitHub repository
- Creating and working on feature branches
- Opening, reviewing, and merging Pull Requests
- Cloning an existing project (Django Todo App) and deploying it to a live hosting platform

## Assignment Goals

1. Understand how to manage a codebase using Git version control.
2. Practice collaborative workflows using GitHub (branching, PRs, merging).
3. Deploy a real-world Django web application to a public hosting service.

## Author

DevOps Student – Batch 09

## Repository Structure

```
Assignment/
├── README.md          # This file
└── Ostad_batch-09/    # Cloned Django Todo App (see Part 6)
```

## Related Links

- **Todo App Repository**: https://github.com/latifurrafi/Ostad_batch-09
- **Live Deployed App**: https://django-todo-app-xxxx.onrender.com *(update after deployment)*

---

## Git Workflow Summary

### Branches
| Branch | Purpose |
|--------|---------|
| `main` | Stable production-ready code |
| `feature-update` | Feature development branch (merged via PR) |

### Commit Convention
- `feat:` – New feature
- `fix:` – Bug fix
- `docs:` – Documentation changes
- `deploy:` – Deployment configuration

---

## Part 6 – Todo App Deployment Notes

The Todo application from [Ostad_batch-09](https://github.com/latifurrafi/Ostad_batch-09) has been:
1. **Cloned** locally into `Ostad_batch-09/`
2. **Updated** with production-ready settings (WhiteNoise, Gunicorn, environment variables)
3. **Configured** for Render deployment via `render.yaml` and `Procfile`
4. **Deployed** to Render (free tier)

### Deployment Steps Used
1. Forked the repo to personal GitHub account
2. Added `gunicorn` and `whitenoise` to `requirements.txt`
3. Created `Procfile` with: `web: gunicorn todo_project.wsgi --log-file -`
4. Created `render.yaml` for one-click deployment
5. Updated `settings.py` to read `SECRET_KEY` and `DEBUG` from environment variables
6. Connected Render to the forked GitHub repo and deployed

