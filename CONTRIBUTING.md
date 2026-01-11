# 🌟 Contributing to **Smart Resume Reviewer**

<div align="center"><img src="assets/SRR-logo.png" style="width: 220px; height: 220px;"  alt="Smart-Resume-Review Logo" /></div>

---

Thank you for your interest in contributing to **Smart Resume Reviewer**! Your contributions help improve the project and empower users to review resumes smarter and faster. This document explains how to contribute, the workflow to follow, and standards we expect.

---

## 🚀 Quick start (TL;DR)

1. Create an issue describing your change.
2. Wait for assignment from a maintainer.
3. Fork the repo and create a branch: `issue-<number>-short-description`.
4. Make changes, add tests, run lint/format.
5. Push and open a Pull Request linking the issue.

---

## 🧭 Contribution Workflow (Must Follow)

### 1) Create an Issue First

Before writing code, open a new issue with:

- Title: short, descriptive
- Description: what you want to change and why
- Reproduction steps / screenshots / logs (if applicable)
- Proposed implementation (optional)

Issue template (suggested):

- Problem summary:
- Proposed change:
- Steps to reproduce / test:
- Screenshots / attachments:

This prevents duplicate work and helps maintainers prioritize.

### 2) Wait for Assignment

Do NOT start working until a maintainer assigns the issue. Maintainers may ask clarifying questions or suggest a different approach.

### 3) Fork & Clone

Fork the repository on GitHub, then clone your fork:

```bash
git clone https://github.com/your-username/Smart-Resume-Reviewer.git
cd Smart-Resume-Reviewer
```

### 4) Create a Branch

Use a descriptive branch name including the issue number:

```
git checkout -b issue-<number>-short-description
```

Examples:

- `issue-12-add-dark-mode`
- `issue-34-fix-upload-crash`

### 5) Make Small, Focused Commits

- Keep PRs focused and small.
- Write clear commit messages following Conventional Commits (see below).

### 6) Run Locally & Add Tests

Install dependencies and run the app locally:

```bash
pip install -r requirements.txt
streamlit run app.py
```

If you add logic, include unit tests where feasible (project uses pytest if available). Ensure tests pass before opening a PR.

### 7) Linting & Formatting

Follow PEP8. Use black/isort/flake8 if you have them configured locally. Remove debug prints and unused imports.

### 8) Commit & Push

Commit examples:

```
git add .
git commit -m "fix(upload): avoid crash on empty file (closes #34)"
git push origin issue-34-fix-upload-crash
```

### 9) Open a Pull Request

Open the PR in the original repository (not your fork). In the PR description:

- Explain what you changed and why
- Link the issue: `Closes #<issue-number>`
- Include screenshots for UI changes
- Describe testing steps for reviewers

---

## 📐 Branch & Commit Conventions

Branch naming:

- `issue-<number>-short-description`

Commit messages (Conventional Commits):

- feat: add new resume section analyzer
- fix: resolve file upload crash
- docs: improve README and contributing guide
- refactor: optimize text preprocessing logic
- style: formatting and indentation fixes

Include the issue number in commit or PR message when applicable (e.g., `fix: parse dates correctly (closes #12)`).

---

## 🧪 PR Checklist (Please complete before requesting review)

- [ ] Issue created and assigned
- [ ] Branch name follows convention
- [ ] Code runs without errors
- [ ] No debug prints or commented-out blocks
- [ ] Tests added/updated (if applicable)
- [ ] Documentation updated if needed
- [ ] Linter/formatter run
- [ ] PR description is clear and includes links to related issues

Maintainers may request changes; please respond to review comments promptly.

---

## 🛠 Development & Testing Details

- To run the app: `streamlit run app.py` (ensure required Python version from `requirements.txt`).
- Unit tests: `pytest` (if tests are present).
- Model files are in `models/` and generated PDFs are in `generated/`.
- Use `data/` for sample inputs; do not commit large files to the repo.

---

## 🧾 Code Style & Best Practices

- Follow PEP8 and write clear docstrings for new modules/functions.
- Keep functions small and focused.
- Avoid hard-coded values; prefer configuration or constants.
- Add logging instead of print statements for non-interactive code.

---

## 🔒 Security & Sensitive Data

- Do NOT commit secrets (API keys, passwords). If you accidentally commit secrets, contact maintainers immediately.
- For security issues, open a private disclosure according to the repository's SECURITY.md.

---

## 📣 Communication

- Ask questions on the issue thread.
- If you need help, tag a maintainer or open a discussion.
- For larger changes, propose the design in the issue before implementing.

---

## 🧾 Templates (Suggested)

Issue template (copy into the issue body):

```
Title:

Problem summary:

Steps to reproduce:

Expected behaviour:

Proposed solution:

Screenshots / attachments:
```

Pull Request template (copy into PR description):

```
Summary of changes:

Related issue: Closes #<number>

How to test:

Screenshots (if any):

Checklist:
- [ ] Tests added/updated
- [ ] Lint/format ran
- [ ] Documentation updated
```

---

## 🧡 Thank you

Every contribution — big or small — helps improve **Smart Resume Reviewer**. We appreciate your effort and enthusiasm. If you have any questions while contributing, please ask in the issue thread.

---

_Maintainers: Add or update guidelines here as the project evolves._
