# Working Guidance for the ERC PoC Proposal

This file defines how project materials are maintained. Follow it for all work in this directory.

## Working files

- `Grant_Structure.md` — the official Part B structure and preparation checklist.
- `Journal.md` — a concise log of substantive user requests, decisions, and completed work.
- `Project_Memory.md` — reusable project facts, working hypotheses, assumptions, and formulations.
- `Technical_Specification.md` — the current platform's technical reference, including fixed constraints, current configuration, and configurable parameters.
- `Proposal/` — working drafts of the Part B sections. Each proposal section is maintained as a separate English Markdown file and may include clearly labelled internal drafting notes that must be removed before submission.
  - The present drafting scope includes `1A.md`, `1B_i.md`, and `1B_ii.md`; do not draft `1B_iii` until the user explicitly requests it.
- `Tasks/` — benchmark and application-oriented TDRC tasks, their scientific purpose, experimental variants, compact outputs, and causal bottlenecks.

## Language rule

- Communicate with the user in Russian unless the user requests another language.
- Write and maintain all content saved in project files in English.
- Keep saved materials clear enough for the user to share directly with colleagues.
- Preserve exact technical terms, proper names, and quotations when translation would reduce precision.

## Technical dictation and numerical values

- When the user dictates compact numerical sequences in a technical context, normalise them to decimal values with explicit units when the surrounding context makes the intended decimal form clear.
  - Example: a dictated frequency sequence such as `973` may mean `9.73 GHz`, not nine hundred and seventy-three GHz.
- Preserve the normalised value consistently across project files.
- When the intended decimal placement is not unambiguous from context, ask rather than silently infer it.

## System-level terminology

- Do not describe the project's central systems challenge merely as optical-electrical conversion.
- The critical distinction is between:
  - **DAC before processing**, when originally digital data must be converted into an analogue optical representation solely to use the optical reservoir; and
  - **ADC after processing**, where the system should ideally emit a compact decision, control signal, or reduced feature representation rather than require full-rate digitisation of the original waveform.
- Prefer application cases with native analogue optical / RF inputs and compact outputs. A compact output may be a class label, detection flag, low-rate feature vector, or control signal.

## Journal maintenance

- After every substantive user request, add one timestamped, substantive entry to `Journal.md`.
  - Record the full local timestamp in Europe/Berlin time, including the UTC offset.
  - Explain the request, relevant context, and the decision or direction agreed.
  - Summarise the action taken, answer provided, and significant trade-offs.
  - List created or changed files and their purpose when useful.
  - Record new facts, assumptions, risks, and open questions when they materially affect the project.
- Write entries so that a colleague can understand what was discussed and decided without reading the full chat transcript.
- Do not invent historical timestamps. Older entries without one may retain their date-only label.
- Write new journal entries from the user's first-person perspective.
  - Use `User:` to describe what I asked, explained, decided, or requested.
  - Use `AI:` to describe what the AI analysed, created, changed, or recommended.
  - Use neutral factual wording only where neither role needs attribution.
- Do not use the journal as a full transcript or include internal reasoning and command output.
- Do not place confidential information in the journal unless the user explicitly directs this.

## Project memory maintenance

- Add reusable project-relevant statements supplied or confirmed by the user.
  - This includes statements about the technology, scientific basis, product, problem, target users, market, competitors, team, partners, intellectual property, work plan, or risks.
- For every entry, state the statement, its source, its status, and relevant proposal sections when known.
- Do not portray working hypotheses as established facts.
- When a statement changes, retain its history: mark the previous entry as superseded and add the current formulation.
- Do not add the agent's own inferences as user statements without explicit confirmation or a reliable source.

## Proposal workflow

- First map new material to `Grant_Structure.md`.
- Then use only relevant, current entries from `Project_Memory.md`.
- Explicitly identify gaps, unverified assumptions, and information that needs checking.

## Audience modes

- **Internal mode** is for the user and collaborators. It may be detailed, caveat-rich, technically specific, and use Obsidian wikilinks, open questions, and competing hypotheses.
- **External proposal mode** is for evaluators, funders, partners, and other external readers. It must be concise, confident, outcome-led, and written to secure support.
  - Lead with the opportunity, ambition, public / industrial value, and the concrete outcome to be delivered.
  - Present technical capabilities as enabling means, not as the central purpose of the work.
  - State risks only where the grant structure requires them; frame them as credible high-risk/high-gain validation questions.
  - Do not include internal wikilinks, drafting commentary, file references, or open-question lists in external text.
  - Avoid unnecessary technical detail and qualify claims only where accuracy requires it.
- Keep internal evidence, technical links, questions, and source-tracing in a separate accompanying note rather than inside an external proposal draft.

## Bottlenecks and risks

- In application, feature, and limitation notes, write bottlenecks as human-readable causal statements, not as unqualified research instructions.
- Prefer this structure: **if** a condition occurs or a limitation applies, **then** state the technical consequence and explain why it obstructs the intended goal.
- State the goal or required operating condition before describing a risk, so the reader understands what the risk threatens.
- Use an action item such as “measure”, “determine”, or “validate” only after the risk itself has been made explicit.

## Obsidian note conventions

- Notes intended for Obsidian must not start with a Markdown H1 that duplicates the filename, because Obsidian already displays the file title. Start substantive content at H2 level.
- Use Obsidian wikilinks whenever a note refers to information maintained elsewhere in the workspace.
  - Link technical values and setup details to `[[Technical_Specification]]` or an appropriate heading in that note.
  - Link project-level decisions and confirmed facts to `[[Project_Memory]]`.
  - Link related application, feature, and limitation notes using their workspace path where ambiguity is possible, for example `[[Features/Multichannel_Operation]]`.
- Do not duplicate technical values or detailed explanations when a stable source note already exists; use a concise summary and a wikilink instead.
