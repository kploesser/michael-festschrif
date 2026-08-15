# Memory

## Project Goal

Draft Karsten Ploesser's scholarly contribution to an LNCS Festschrift honoring Professor Michael Rosemann's contributions to Business Process Management.

The article should show the evolution from Karsten's 2013 research on context-aware information systems to contemporary artificial intelligence, including agentic systems that interact with and adjust actions to their environment.

## Confirmed Scope

- Author: Karsten Ploesser.
- Honoree: Professor Michael Rosemann.
- Field: Business Process Management.
- Publication form: chapter in an LNCS Festschrift volume.
- Historical anchor: Karsten's doctorate, *A Design Theory for Context-Aware Information Systems*.
- Contemporary destination: AI-augmented and agentic systems, with particular attention to environmental interaction and adaptation.
- Required tone: scholarly and appropriate to the German academic Festschrift tradition, with framing help for the author.

## Source Baseline

- The thesis title page is dated December 2012 and identifies Michael Rosemann as principal supervisor and Jan Recker as associate supervisor.
- The completed doctorate is conventionally cited as 2013, matching the user's framing.
- The thesis defines a context-aware information system as an adaptive socio-technical system that responds to relevant context change by modifying how humans and machines perform work.
- The thesis develops five CAIS meta-requirements: represent the work system, represent relevant context, specify adaptation strategies, match situations to strategies, and learn by modifying context representations and strategies.
- The thesis acknowledgments thank Michael Rosemann and Jan Recker for their advice, patience, and guidance while Karsten worked full time.
- The thesis is preserved in `raw/KARSTEN-PLOESSER-CONTEXT-AWARE-INFORMATION-SYSTEMS-THESIS-2013.pdf`.

## Contemporary Research Baseline

- ReAct demonstrated an interleaved reasoning and action pattern in which actions retrieve new observations from external sources or environments.
- Reflexion demonstrated improvement across trials using linguistic feedback and episodic memory without updating model weights.
- AgentBench found meaningful agent capabilities but persistent weaknesses in long-horizon reasoning, decision-making, and instruction following.
- The 2023 AI-augmented BPM manifesto described systems that are framed, autonomous, context-sensitive, adaptive, explainable, and self-improving.
- Large Process Models combine generative correlation with symbolic knowledge and reasoning to produce context-specific process insights.
- Rosemann and coauthors' 2024 paper describes drifts from transactions to conversations, automation to autonomization, and simplification to sophistication.
- The 2026 Agentic BPM manifesto reframes human and software agents as actors that perceive, reason, and act within explicit process frames, emphasizing framed autonomy, explainability, conversational actionability, and self-modification.

## Working Contribution

The article argues that a model's context window is not equivalent to context-awareness. The context window contains selected representations, while context-awareness is a design capability that determines which environmental information matters, how it changes system behavior, how actions remain aligned with goals and constraints, and how the system learns.

The proposed synthesis maps the five 2013 CAIS meta-requirements to five design principles for context-aware agentic process systems:

1. Frame the socio-technical work system and its goals.
2. Select and maintain relevant context, including uncertainty and provenance.
3. Provide sufficient but bounded action variety.
4. Match situations to actions with traceability and timely escalation.
5. Learn through governed updates to context models and action strategies.

This synthesis is conceptual. It is not presented as an empirically validated design theory.

## Festschrift Framing

An LNCS Festschrift chapter remains a substantive research article. The tribute should come through the problem selection, intellectual lineage, and a brief personal opening and closing. Avoid turning the chapter into biography or ceremonial praise.

The current draft uses Michael's early context-aware BPM work and later thinking about process autonomization as bookends. One specific personal memory from Karsten would strengthen the chapter.

## Open Inputs

- Volume title, editors, call for chapters, deadline, page limit, and review process.
- Karsten's current affiliation, corresponding email, and ORCID.
- One publication-cleared supervisory memory or anecdote involving Michael.
- Whether to include Karsten's post-2013 industry trajectory and, if so, which facts are cleared.
- Whether a current practical agentic-system example can be included.
- Required disclosure language for generative-AI assistance.

## Current Working State

- Repository scope and instructions reflect the confirmed submission.
- The thesis and generic Springer proceedings instructions are retained in `raw/`.
- Normalized source notes, a framing and outline memo, and manuscript v01 are present.
- `TODO.md` tracks factual, editorial, and production work.
- `SESSION-LOG.md` records chronological decisions.

## Cold-Start Sequence

1. Read `AGENTS.md`.
2. Read `README.md`.
3. Read `TODO.md`.
4. Read `analysis/FESTSCHRIFT-BRIEF.md`.
5. Read `analysis/FESTSCHRIFT-FRAMING-AND-OUTLINE-01.md`.
6. Read the current article draft.
7. Read the latest section of `SESSION-LOG.md`.
8. Continue from the newest user instruction without inventing open inputs.
