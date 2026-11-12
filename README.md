# SDNA Python Notebook Bounty

This public repository is the common starting point for an independent notebook
bounty. Build a Python/Jupyter implementation that extracts source-grounded,
atomic evidence blurbs from the documents in `synthetic_sources/`.

This repository is competition infrastructure, not an invitation or announcement.
The operator will separately authorize the start of the bounty.

## Before you participate

1. Read [`BOUNTY.md`](BOUNTY.md).
2. Copy [`ACKNOWLEDGEMENT_TEMPLATE.md`](ACKNOWLEDGEMENT_TEMPLATE.md) to
   `ACKNOWLEDGEMENT.md` in your fork. Record your GitHub identity and acceptance
   of the rules. Committing an acknowledgment is required, but it does not and
   cannot prevent anyone from viewing this public repository.
3. Fork this repository into your own GitHub account. Do not develop on the
   operator's authoritative `main` branch.
4. From your fork, select **Code → Codespaces → Create codespace on main**.
5. Open `starter.ipynb`, select the Python kernel, record your builder identifier,
   and run the notebook.
6. Build your own extraction implementation in the marked workspace. Inspect and
   save your results in your fork.

## Submission

Follow the package checklist in [`SUBMISSION.md`](SUBMISSION.md). Submit the
immutable commit URL from your fork, the executed notebook, result artifact, and
execution evidence through the operator-designated channel by the
operator-designated deadline. Those operator-controlled details are intentionally
not guessed here.

## Repository map

- `BOUNTY.md` — public scope, deliverable, and output requirements
- `ACKNOWLEDGEMENT_TEMPLATE.md` — required participant acknowledgment template
- `SUBMISSION.md` — submission package and evidence checklist
- `synthetic_sources/` — identical public test inputs for every participant
- `starter.ipynb` — runnable starting notebook, without an extraction solution
- `.devcontainer/devcontainer.json` — GitHub Codespaces configuration
- `requirements.txt` — pinned minimum notebook dependencies

## Boundary

This bounty ends at Python extraction. It excludes downstream classification,
Google Sheets or workbook routing, pipeline execution, private evaluator answers,
and the operator's internal architecture. Evaluation happens separately. Do not
place confidential or proprietary material in a public fork.
