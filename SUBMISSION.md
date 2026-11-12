# Submission Procedure

Submit from your fork, not by changing the authoritative repository.

## Prepare the package

1. Complete and commit `ACKNOWLEDGEMENT.md`.
2. Restart the notebook kernel and run all cells from top to bottom in the
   Codespaces environment.
3. Confirm `output/results.json` is valid JSON and contains the documented fields.
4. Save the executed `starter.ipynb` with its cell outputs visible.
5. Commit all implementation files needed for a clean run. Do not commit secrets,
   credentials, caches, virtual environments, or private evaluator material.
6. Push the final commit to your fork and record its full 40-character SHA.

## Execution evidence

Include:

- the immutable GitHub URL for the final commit in your fork;
- the executed `starter.ipynb` at that commit;
- `output/results.json` at that commit;
- a screenshot or text capture showing **Restart Kernel and Run All Cells**
  completed without error in Codespaces; and
- the Python version and UTC execution timestamp printed by the starter notebook.

## Send

Send the package through the channel and before the deadline designated by the
operator. A pull request to this authoritative repository is not a submission
unless the operator explicitly says otherwise. The official channel, deadline,
reward, eligibility terms, and any required disclosure form remain operator
dependencies and must be announced before the bounty opens.
