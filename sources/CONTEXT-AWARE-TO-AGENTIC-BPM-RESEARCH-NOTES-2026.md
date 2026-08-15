# Context-Aware to Agentic BPM Research Notes, 2026

## Purpose and Cutoff

This note records the primary sources used to connect the 2013 CAIS design theory to current language agents, AI-augmented BPM, and Agentic Business Process Management (APM). Sources were checked on 2026-08-15. The 2026 literature is emerging and should not be represented as settled consensus.

## Evidence Levels

- **Established source claim:** a claim made or demonstrated in the cited work.
- **Article synthesis:** the proposed mapping from CAIS to agentic process systems.
- **Research question:** an issue requiring conceptual, technical, or empirical study.

The article's five design principles are a synthesis, not a result reported by any one source.

## Early Context-Aware BPM Lineage

### Rosemann, Recker, and Flender (2008)

Rosemann, M., Recker, J., and Flender, C. (2008). Contextualisation of business processes. *International Journal of Business Process Integration and Management*, 3(1), 47-60. DOI: `10.1504/IJBPIM.2008.019347`.

- Shifts attention from the intrinsic flexibility of a process to the extrinsic conditions that create a need for flexibility.
- Identifies such drivers as time, location, weather, legislation, and performance requirements.
- Proposes an explicit classification and representation of relevant process context.
- Article use: establishes Michael's role in widening the process boundary from internal variation to environmental causes.

### Ploesser, Recker, and Rosemann (2011a)

Ploesser, K., Recker, J., and Rosemann, M. (2011). Supporting Context-Aware Process Design: Learnings from a Design Science Study. In *Business Process Management Workshops*, LNBIP 66, 97-104. DOI: `10.1007/978-3-642-20511-8_9`.

- Develops a context-aware process-design method and models through design-science work with an insurance provider.
- Article use: links the journal-level context argument to Karsten's design-theory program.

### Ploesser, Recker, and Rosemann (2011b)

Ploesser, K., Recker, J., and Rosemann, M. (2011). Challenges in the Context-Aware Management of Business Processes: A Multiple Case Study. *Proceedings of ECIS 2011*, paper 6, 51-62. Stable record: `https://aisel.aisnet.org/ecis2011/6/`.

- Critiques internally optimized but comparatively static process conceptualizations.
- Uses two cases to conceptualize processes as complex adaptive systems interacting with environmental conditions.
- Article use: supplies the empirical bridge from context classification to a socio-technical view of adaptation.

## Language Agents and Environment Interaction

### ReAct

Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., and Cao, Y. (2023). ReAct: Synergizing Reasoning and Acting in Language Models. *International Conference on Learning Representations*. Stable record: `https://openreview.net/forum?id=WE_vluYUL-X`; preprint: `https://arxiv.org/abs/2210.03629`.

- Interleaves language-model reasoning traces and task-specific actions.
- Actions allow an agent to retrieve new information from external sources or an interactive environment, while observations can update subsequent reasoning and plans.
- Demonstrates an architecture pattern, not a general guarantee of reliable perception, reasoning, or action.
- Article use: shows how the observation-action loop makes context selection and activation operational at run time.

### Reflexion

Shinn, N., Cassano, F., Gopinath, A., Narasimhan, K., and Yao, S. (2023). Reflexion: Language Agents with Verbal Reinforcement Learning. *Advances in Neural Information Processing Systems*, 36. Stable record: `https://openreview.net/forum?id=vAElhFcKW6`; preprint: `https://arxiv.org/abs/2303.11366`.

- Uses feedback, natural-language reflection, and episodic memory to influence later trials without updating base-model weights.
- Reports improvement over baselines across selected sequential decision-making, coding, and reasoning tasks.
- Article use: illustrates a limited implementation analogue of CAIS learning, while leaving governance, validity, and memory maintenance open.

### AgentBench

Liu, X., Yu, H., Zhang, H., et al. (2024). AgentBench: Evaluating LLMs as Agents. *International Conference on Learning Representations*. Stable preprint: `https://arxiv.org/abs/2308.03688`.

- Evaluates language-model agents across eight interactive environments.
- Reports meaningful capability in leading models but a substantial distance from practical usability, including weaknesses in long-horizon reasoning, decision-making, and instruction following.
- Article use: counterweight to claims that tool use or benchmark task completion establishes dependable organizational autonomy.

## AI-Augmented BPM

### Dumas et al. (2023)

Dumas, M., Fournier, F., Limonad, L., Marrella, A., Montali, M., Rehse, J.-R., Accorsi, R., Calvanese, D., De Giacomo, G., Fahland, D., Gal, A., La Rosa, M., Völzer, H., and Weber, I. (2023). AI-Augmented Business Process Management Systems: A Research Manifesto. *ACM Transactions on Management Information Systems*, 14(1), Article 11, 1-19. DOI: `10.1145/3576047`.

- Defines AI-augmented BPMSs as process-aware systems using trustworthy AI to make processes adaptable, proactive, explainable, and context-sensitive.
- Proposes lifecycle steps: frame, enact, perceive, reason, explain, adapt, and improve.
- Identifies five characteristics: framed autonomy, conversational actionability, adaptation, self-improvement, and explainability.
- Article use: the closest established BPM bridge between the CAIS structure and later APM.

### Kampik et al. (2025)

Kampik, T., Warmuth, C., Rebmann, A., et al. (2025). Large Process Models: A Vision for Business Process Management in the Age of Generative AI. *KI - Künstliche Intelligenz*, 39, 81-95. DOI: `10.1007/s13218-024-00863-8`.

- Envisions a Large Process Model that generates insights and actions for a process in a specific organizational context using heterogeneous data and knowledge across processes and contexts.
- Combines foundation-model correlation and generation with symbolic knowledge, queries, and reasoning.
- Keeps humans in control for important interpretations and changes and explicitly identifies feasibility limits and business and societal risks.
- Article use: supports the argument that a language model is one component of a context-aware process architecture, not the whole architecture.

## Michael Rosemann's Contemporary BPM Framing

### Rosemann et al. (2024)

Rosemann, M., vom Brocke, J., Van Looy, A., and Santoro, F. (2024). Business process management in the age of AI: Three essential drifts. *Information Systems and e-Business Management*, 22, 415-429. DOI: `10.1007/s10257-024-00689-9`.

- Proposes three field-level drifts: transaction to conversation, automation to autonomization, and simplification to sophistication.
- Distinguishes automation of predictable execution from autonomous processes that can make situational or structural decisions and may produce less predictable paths and outcomes.
- Argues that next-generation processes will be sensitive to contextual data and adapt accordingly.
- Calls for a taxonomy, modeling support, decision methods for appropriate autonomy, and responsible autonomization.
- Article use: closes a direct intellectual loop from Michael's 2008 external-context framing to his 2024 account of context-sensitive process autonomization.

## Agentic Business Process Management

### Calvanese et al. (2026)

Calvanese, D., Casciani, A., De Giacomo, G., Dumas, M., Fournier, F., Kampik, T., La Malfa, E., Limonad, L., Marrella, A., Metzger, A., Montali, M., Amyot, D., Fettke, P., Polyvyanyy, A., Rinderle-Ma, S., Sardiña, S., Tax, N., and Weber, B. (2026). Agentic Business Process Management: A Research Manifesto. *Information Systems*, 140, 102738. DOI: `10.1016/j.is.2026.102738`.

- Defines APM as an extension of BPM for governing autonomous agents executing organizational processes.
- Treats human and software agents as actors that perceive, reason, and act within explicit process frames.
- Positions process awareness as a way to constrain, align, and operationalize autonomy.
- Identifies four capabilities: framed autonomy, explainability, conversational actionability, and self-modification.
- Article use: principal current source. It provides the immediate research setting for the proposed CAIS-to-agentic mapping.

### De Giacomo et al. (2026)

De Giacomo, G., Kampik, T., Kirchdorfer, L., Montali, M., and Weinhuber, C. (2026). Formal Foundations of Agentic Business Process Management. Preprint. `https://arxiv.org/abs/2604.17347`.

- Models process execution as involving multiple autonomous decision-makers whose behavior cannot be fully controlled.
- Augments process specifications with goals and strategy-level guardrails.
- Article use: supports a research-agenda claim that action selection and autonomy need explicit goals, constraints, and formal reasoning, not merely prompts.
- Publication caution: cite as a 2026 preprint unless a version of record appears before submission.

## Proposed Continuity Map

This table is the Festschrift article's synthesis:

| 2013 CAIS requirement | Updated agentic-process principle | New implementation pressure |
| --- | --- | --- |
| Represent work system | Frame the socio-technical system, goals, roles, and constraints | Agents may alter both digital and human work, not just execute a modeled task |
| Represent relevant context | Select and maintain observations with provenance, freshness, and uncertainty | Retrieval and sensors increase volume, while model input remains selective and fallible |
| Specify adaptation strategies | Provide sufficient but bounded action variety | Tool calls can have immediate, external, and sometimes irreversible effects |
| Match situations to strategies | Select and trigger actions with traceability, timing, and escalation | Probabilistic reasoning replaces many explicit event-condition-action rules |
| Learn by changing representations and strategies | Govern memory, reflection, policy change, and self-modification | Learning can propagate error, drift, or manipulation unless reviewed and reversible |

## Distinctions the Article Must Preserve

### Context window versus context-awareness

An LLM context window is a bounded input sequence. It can contain instructions, retrieved text, memories, observations, tool results, and process state. It does not by itself:

- identify which external facts are relevant to organizational goals;
- establish the provenance, freshness, or reliability of those facts;
- model the social and technical system affected by an action;
- determine whether an action is authorized, timely, proportionate, or reversible;
- learn validly from outcomes.

The article's central inference is that context-awareness belongs to the whole socio-technical system and its governance, not to the model input alone.

### Adaptation versus agency

A CAIS may support humans who decide and act, automate pre-specified event-condition-action rules, or combine the two. Contemporary agentic systems may generate intermediate plans and select tools dynamically. The latter expands the action space and uncertainty but does not erase the earlier design requirements.

### Learning versus self-modification

Reflexion-style memory can change subsequent behavior without changing model weights. APM's self-modification is a broader system capability. The article should ask what may change, who approves it, how changes are evaluated, how provenance is retained, and how rollback works.

## Proposed Research Agenda

1. **Context boundaries:** How should an agent decide which signals matter, which sources it may access, and when ambiguity requires human interpretation?
2. **Requisite and restricted variety:** How much action variety is needed for resilience, and how should permissions, budgets, process constraints, and safe fallbacks bound it?
3. **Activation under uncertainty:** How can agents combine probabilistic beliefs, event timing, and explicit process constraints while exposing reasons and escalating appropriately?
4. **Governed learning:** Which memories, rules, prompts, tools, and process structures may change at run time, with what evidence, review, versioning, and rollback?
5. **Socio-technical outcomes:** How should evaluations measure not only task success, but also effects on human agency, work distribution, fairness, accountability, resilience, and organizational goals?

## Citation and Claim Cautions

- Do not describe ReAct as a universal architecture or interpret its reported task results as operational reliability.
- Do not describe Reflexion as validated organizational learning.
- Do not call a system context-aware simply because it uses retrieval, a long context window, tools, or memory.
- Do not present Large Process Models or APM as mature deployed standards.
- Do not imply that the five proposed principles have been empirically evaluated.
- Update the current-literature scan immediately before submission because the 2026 APM field is moving quickly.
