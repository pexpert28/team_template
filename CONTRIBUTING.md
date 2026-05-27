# Contributing

Thanks for contributing! Follow these steps to keep things smooth for everyone.

---

## Getting started

```bash
git clone https://github.com/YOUR_ORG/YOUR_REPO.git
cd YOUR_REPO

python -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

---

## Workflow

1. **Branch off `main`** — never commit directly to `main`

   ```bash
   git checkout -b feat/your-feature-name
   ```

2. **Branch naming conventions**

   | Prefix | Use for |
   |---|---|
   | `feat/` | New features |
   | `fix/` | Bug fixes |
   | `chore/` | Maintenance, dependency updates |
   | `docs/` | Documentation only |
   | `refactor/` | Code changes with no functional effect |

3. **Commit style** — use [Conventional Commits](https://www.conventionalcommits.org/):

   ```
   feat: add station metadata endpoint
   fix: handle missing timestamp in parser
   docs: update setup instructions
   ```

4. **Run checks before pushing**

   ```bash
   black .
   flake8 . --max-line-length=120
   pytest tests/ -v
   ```

5. **Open a Pull Request** against `main`, fill in the PR template, and request a review.

---

## Rules

- Do **not** commit credentials, API keys, or `.env` files — use environment variables
- Keep PRs focused: one concern per PR
- All CI checks must pass before merge
- At least one approval from a Code Owner is required

---

## Questions?

Open an issue or ping `@YOUR_ORG/YOUR_TEAM_NAME` on GitHub.
