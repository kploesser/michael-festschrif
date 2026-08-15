# Agent Instructions

## Purpose

This project develops Karsten Ploesser's invited scholarly contribution to an LNCS Festschrift honoring Professor Michael Rosemann's contributions to Business Process Management (BPM).

The article traces an intellectual line from Karsten's 2013 doctoral research, *A Design Theory for Context-Aware Information Systems*, to contemporary AI-augmented and agentic systems that perceive, reason about, act within, and learn from their environments.

The immediate goal is a rigorous, personal, and submission-ready chapter that explains what changed between context-aware information systems and agentic AI, what did not change, and what the earlier design theory contributes to the governance of agentic business processes.

Ask for permission before overwriting or deleting user-provided files. Preserve superseded manuscript versions in `archive/` when revisions become material.

## Folder Guidance

Use a shallow project structure organized by artifact purpose.

Use lowercase folder names.

Use uppercase base filenames with lowercase file extensions for steering, analysis, source, and draft files, except for generated files in `output/`.

Keep only steering files, project-management files, and standard repository metadata in the root folder:

- `README.md`
- `AGENTS.md`
- `MEMORY.md`
- `SESSION-LOG.md`
- `STYLE-GUIDE.md`
- `TODO.md`

Keep read-only normalized research notes and bibliographic records in `sources/`. Treat source files as read-only unless the user explicitly asks to correct source material.

Use `raw/` for original PDFs and other source assets. Do not alter original source files.

Keep argument design, literature synthesis, Festschrift framing, conceptual mappings, and submission analysis in `analysis/`.

Keep editable article manuscripts and working prose in `drafts/`.

Keep superseded manuscript snapshots in `archive/`.

Keep generated LNCS, Word, and PDF exports in `output/`.

## Core Files

- `raw/KARSTEN-PLOESSER-CONTEXT-AWARE-INFORMATION-SYSTEMS-THESIS-2013.pdf`: authoritative thesis source.
- `raw/SPRINGER-COMPUTER-SCIENCE-PROCEEDINGS-AUTHOR-INSTRUCTIONS.pdf`: generic Springer proceedings guidance. Volume-specific instructions take precedence.
- `sources/PLOESSER-CONTEXT-AWARE-INFORMATION-SYSTEMS-2013.md`: normalized thesis findings and page references.
- `sources/CONTEXT-AWARE-TO-AGENTIC-BPM-RESEARCH-NOTES-2026.md`: current literature record and evidence boundaries.
- `analysis/FESTSCHRIFT-BRIEF.md`: confirmed scope, thesis, and open submission decisions.
- `analysis/FESTSCHRIFT-FRAMING-AND-OUTLINE-01.md`: tone guidance, article architecture, and author-input questions.
- `drafts/CONTEXT-THEN-AND-NOW-FESTSCHRIFT-ARTICLE-01.md`: current manuscript.

## Research Integrity

- Use the thesis PDF as the authority for Karsten's 2013 design theory. The thesis title page is dated December 2012; the repository and subsequent citations identify the completed doctorate as 2013. Preserve that distinction when it matters.
- Do not invent post-2013 research activity, present-day empirical findings, personal anecdotes, supervisory conversations, or claims about Michael's influence.
- Use Karsten's thesis acknowledgments as the only source for personal supervision claims until Karsten provides more detail.
- Cite primary research papers or official publisher records for technical and historical claims.
- Distinguish established findings, conceptual synthesis, proposed design principles, and future research questions.
- Describe current agentic AI capabilities cautiously. Do not equate benchmark demonstrations with dependable organizational autonomy.
- Treat the 2026 Agentic BPM literature as emerging. Do not present its terminology or architecture as settled consensus.
- Distinguish an LLM context window from organizational or process context. A context window contains representations; context-awareness requires selecting and interpreting information relevant to system goals.
- Do not reproduce thesis figures or tables in the article without confirming whether permission is required. Prefer a new conceptual mapping unless the user requests reuse.
- Keep all quotations short, exact, attributed, and page-checked.

## Festschrift Positioning

- Write a scholarly contribution first and a tribute through the choice of problem, intellectual lineage, and reflective framing.
- Use a warm first-person opening and closing, but keep the technical core analytical and evidence-based.
- Connect the article specifically to Michael's work on context-aware BPM and his later framing of conversational BPM, process autonomization, and process sophistication.
- Avoid generic praise, biography, or a catalogue of Michael's achievements.
- Make the author's independent contribution clear: a conceptual bridge from the five CAIS meta-requirements to design principles for context-aware agentic process systems.
- Preserve room for one concrete personal recollection supplied by Karsten.

## LNCS Conventions

- Use the official Springer LNCS template for the submission artifact.
- Use American English unless the volume editors instruct otherwise.
- Include title, author and affiliation details, abstract, keywords, numbered sections, acknowledgments if appropriate, disclosure of interests, and references.
- Use numeric citations and include DOI or stable primary-source links where available.
- Treat 12 to 15 LNCS pages as a provisional full-paper planning range only. The volume invitation and editors' page limit override the generic guidance.
- Keep the abstract self-contained and free of citations.
- Number only the first two heading levels in the final LNCS artifact.
- Create alt text for all figures and other non-text content.
- Confirm the volume's policy for disclosure of generative-AI assistance before submission.

## Terminology and Style

- Use `context-aware information system` and `CAIS` for the 2013 design-theory class.
- Use `AI-augmented BPM system` and `ABPMS` for the 2023 manifesto's system class.
- Use `agentic business process management` and `APM` only when discussing the 2026 manifesto or explicitly extending it.
- Use `agentic system` as the broader technical term.
- Do not capitalize `agentic` unless it begins a title or sentence.
- Prefer `perceive, reason, act, and learn` when describing the agent loop, while noting that implementations vary.
- Use `Michael` in personal reflections and `Rosemann et al.` in scholarly claims.
- Use short paragraphs, explicit transitions, and concrete distinctions.
- No em dashes.
