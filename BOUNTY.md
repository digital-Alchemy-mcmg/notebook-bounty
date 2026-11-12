# SDNA Python Extraction Bounty Brief

## Objective

Create a Python notebook that reads the provided synthetic candidate documents
and emits atomic evidence blurbs grounded in those sources.

An atomic evidence blurb communicates one independently supportable fact. It must
remain faithful to the source and carry enough provenance for an evaluator to
find the supporting passage. Competitors choose their own extraction approach.
This brief does not prescribe segmentation, semantic decomposition, or claim
extraction architecture.

## Inputs

All competitors receive the same public files under `synthetic_sources/`. They
are fictional and exist only for this bounty. Do not introduce private evaluator
materials or confidential source documents into a public fork.

## Required result fields

Return a JSON array. Every item must contain:

| Field | Requirement |
| --- | --- |
| `builder_id` | The builder identifier recorded in the notebook |
| `source_file` | Repository-relative path of the supporting source |
| `source_locator` | Human-checkable location, such as section and paragraph or line range |
| `source_quote` | Verbatim source text supporting the blurb |
| `evidence_blurb` | One concise, independently supportable fact |

Additional fields are allowed if documented. Save the final array to
`output/results.json`. The starter notebook creates the output directory but
does not produce claims.

## Source fidelity

- Do not add facts absent from the cited passage.
- Do not combine independently supportable facts into one blurb.
- Preserve names, dates, quantities, units, qualifications, and negation.
- A quote and locator must let a reviewer verify each blurb against its source.
- Make uncertainty or conflict visible rather than silently resolving it.
- Do not treat headings, filenames, or metadata as evidence unless the source
  itself supports the blurb.

## Deliverable

Submit one executed notebook based on `starter.ipynb`, its generated
`output/results.json`, and the evidence described in `SUBMISSION.md`. The
notebook must run in the repository's Codespaces environment from a clean clone.

## Out of scope

Downstream classification, spreadsheets, workbook routing, pipeline execution,
and private evaluation are not notebook responsibilities. No internal system
architecture or private answer key is included here.

## Evaluation boundary

The operator evaluates submissions separately against an unpublished rubric and
private materials, if any. Public synthetic examples are development inputs, not
an answer key. Reward, legal terms, schedule, private scoring details, and the
official submission channel must be supplied by the operator before launch.
