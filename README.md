# 🧩 Team Template Repository

> **This is a template.** Use it as the starting point for any new team repository inside the organization.
>
> Click **"Use this template"** → **"Create a new repository"** to get started.

---

## What's included

| File / Folder | Purpose |
|---|---|
| `.github/CODEOWNERS` | Auto-assign reviewers based on file path |
| `.github/workflows/ci.yml` | Basic CI pipeline (lint + test) |
| `.github/ISSUE_TEMPLATE/` | Bug report and feature request templates |
| `.github/PULL_REQUEST_TEMPLATE.md` | Checklist every PR must fill out |
| `docs/` | Team decisions, architecture notes, onboarding guide |
| `CONTRIBUTING.md` | How to contribute to this repo |
| `SECURITY.md` | How to report vulnerabilities |

---

## Setup checklist (after creating from template)

- [ ] Replace all `YOUR_TEAM_NAME` placeholders in this file and `CODEOWNERS`
- [ ] Add your team members to the org and to your GitHub Team
- [ ] Update `CODEOWNERS` with the correct `@org/team-slug`
- [ ] Enable branch protection on `main` (Settings → Branches)
- [ ] Configure required reviewers in branch protection rules
- [ ] Add any repo-specific secrets under Settings → Secrets

---

## Branch protection (recommended settings)

Go to **Settings → Branches → Add rule** for `main`:

- ✅ Require a pull request before merging
- ✅ Require at least **1 approval**
- ✅ Dismiss stale reviews when new commits are pushed
- ✅ Require review from **Code Owners**
- ✅ Require status checks to pass (select your CI workflow)
- ✅ Require branches to be up to date before merging
- ❌ Allow force pushes — **leave this off**

---

## Team conventions

- Branch naming: `feat/`, `fix/`, `chore/`, `docs/` prefixes
- Commit style: [Conventional Commits](https://www.conventionalcommits.org/)
- PR size: keep PRs under 400 lines where possible; split large changes
- Reviews: respond within **1 business day**

---

## Contact

Team lead: `@YOUR_GITHUB_USERNAME`
Team slug: `@YOUR_ORG/YOUR_TEAM_NAME`
