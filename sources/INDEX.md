# Source Index

## Purpose

Track every source, submission, image, recording, quotation, and reference used or considered for the festschrift. Preserve provenance and publication status from intake through final approval.

## Status Values

- `staged`: original exists in `raw/` but has not been normalized or reviewed.
- `normalized`: a read-only working representation exists in `sources/`.
- `reviewed`: editorial relevance and provenance have been checked.
- `approved`: the contributor or rights holder has approved the intended use.
- `restricted`: material is retained for private context but is not cleared for publication.
- `excluded`: material will not be used in the current edition.

## Inventory

| ID | Source | Contributor or rights holder | Original path | Normalized path | Status | Permission | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| `[SRC-001]` | `[description]` | `[name or unknown]` | `[raw/path]` | `[sources/path or pending]` | `[status]` | `[unknown, requested, granted, restricted]` | `[provenance and intended use]` |

## Intake Rules

- Preserve original files in `raw/`.
- Use semantic, uppercase base filenames for normalized source notes.
- Do not alter normalized source content to improve a story. Put interpretation and synthesis in `analysis/` or `drafts/`.
- Record who supplied each item, when it was received, and whether that person controls publication rights.
- Track permission separately for text, images, artwork, recordings, and substantial quotations.
- Remove the placeholder inventory row after the first real source is recorded.
