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
| `SRC-001` | Ploesser doctoral thesis, *A Design Theory for Context-Aware Information Systems* | Karsten Ploesser; QUT repository record | `raw/KARSTEN-PLOESSER-CONTEXT-AWARE-INFORMATION-SYSTEMS-THESIS-2013.pdf` | `sources/PLOESSER-CONTEXT-AWARE-INFORMATION-SYSTEMS-2013.md` | reviewed | author use; reproduction rights unconfirmed | Primary authority for the 2013 design theory, supervision, and acknowledgment. Cite or paraphrase; do not reproduce figures without a rights check. |
| `SRC-002` | Springer computer-science proceedings author instructions | Springer Nature | `raw/SPRINGER-COMPUTER-SCIENCE-PROCEEDINGS-AUTHOR-INSTRUCTIONS.pdf` | `sources/SPRINGER-LNCS-AUTHOR-GUIDANCE-2024.md` | reviewed | reference use | Generic October 2024 guidance. Volume-specific editor instructions override it. |
| `SRC-003` | Context-aware BPM publications, 2008-2011 | Named publication authors and publishers | primary publisher and repository records | `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md` | reviewed | citation use | Intellectual lineage from extrinsic context drivers to the CAIS thesis. |
| `SRC-004` | Language-agent research: ReAct, Reflexion, AgentBench | Named publication authors | primary paper and conference records | `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md` | reviewed | citation use | Evidence for environment interaction, feedback memory, and capability limits. |
| `SRC-005` | AI-augmented BPM and Large Process Models | Named publication authors and publishers | ACM and Springer records | `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md` | reviewed | citation use | Bridge from process-aware systems to generative-AI architectures. |
| `SRC-006` | Rosemann et al., three AI-era BPM drifts | Michael Rosemann et al.; Springer Nature | DOI `10.1007/s10257-024-00689-9` | `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md` | reviewed | CC BY 4.0 citation use | Central contemporary Michael Rosemann source. |
| `SRC-007` | Agentic BPM manifesto and formal foundations | Named publication authors; Elsevier and preprint authors | DOI `10.1016/j.is.2026.102738`; arXiv `2604.17347` | `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md` | reviewed | citation use | Current 2026 research frontier; recheck publication status before submission. |

## Intake Rules

- Preserve original files in `raw/`.
- Use semantic, uppercase base filenames for normalized source notes.
- Do not alter normalized source content to improve a story. Put interpretation and synthesis in `analysis/` or `drafts/`.
- Record who supplied each item, when it was received, and whether that person controls publication rights.
- Track permission separately for text, images, artwork, recordings, and substantial quotations.
- Remove the placeholder inventory row after the first real source is recorded.
