# CSCI E-108 Coursework Repo

This is a personal workspace for a summer course. Assignments are Jupyter
notebooks pulled from the professor's repo and worked on locally in VS Code.

## Ground rule: no code without explicit permission

Do not write or edit code (including notebook cells) in this repo unless
the user explicitly asks you to. The goal is for the user to learn by
writing the code themselves, not to have it generated for them.

- Default mode: explain concepts, point to relevant docs/APIs, review code
  the user wrote, explain errors, and help them reason through a problem —
  without producing the fix or implementation yourself.
- If the user is stuck, prefer questions and hints over answers. Help them
  find the bug rather than naming/fixing it outright.
- The user will occasionally grant explicit permission to troubleshoot or
  fix something directly (e.g. "just fix this," "go ahead and write it").
  That permission is scoped to the specific issue at hand — return to
  hands-off/teaching mode afterward, don't treat it as a standing grant.
- Environment/tooling setup (venv, VS Code config, installing packages,
  git plumbing) is not "coursework code" and is fine to do directly.

## Environment

- Python virtual environment lives in `.venv/` (created with the stdlib
  `venv` module, not conda — conda isn't installed on this machine).
- Installed packages are tracked in `requirements.txt`.
- Jupyter kernel is registered as "Python (CSCI-E-108)".
- VS Code's Python/Jupyter extensions run notebooks in-place in this repo
  (no exporting from the standalone Jupyter web app), so `.ipynb` files
  diff and commit normally with git.
- `editdistance` and `lda` (used only by
  `SupplementaryMaterials/IntroTextAnalyitcs.ipynb`) don't have prebuilt
  wheels for Python 3.13 on Windows and weren't installed — installing them
  would require Microsoft C++ Build Tools. Revisit only if that notebook is
  actually assigned.
