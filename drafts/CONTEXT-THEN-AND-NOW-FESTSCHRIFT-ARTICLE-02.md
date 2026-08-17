# Context Is More Than a Window: From Context-Aware Information Systems to Agentic Business Processes

<!--

- Review title: it should say "context then and now"
- Align with expectations for an LNCS "Festschrift" in tone and style
- Review line by line and annotate
- Produce a general workable version without applying any extra "thinking" work
- Only then address conceptual gaps such as the statement that Agentic Systems are the first true CAIS

-->

<!--

Chapter flow

1. Introduction
   - Write this last: memorable moment or influence
2. Before Agency: Moving Context Into the Process Frame
   - System + Adaptation
3. The 2013 CAIS Design Theory
   - Properties of CAIS
   - Innovation: System + Context, Adaptation, Activation, and Learning
4. What Agentic AI Changes
   - Properties of Agentic AI
   - Notion of context in Agentic AI
5. From AI-Augmented BPM to Agentic BPM
   - Properties of APM
6. Five Principles for Context-Aware Agentic Process Systems
   - Mapping APM onto CAIS = contingencies
7. What Changed and What Did Not
   - Mapping contingencies to resolutions
8. A Research Agenda for Context-Aware Agency
   - Research agenda for identified resolutions
9. Conclusion: Context as a Way of Seeing

Each section maps to one bounded essay and reflection on an emerging topic of question. The section opener stitches section together in a seamless narrative flow.

-->

Karsten Ploesser
[AUTHOR INPUT: current affiliation]
[AUTHOR INPUT: city and country]
[AUTHOR INPUT: corresponding email and ORCID]

## Abstract

In 2013, I proposed a design theory for context-aware information systems: socio-technical systems that recognize relevant changes in their environment and adapt how people and machines perform work. Today, language-model-based agents can gather observations, reason over them, use tools, and modify later behavior in response to feedback. These capabilities make context-driven adaptation executable at a new scale, but they do not make the underlying design problem disappear. This conceptual article reconstructs five meta-requirements of the earlier design theory and relates them to AI-augmented and agentic business process management. It argues that a model's context window is a container for selected representations, whereas context-awareness is a property of a governed socio-technical system. The article translates the five meta-requirements into principles for framing the work system, maintaining relevant context, bounding action variety, connecting situations to actions, and governing learning. The resulting synthesis offers a research agenda for agentic process systems whose autonomy is context-sensitive, explainable, and organizationally accountable.

**Keywords:** context-awareness · agentic artificial intelligence · business process management · adaptive systems · socio-technical systems · design theory

## 1 Introduction: A Question That Returned

<!-- This requires more work. The fact that I did my doctoral research while working full time is irrelevant to the topic -->

More than a decade ago, while completing a doctorate at Queensland University of Technology under the supervision of Michael Rosemann and Jan Recker and continuing to work full time, I asked what an information system must know about its environment to adapt effectively. In the acknowledgments to the thesis, I thanked Michael and Jan for guiding me along the "rocky road to completion" [11, p. 15]. Time has turned that road into an unexpectedly direct route to a current question: what must an artificial-intelligence agent know, and how should it be governed, when it can act on the world it observes?

<!-- AUTHOR INPUT: Replace or supplement the published acknowledgment with one concrete memory of Michael's intellectual or supervisory influence. An ideal detail is a question, diagram, or reframing that changed how Karsten understood context or BPM. -->

The question has returned because the boundary between information and action has moved. A conventional language model generates an output from an input. An agentic system can place that model in a loop: observe a state, form or revise a plan, invoke a tool, receive the resulting observation, and act again. Its tools may search a knowledge base, update a record, allocate a resource, send a message, or trigger another system. Memory and feedback can also influence later attempts. What was previously a design question about recognizing context and recommending an adaptation can therefore become a run-time question about whether software should take an action that changes the process and its environment.

This technical change is consequential for Business Process Management (BPM). The field has long supplied models, rules, roles, controls, and lifecycle methods for organizing work. It is now being asked to frame systems whose process paths and intermediate decisions may not be fully determined in advance. Research on AI-augmented BPM systems describes a lifecycle of framing, enacting, perceiving, reasoning, explaining, adapting, and improving [7]. More recent Agentic Business Process Management (APM) research treats human and software agents as actors that perceive, reason, and act within explicit process frames [3]. Michael and his coauthors describe the corresponding field-level movement as, among other changes, a drift from automation to autonomization [15].

This contemporary discussion also returns to a much earlier move in context-aware BPM. In 2008, Michael Rosemann, Jan Recker, and Christian Flender argued that process flexibility research needed to examine not only a process's intrinsic ability to vary but also the extrinsic conditions that create a need for variation [14]. Weather, location, legislation, customer conditions, and other environmental variables were not merely background. They could explain why a process that worked yesterday no longer achieved its purpose today. Our subsequent work developed empirical and design-science accounts of that problem [12, 13]. My thesis then generalized it into a design theory for Context-Aware Information Systems (CAIS) [11].

This article asks: **What can the CAIS design theory contribute to the design and governance of contemporary agentic business processes?** I answer through a conceptual reconstruction and synthesis. First, I recover the socio-technical assumptions and five meta-requirements of the 2013 theory. Second, I distinguish organizational context-awareness from the more limited idea of a large language model's context window. Third, I map the earlier requirements to five proposed principles for agentic process systems:

1. Frame the socio-technical work system and its goals.
2. Select and maintain relevant context.
3. Provide sufficient but bounded action variety.
4. Match situations to actions with traceability and escalation.
5. Learn through governed change.

The mapping is not offered as an empirically validated extension of the original design theory. Nor does it suggest that the 2013 work anticipated the technical form of current language agents. Rather, it identifies a continuity in the design problem. Probabilistic generation, tool use, memory, and run-time planning alter how adaptation can be realized. They do not remove the need to define the system, determine what matters, bound possible actions, decide when to act, and evaluate what the system learns.

That continuity is also the article's Festschrift connection. Michael's influence on this line of work was not only to supply an answer about context. It was to widen the frame of the question. The early work looked beyond the process model to its environment. His recent work asks BPM to look beyond automation toward conversation, autonomization, and sophistication [15]. The sections that follow trace an idea between those two moments and propose where it might go next.

## 2 Before Agency: Moving Context Into the Process Frame

<!-- Lit Review -->

### 2.1 From Internal Flexibility to External Causes

At the time of the early context-aware BPM work, process flexibility was often described through what a process could change internally: an alternate path, a configurable model, an exception handler, or an ad hoc deviation. Such mechanisms were necessary, but they began after the need for change had already become apparent. They said comparatively little about the environmental conditions that made one variant more suitable than another.

Rosemann, Recker, and Flender addressed this gap by distinguishing intrinsic process flexibility from its extrinsic drivers [14]. Their context framework placed a process within nested environmental layers and treated contextual factors as possible causes of process variation. The important conceptual move was not simply to add more data to a process model. It was to ask which elements outside the process boundary could change whether the process achieved its goals.

This goal-relative view prevents context from expanding without limit. An organization exists amid countless facts, most of which should not influence a particular process decision. A weather forecast may matter to passenger facilitation but not to every accounting task. A change in regulation may be decisive for a claims process even when no case data have changed. A customer condition can be relevant at one activity and immaterial at another. Context therefore cannot be equated with everything observable around a system. It is selected by a relationship among an environmental variable, a work system, and an objective.

Our later studies carried this idea into process design and empirical inquiry. A design-science study developed method and model support for identifying context factors and relating them to process adaptations [13]. A multiple-case study of insurance claims handling and aviation passenger facilitation described business processes as complex adaptive systems rather than internally optimized but static arrangements [12]. The cases showed that context can affect technologies, information, task sequences, organizational structures, and people. They also showed that adaptation may be enacted by humans, machines, or both.

### 2.2 A Socio-Technical System, Not an Isolated Artifact

The thesis built on this work by adopting a work-system view of information systems [2, 11]. On this view, the system of interest is not only a software artifact. It includes human participants and machines performing activities with information, technology, and other resources to produce products or services. It is therefore socio-technical. Its components are interdependent, and its performance cannot be attributed to software in isolation.

That choice matters for adaptation. A technical component may detect an external change, while a person determines its meaning. A model may recommend a different process path, while an organizational role supplies authorization. A new tool may increase processing capacity but shift judgment to workers who lack the information or time to exercise it. An apparently successful automation can therefore be a poor system adaptation if it degrades human agency, accountability, or the quality of the resulting service.

The thesis adopted a representational view of context as information about the situation of a relevant entity [5, 11]. It also recognized a second tradition in which context is an occasioned property that emerges through interaction and cannot be fully encoded in advance [6]. The design theory concentrated on representable context because system design requires some way to identify, store, and reason about environmental conditions. Yet the interactional critique remains important. Any context representation is selective. It reflects a boundary, vocabulary, measurement practice, and purpose. The representation is not the situation itself.

This tension has become more, not less, significant with generative AI. Language models can accept unstructured descriptions and draw correlations across heterogeneous material. This can reduce the need to enumerate every contextual category in advance. It can also create an illusion that because more material can be processed, the relevant context has been captured. The old systems question then returns: relevant to which work, goal, stakeholder, and possible adaptation?

## 3 The 2013 CAIS Design Theory

<!-- Set A: CAIS Design Elements -->

### 3.1 Problem, Definition, and Scope

The thesis framed context-aware system design through three questions: what context is relevant, where context change affects an information system, and how the system should change in response [11, pp. 18-20]. It defined a CAIS as an adaptive system that responds when a context change impairs its production of information-based products or services by modifying how human participants and machines perform work [11, p. 22].

Several aspects of that definition deserve emphasis. First, awareness is tied to a change that matters for system purpose, not merely to sensing. Second, the object of adaptation is work, which can include social and technical components. Third, an adaptation may change the system or an element in its environment, consistent with a systems-theory account of adaptive behavior [1]. Fourth, effectiveness is ultimately an empirical matter. A response counts as useful because it improves the system's pursuit of its goals, not because it is technically elaborate.

The thesis used information-systems design theory to connect a class of recurring design problems, or meta-requirements, to a class of proposed solutions, or meta-design features, and then to testable propositions [8, 11]. It derived five meta-requirements from systems theory, socio-technical design, work-system theory, prior context-aware technologies, and the two cases. Table 1 presents the original logic in compact form.

**Table 1. The five CAIS meta-requirements and their design purposes**

| Construct | Meta-requirement | Design purpose |
| --- | --- | --- |
| System | Represent the work system | Make system variables and their interdependencies visible |
| Context | Represent relevant work-system context | Identify environmental variables, states, and impacts that matter to system goals |
| Adaptation | Specify behavioral adaptation strategies | Create a repertoire of responses sufficient for anticipated contextual variation |
| Activation | Match contextual situations to adaptation strategies | Connect signals and conditions to timely responses through rules and thresholds |
| Learning | Modify context representations and adaptation strategies | Improve later responses using evidence from context change and adaptation outcomes |

### 3.2 Five Requirements as a System

The requirements are most useful when treated as an interdependent system rather than a checklist. A context representation has no operational significance unless the work system and its purposes are known. An adaptation repertoire cannot be judged sufficient unless the contextual situations it must address have been considered. Activation cannot be judged timely or correct without a link among observations, goals, and authorized strategies. Learning is not improvement unless it revises those elements in ways that produce better outcomes.

**Representing the work system** establishes what is adapting. The thesis proposed models of tasks, technologies, structures, and people, including their interdependencies. This representation makes it possible to reason about joint optimization and tradeoffs rather than treating software behavior as the entire system.

**Representing relevant context** establishes why adaptation may be needed. Context models identify environmental entities and variables, the states those variables can assume, and their possible impacts on work. Relevance comes from the relationship to system purpose, while the representation provides an explicit and revisable hypothesis about that relationship.

**Specifying adaptation strategies** establishes what the system might do. The thesis connected this requirement to requisite variety: a system needs a sufficiently varied response repertoire to handle the environmental variety it encounters. Preparedness does not require predicting every event. It does require knowing which aspects of the system or environment may be changed and what tradeoffs those changes create.

**Matching situations to strategies** establishes when and under what conditions a response should occur. The 2013 meta-design relied substantially on event-condition-action rules, thresholds, and alternative levels of human involvement. The design goal was not maximum automation. It was lower response latency with a suitable allocation of sensing, interpretation, authorization, and action.

**Learning from context and adaptation** establishes how the system can improve. Learning can revise which context sources are used, which thresholds activate a response, and which strategies belong in the repertoire. It therefore differs from accumulating data. Learning changes a representation or a future choice based on evidence about relevance and effectiveness.

### 3.3 What the Theory Established, and What It Did Not

The thesis analytically evaluated whether the design theory was applicable to the case evidence and whether it could generate actionable recommendations. It found that the concepts could organize decisions observed in the cases and identify possible improvements in context modeling, adaptation strategies, activation rules, and learning [11, pp. 207-263]. This supplied a chain from empirical evidence and justificatory theory to design prescriptions.

<!-- Unclear where we're headed with this -->

The evaluation did not establish that a concrete CAIS implementation would reliably improve a live work system. The thesis explicitly called for expository instantiations and further empirical validation through methods such as experiments and focus groups [11, pp. 269-273]. Its literature review was selective, its cases were qualitative, and its utility evaluation was analytical. Those limits are particularly important when revisiting the work now. The five requirements provide a disciplined lens for examining agentic systems. Whether the translated principles improve their safety, effectiveness, or governance remains a question for design and evaluation.

## 4 What Agentic AI Changes

<!-- Set B: components of an Agentic System -->
<!-- Ref: Sutton's Agent-Environment Loop -->

### 4.1 From Producing an Answer to Changing a State

`Agentic AI` is used broadly and inconsistently. For this article, an agentic system is a computational system that pursues a goal through a sequence of environment-facing actions, incorporates observations of the resulting state, and adjusts later choices. This operational definition does not require claims about human-like understanding or general autonomy. It directs attention to a consequential capability: the system can do more than produce content for a person to interpret. It can participate in changing the state of a process.

The ReAct pattern provides a clear early illustration [17]. It interleaves model-generated reasoning with actions that query an external source or operate in an interactive environment. An action produces a new observation, which can change the plan and the next action. The important development for context-awareness is not the textual reasoning trace itself. It is the coupling among an incomplete representation, an environment-facing action, and new evidence. Context is sampled and revised during execution.

Reflexion adds a second capability [16]. Feedback on an attempt is converted into a natural-language reflection stored in episodic memory and used in later attempts. This can improve performance without updating the base model's weights. It also shows why the word `learning` needs precision. The model may be unchanged while the surrounding system changes the memories supplied to it. Learning can reside in a prompt, a retrieval store, a rule, a tool description, a process constraint, or a revised policy.

<!-- Not sufficiently connected to the rest of the argument -->

Neither pattern establishes dependable organizational agency. AgentBench evaluated language-model agents in eight interactive environments and found significant performance gaps, particularly in long-horizon reasoning, decision-making, and instruction following [10]. An agent that succeeds on selected benchmark tasks may still act on stale data, misread an ambiguous instruction, misuse a tool, fail to recover from an unexpected observation, or optimize a local objective at the expense of the work system. Interactive capability increases both the possible value and the possible cost of a contextual error.

### 4.2 Why a Context Window Is Not Context-Awareness

The contemporary use of the word `context` can obscure this problem. For a language model, the context window is the bounded sequence of tokens available for producing the next output. It may contain instructions, retrieved documents, process state, conversation history, memories, observations, and tool results. Increasing its size allows more representations to be considered at once. It does not determine whether those representations are the right ones.

A context window is therefore a container. Context-awareness is a design achievement of the surrounding system. At least five transformations occur before environmental conditions can guide responsible action:

1. **Sensing:** some aspect of the environment is made available as data.
2. **Selection:** the system decides, or inherits a decision about, which signals and sources matter.
3. **Representation:** observations are encoded, summarized, retrieved, and placed in relation to process state and goals.
4. **Interpretation and action:** the system infers what a situation means and chooses an authorized response.
5. **Evaluation and learning:** outcomes are assessed and some future representation or strategy may change.

An LLM can participate in several of these transformations. It cannot make their boundary choices disappear. Retrieval can omit decisive evidence or introduce irrelevant material. Summarization can erase a condition or its uncertainty. A tool result can be current yet come from an untrusted source. A long conversation can contain mutually inconsistent instructions. Environmental text can even be crafted to redirect the agent away from its authorized purpose. The context window holds the result of prior system decisions about access, relevance, ordering, and compression, whether those decisions were explicit or accidental.

<!-- This has the "It's Not X, It's Y" pattern of LLM text -->

The socio-technical boundary also remains. A process state may be fully represented at the data level and still be poorly understood because a customer's vulnerability, a worker's tacit knowledge, an informal dependency, or an ethical concern has not been encoded. Conversely, a model may infer a plausible condition that no authorized participant has verified. The design question is not only what the model receives. It is how observations, people, organizational rules, and technical components jointly establish a situation on which action may safely be based.

## 5 From AI-Augmented BPM to Agentic BPM

### 5.1 Process Awareness as a Frame for AI

The AI-Augmented Business Process Management Systems manifesto offers an important intermediate architecture [7]. It describes systems that frame and enact a process, perceive its state, reason about it, explain behavior, adapt execution, and improve over time. Such systems should act autonomously within a frame, support action through conversation, adapt, improve, and explain their behavior. The process frame supplies goals and constraints within which AI capabilities operate.

This formulation closely resembles the CAIS concern with system, context, adaptation, activation, and learning, although it introduces stronger autonomy and explainability requirements. Its contribution is not to attach an AI component to an otherwise unchanged workflow. It positions perception and reasoning inside the operational lifecycle and requires adaptations to remain process-aware. The process supplies a unit of purpose and accountability that a general model does not possess on its own.

The Large Process Model vision further resists a model-only architecture [9]. It proposes combining foundation-model generation and correlation with heterogeneous process data, organizational knowledge, symbolic models, queries, and reasoning. The authors emphasize human control for consequential interpretation and deployment decisions and retain non-LLM components for orchestration and guarantees. In this view, a language model helps contextualize and generate process knowledge, but context-specific action arises from an architecture of multiple forms of representation and control.

### 5.2 From Automation to Autonomization

Rosemann and coauthors place these technical developments within three broader BPM drifts: transaction to conversation, automation to autonomization, and simplification to sophistication [15]. All three involve context. Conversation allows process participants, including nonhuman participants, to exchange process and contextual information in natural language. Autonomization allows machines to assume parts of process governance and make situational or structural decisions. Sophistication seeks new process experiences and outcomes while introducing broader measures, including responsibility, fairness, privacy, and sustainability.

The distinction between automation and autonomization is central. Automation executes a path or rule that has been determined in advance. Autonomization delegates part of the selection or construction of that path. The resulting process may be more sensitive to a case and its environment, but it is also less predictable. That unpredictability is not automatically intelligence. It is transferred decision variety. BPM must determine where that variety is useful, how it is constrained, and who remains answerable for its effects.

The 2026 APM manifesto makes the framing problem explicit [3]. It treats human and software agents as primary functional entities that perceive, reason, and act within a process frame. Its four principal capabilities are framed autonomy, explainability, conversational actionability, and self-modification. A process frame constrains and aligns agency while allowing proactive pursuit of goals. Emerging formal work similarly models agents as autonomous decision-makers whose behavior cannot be completely controlled and uses goals and strategy-level guardrails to constrain their choices [4].

This literature supplies a contemporary answer to one part of the earlier CAIS problem: BPM can provide the frame in which action becomes process-aware. The remaining problem is how that frame becomes context-aware. A goal and a guardrail do not specify which observations should affect a decision, what uncertainty accompanies them, which response variety is appropriate, when human interpretation is required, or what evidence justifies changing future behavior. The CAIS requirements can be translated to make those concerns explicit.

## 6 Five Principles for Context-Aware Agentic Process Systems

Table 2 maps the five CAIS requirements to proposed principles for agentic process systems. The third column identifies what agentic technology makes newly urgent. The principles apply to the system around an agent, not only to the language model.

**Table 2. From CAIS meta-requirements to agentic-process design principles**

| CAIS requirement | Proposed agentic-process principle | New implementation pressure |
| --- | --- | --- |
| Represent the work system | Frame the socio-technical system, goals, roles, and constraints | Generated actions can reconfigure both digital and human work |
| Represent relevant context | Select and maintain observations with provenance, freshness, and uncertainty | Retrieval and sensors expand available data while model input remains selective and fallible |
| Specify adaptation strategies | Provide sufficient but bounded action variety | Agents can compose plans and invoke tools whose effects were not enumerated path by path |
| Match situations to strategies | Select actions with traceability, timing, and escalation | Probabilistic inference increasingly mediates between events and actions |
| Learn by modifying representations and strategies | Govern memory, reflection, policy change, and self-modification | Run-time changes can preserve improvement or propagate error and manipulation |

<!-- Where is this example sourced from? -->

A stylized passenger-disruption process illustrates the dependencies. An agent might monitor flight status, weather, passenger connections, staffing, and gate capacity; propose rebooking or resource-allocation actions; execute some changes within authority limits; escalate exceptional cases; and retain feedback about outcomes. This is not evidence from a deployed agentic system. It is a thought experiment derived from the type of work system examined in the original research. Even in this simplified scenario, no single model output establishes context-awareness. The system must determine what a successful passenger outcome is, which sources are trusted, what actions are permitted, when delay creates harm, and which outcome should alter future policy.

### 6.1 Principle 1: Frame the Socio-Technical System and Its Goals

The first principle asks what the agent is part of before asking what the agent can do. A useful frame specifies the process purpose, relevant outputs, affected stakeholders, human and software roles, information resources, tools, decision rights, and constraints. It also describes important interdependencies. If an agent reallocates a scarce resource, which activities lose it? If it accelerates case handling, whose review time is compressed? If it contacts a customer directly, which employee responsibility and communication policy are changed?

This extends the APM idea of framed autonomy with an explicitly socio-technical model. A process specification can define allowed sequences and goals, but the work system identifies whose work and outcomes those sequences constitute. That distinction matters because an agent may satisfy a local process metric while degrading the system's service, increasing hidden work, or displacing risk to a participant outside the modeled path.

The frame should also support multiple levels of goal. An immediate task objective, such as finding an alternate flight, sits within case goals, process goals, organizational obligations, and public or ethical constraints. Conflicts among these levels should not be left for a prompt to reconcile implicitly. The system needs priorities, non-negotiable restrictions, and conditions under which a person assumes the decision.

Evidence that this principle has been implemented would include more than a role prompt. It would include an explicit process or work-system boundary, versioned goals and policies, mappings between tools and decision rights, named owners for outcomes, and evaluation criteria covering both technical performance and effects on people.

### 6.2 Principle 2: Select and Maintain Relevant Context

The second principle treats a context model as a maintained hypothesis about what may affect goal achievement. For an agentic system, the model should identify sources, variables, entities, relationships, temporal properties, and confidence. An observation should carry enough provenance to answer where it came from, when it was valid, how it was transformed, and whether another participant confirmed it.

Relevance has both inclusion and exclusion costs. If the system excludes a decisive signal, its action may be inappropriate. If it includes every accessible signal, noise, conflict, privacy exposure, and manipulation risk grow. Selection should therefore be evaluated against specific decisions. Which observations could change the chosen action? Which are required by policy? Which should be unavailable because they are sensitive, discriminatory, or outside purpose? Which uncertainties should stop action rather than be silently completed by a plausible model inference?

Context also decays. Flight status, staffing, inventory, prices, customer consent, and legal conditions have different validity periods. Retrieval at the start of a plan may be obsolete before the action is executed. A context-aware agentic system should specify freshness requirements and revalidation points, particularly for consequential or irreversible actions. It should distinguish facts, estimates, inferred states, and instructions rather than flattening all text into one prompt.

Natural-language interaction does create an important opportunity. People can contribute situated information that is difficult to pre-model, question a system's interpretation, and explain why an exceptional condition matters. Conversation can therefore be a context-acquisition and context-negotiation mechanism. It should not be assumed to produce ground truth. Identity, authority, ambiguity, and conflict among accounts still require resolution.

### 6.3 Principle 3: Provide Sufficient but Bounded Action Variety

The third principle translates the CAIS adaptation repertoire into an agentic action space. A system facing varied conditions needs varied responses. A tool-using agent expands this repertoire because it can select and compose operations dynamically rather than choose only among complete paths enumerated at design time. Yet every tool, parameter, delegation, and plan composition also creates a possible state transition that must be governed.

The objective is neither maximum variety nor maximal restriction. Too little variety produces brittle automation that escalates every deviation or forces a poor standard response. Too much unrestricted variety exposes the organization to unauthorized changes, inconsistent treatment, resource overuse, and actions whose effects cannot be reversed. A bounded repertoire supplies enough flexibility for expected variation while constraining scope, cost, information access, and impact.

Several mechanisms can realize the boundary: least-privilege tool access, typed and validated parameters, transaction limits, resource budgets, process constraints, separation of proposal from execution, approvals for higher-impact actions, simulated execution, and compensating actions or rollback. The appropriate mechanism depends on consequence, uncertainty, and reversibility. An agent may autonomously retrieve status information, propose a reallocation, execute a low-cost rebooking within policy, and require human approval for an action that changes legal, financial, or safety obligations.

The action repertoire must include graceful non-action. Asking for clarification, gathering another observation, deferring until a condition is met, escalating to a named role, and stopping safely are legitimate strategies. Without them, a system optimized for completion may act precisely when its context representation is weakest.

### 6.4 Principle 4: Match Situations to Actions With Traceability and Escalation

The fourth principle concerns activation. Earlier CAIS designs could express much of the relationship through event-condition-action rules and thresholds. Agentic systems can use probabilistic inference and generate a plan that was not specified in complete form. This enables richer interpretation, but it makes the reason for action harder to locate.

A context-aware agentic system should retain a decision record that connects the action to the observed situation, relevant goal, applicable constraint, selected strategy, uncertainty, and authority. This record need not expose private model internals or a verbose reasoning trace. It should expose an auditable rationale at the level required to contest, review, and improve the decision. For example: which flight disruption was detected, which passenger constraint changed the normal policy, what alternatives were considered at the process level, why the selected action was within authority, and when the underlying information was last confirmed.

Timing is part of correctness. A safe response delivered too late may be ineffective, while a rapid response to an unverified signal may create unnecessary disruption. Activation policies should combine event time, information freshness, decision urgency, uncertainty, impact, and reversibility. Confidence alone is insufficient. A moderately uncertain but reversible action can sometimes proceed; a similarly uncertain irreversible action may require approval.

Escalation should be designed as a transfer of context, not merely a refusal. The receiving person or agent needs the relevant observations, unresolved ambiguity, attempted steps, constraints, and remaining decision time. Otherwise, automation lowers its own latency by imposing reconstruction work on the human participant. Effective escalation preserves both responsibility and the ability to act.

### 6.5 Principle 5: Learn Through Governed Change

The fifth principle asks what the system is allowed to change after an outcome. Agentic architectures can update memories, retrieval indexes, prompts, tool descriptions, routing policies, planning heuristics, process models, permissions, or even learned parameters. These changes have different scope and risk. Calling all of them `learning` hides the governance decision.

Governed learning begins with an outcome model. Task completion is not enough. The system should assess whether the action served the work-system goal, complied with constraints, created downstream work, affected stakeholders fairly, and remained robust after conditions changed. Feedback may come from process measures, a human review, an external event, or later consequences. Its source and delay influence what can validly be learned.

A learning record should link evidence to the proposed change and preserve provenance, version, evaluation, approval, and rollback. A reflection generated after failure can be useful working memory, as Reflexion demonstrates in bounded tasks [16]. In organizational use, that reflection may also be an incorrect causal story. Repetition can entrench the error if it is retrieved as fact on later cases. Memories should therefore carry type, source, confidence, retention period, and scope of applicability.

Self-modification raises the standard further. A system that changes its process strategy or tool policy changes the basis on which prior assurance was given. Low-risk modifications may be evaluated online within a controlled envelope. Structural changes should pass through tests, comparison against a baseline, approval by an accountable owner, staged deployment, monitoring, and a reversible release. Learning is context-aware only if the system can distinguish a genuine improvement from adaptation to noise, local optimization, manipulation, or a context that no longer applies.

## 7 What Changed and What Did Not

The mapping reveals continuity, not equivalence. Contemporary agentic systems differ substantially from the systems envisioned in 2013. They can interpret unstructured observations, generate intermediate plans in natural language, compose tool calls, converse with participants, and use feedback memory. They can construct a response at run time instead of selecting only a fully specified process variant. Multiple agents may also negotiate, delegate, and change one another's effective environment. These capabilities enlarge both the representational and action spaces.

The basis of action has changed as well. Explicit event-condition-action rules made activation logic inspectable, even when incomplete. A model-mediated choice may depend on statistical associations distributed across parameters, retrieved material, instructions, and interaction history. The system can respond to situations that its designers did not enumerate, but its decision boundary is harder to characterize. Explanation, evaluation, and recovery must therefore be designed into the surrounding process architecture.

What did not change is the open-system problem. An organization still pursues goals through interdependent human and technical work. Its environment contains more variation than any model can capture. Available information still differs from relevant and reliable information. A response repertoire can still be too narrow to handle variation or too broad to control. Acting too late, too early, or on the wrong signal still changes outcomes. Experience becomes learning only when it produces a valid improvement in future behavior.

The most important discontinuity may therefore be one of consequence. Earlier context-aware systems often placed a recommendation or rule between context recognition and human action. An agent can collapse that distance by interpreting a situation, selecting a tool, and changing process state in one loop. Governance can no longer be treated as a review added after intelligence. It is part of the mechanism that turns a generated possibility into an organizational action.

## 8 A Research Agenda for Context-Aware Agency

The five principles require conceptual refinement, technical realization, and empirical evaluation. They suggest a research program in which BPM, information-systems design, artificial intelligence, and socio-technical research contribute different forms of assurance.

### 8.1 Context Boundaries and Provenance

Research should compare methods for selecting context in processes where relevant signals are numerous, dynamic, and partly unstructured. Candidate approaches include designer-specified context models, retrieval learned from process traces, participant elicitation through conversation, and hybrids of symbolic and generative representations. Evaluation should measure not only task success but missed decisive signals, irrelevant or prohibited data use, information freshness, calibration of uncertainty, and sensitivity to source manipulation. A core question is when an agent can revise its own context boundary and when that boundary remains an organizational design decision.

### 8.2 Requisite Variety and Guardrails

Agentic systems create a design frontier between resilience and control. Too few actions reduce adaptation; too many permissions increase exposure. Controlled process simulations could vary tool access, plan-composition freedom, approval thresholds, and reversibility to examine where additional variety ceases to improve outcomes. Formal APM work on goals and strategy-level guardrails [4] provides one foundation. Organizational research is also needed because a technically valid boundary may transfer excessive monitoring, exception handling, or moral responsibility to human participants.

### 8.3 Activation Under Uncertainty and Time Pressure

Activation research should unite process-event semantics with calibrated beliefs, consequence, urgency, and reversibility. Useful experiments would compare rule-only, model-only, and hybrid decision mechanisms under changing context quality. Outcomes should include false activation, missed activation, response latency, quality of escalation, and recoverability. Explanations should be tested for whether participants can understand, contest, and act on them, not merely whether the system can generate a plausible account.

### 8.4 Governed Learning and Self-Modification

Research should develop a taxonomy of what agentic process systems change when they learn: case memory, contextual relevance, activation thresholds, plans, tools, permissions, or process structure. Each type needs an evidence threshold, evaluation method, approval path, monitoring period, and rollback mechanism proportionate to its scope. Longitudinal field studies are especially important. A modification that improves immediate task completion may create drift, inequity, fragility, or accumulated policy inconsistency only after many cases.

### 8.5 Socio-Technical Evaluation in Use

Benchmarks remain useful for isolating reasoning and interaction capabilities, and their limitations warn against equating task demonstrations with practical dependability [10]. BPM research should complement them with process-level and work-system-level evaluation. Relevant outcomes include service quality, resilience, compliance, explanation quality, human workload, distribution of discretion, ability to recover, and effects on stakeholders who do not directly interact with the agent. The empirical question is not simply whether an agent completes more cases. It is whether the changed configuration of people and machines achieves legitimate organizational goals more effectively and responsibly.

Together, these areas turn the proposed principles into falsifiable design questions. They also address an unfinished part of the original CAIS program. The thesis provided an analytical evaluation but called for concrete instantiations and empirical tests [11, pp. 269-273]. Agentic process systems now offer technically plausible instantiations, while their expanded action capacity raises the standard those tests must meet.

## 9 Conclusion: Context as a Way of Seeing

Agentic AI has not made context-awareness obsolete. It has moved context-driven adaptation closer to action. A language model's context window can carry observations and instructions, but context-awareness requires a governed relationship among environmental conditions, work-system goals, representations, authorized actions, and learning. That relationship belongs to the whole socio-technical system.

Revisiting the 2013 CAIS design theory produced five corresponding principles: frame the work system, maintain relevant context, bound the action repertoire, make activation traceable and capable of escalation, and govern what the system learns. The principles do not solve Agentic BPM, and they have not yet been empirically validated for that setting. Their value is to expose design questions that may otherwise be hidden by a model-centric account of agency.

In the conclusion to my thesis, I wrote that context-awareness remained in its infancy and that future research would extend the program [11, p. 273]. Agentic BPM does not fulfill that expectation automatically. It gives the expectation a more demanding object. In the work I was fortunate to undertake with Michael, a decisive move was to look beyond the process boundary for the conditions that made adaptation necessary [12-14]. His recent work on autonomization again invites BPM to enlarge its field of view [15].

That is a fitting lesson to carry forward in a volume honoring his contributions. What lies outside a process model can still determine whether the process achieves its purpose. Context is more than the contents of a window. It is a disciplined way of relating a system to its world, and designing that relationship responsibly is now central to the age of agents.

## Acknowledgments

[AUTHOR INPUT: Add a short acknowledgment to Michael Rosemann, the volume editors, and any readers who comment on the manuscript. Confirm whether Jan Recker should be acknowledged here in addition to the text.]

## Disclosure of Interests

[AUTHOR INPUT: Insert the disclosure required by the volume. Do not assume that there are no relevant interests without author confirmation.]

## Declaration on Generative-AI Assistance

[AUTHOR INPUT: Insert the exact disclosure required by Springer and the volume editors. The final statement should accurately describe research, drafting, editing, and verification assistance.]

## References

1. Ackoff, R.L.: Towards a system of systems concepts. Management Science 17(11), 661-671 (1971). https://doi.org/10.1287/mnsc.17.11.661

2. Alter, S.: Defining information systems as work systems: Implications for the IS field. European Journal of Information Systems 17, 448-469 (2008). https://doi.org/10.1057/ejis.2008.37

3. Calvanese, D., Casciani, A., De Giacomo, G., Dumas, M., Fournier, F., Kampik, T., La Malfa, E., Limonad, L., Marrella, A., Metzger, A., Montali, M., Amyot, D., Fettke, P., Polyvyanyy, A., Rinderle-Ma, S., Sardiña, S., Tax, N., Weber, B.: Agentic Business Process Management: A research manifesto. Information Systems 140, 102738 (2026). https://doi.org/10.1016/j.is.2026.102738

4. De Giacomo, G., Kampik, T., Kirchdorfer, L., Montali, M., Weinhuber, C.: Formal foundations of Agentic Business Process Management. arXiv:2604.17347 (2026). https://arxiv.org/abs/2604.17347

5. Dey, A.K.: Understanding and using context. Personal and Ubiquitous Computing 5, 4-7 (2001). https://doi.org/10.1007/s007790170019

6. Dourish, P.: What we talk about when we talk about context. Personal and Ubiquitous Computing 8, 19-30 (2004). https://doi.org/10.1007/s00779-003-0253-8

7. Dumas, M., Fournier, F., Limonad, L., Marrella, A., Montali, M., Rehse, J.-R., Accorsi, R., Calvanese, D., De Giacomo, G., Fahland, D., Gal, A., La Rosa, M., Völzer, H., Weber, I.: AI-augmented business process management systems: A research manifesto. ACM Transactions on Management Information Systems 14(1), Article 11, 1-19 (2023). https://doi.org/10.1145/3576047

8. Gregor, S., Jones, D.: The anatomy of a design theory. Journal of the Association for Information Systems 8(5), 312-335 (2007). https://doi.org/10.17705/1jais.00129

9. Kampik, T., Warmuth, C., Rebmann, A., Agam, R., Egger, L.N.P., Gerber, A., Hoffart, J., Kolk, J., Herzig, P., Decker, G., van der Aa, H., Polyvyanyy, A., Rinderle-Ma, S., Weber, I., Weidlich, M.: Large process models: A vision for business process management in the age of generative AI. KI - Künstliche Intelligenz 39, 81-95 (2025). https://doi.org/10.1007/s13218-024-00863-8

10. Liu, X., Yu, H., Zhang, H., et al.: AgentBench: Evaluating LLMs as agents. In: International Conference on Learning Representations (2024). https://arxiv.org/abs/2308.03688

11. Ploesser, K.: A Design Theory for Context-Aware Information Systems: Improving IS Design Science Outcomes Through Theory-Driven Design. Doctoral thesis, Queensland University of Technology, Brisbane (2013). https://eprints.qut.edu.au/60865/

12. Ploesser, K., Recker, J., Rosemann, M.: Challenges in the context-aware management of business processes: A multiple case study. In: Proceedings of the 19th European Conference on Information Systems, paper 6, pp. 51-62. Association for Information Systems (2011). https://aisel.aisnet.org/ecis2011/6/

13. Ploesser, K., Recker, J., Rosemann, M.: Supporting context-aware process design: Learnings from a design science study. In: zur Muehlen, M., Su, J. (eds.) Business Process Management Workshops. LNBIP, vol. 66, pp. 97-104. Springer, Heidelberg (2011). https://doi.org/10.1007/978-3-642-20511-8_9

14. Rosemann, M., Recker, J., Flender, C.: Contextualisation of business processes. International Journal of Business Process Integration and Management 3(1), 47-60 (2008). https://doi.org/10.1504/IJBPIM.2008.019347

15. Rosemann, M., vom Brocke, J., Van Looy, A., Santoro, F.: Business process management in the age of AI: Three essential drifts. Information Systems and e-Business Management 22, 415-429 (2024). https://doi.org/10.1007/s10257-024-00689-9

16. Shinn, N., Cassano, F., Gopinath, A., Narasimhan, K., Yao, S.: Reflexion: Language agents with verbal reinforcement learning. In: Advances in Neural Information Processing Systems, vol. 36 (2023). https://openreview.net/forum?id=vAElhFcKW6

17. Yao, S., Zhao, J., Yu, D., Du, N., Shafran, I., Narasimhan, K., Cao, Y.: ReAct: Synergizing reasoning and acting in language models. In: International Conference on Learning Representations (2023). https://openreview.net/forum?id=WE_vluYUL-X
