# ERC PoC Proposal Journal

## Journal convention

- New entries use the local Europe/Berlin timestamp, including UTC offset.
- Earlier entries retain date-only labels because exact historical message times were not recorded.
- The journal is a concise project record, not a complete conversation transcript.

## 2026-10-07 — Proposal-template analysis

- Request and context: the user asked for an analysis of the grant-template file in the project directory and wanted the requirements represented as an actionable nested Markdown outline.
- Decision: use the template as the authoritative source for a working preparation checklist rather than begin drafting narrative text immediately.
- Work completed: created `Grant_Structure.md`.
- Contents recorded: formatting requirements; 10-page overall limit; abstract requirements; Sections 1a, 1b, and 1c; Gantt / milestones, resources, team, risk mitigation, and possible supporting annexes.
- Relevance: `Grant_Structure.md` is the reference document against which future proposal content will be mapped.

## 2026-10-07 — Project working-memory system

- Request and context: the user requested durable project files for operating guidance, a log of the discussion, and reusable project assertions that could support both the grant and later dissertation work.
- Decision: maintain three linked files: `AGENTS.md` for operating guidance, `Journal.md` for the project record, and `Project_Memory.md` for reusable facts, hypotheses, and formulations.
- Work completed: created the initial files and established rules for recording source, status, and proposal relevance of technical statements.
- Relevance: this prevents confirmed information, working assumptions, and agent suggestions from being mixed together as the proposal evolves.

## 2026-10-07 — Filename and technical-baseline clarification

- Request and context: the user asked for short English filenames and clarified that the broader effort extends beyond the immediate grant towards related dissertation work.
- Decision: adopt `AGENTS.md`, `Journal.md`, `Project_Memory.md`, and `Grant_Structure.md` as the core project-file names.
- Technical baseline recorded: the broader project uses an optoelectronic oscillator as a time-delay reservoir computer and employs stimulated Brillouin scattering (SBS).
- Work completed: migrated the filenames and consolidated the previously separate technical notes into a single confirmed project-level statement in `Project_Memory.md`.

## 2026-10-07 — Language policy for saved materials

- Request and context: the user clarified that conversation should remain in Russian, while all saved project files must be in English so the user can share them directly with colleagues.
- Decision: English is mandatory for all persistent project materials; Russian remains the default language for dialogue with the user.
- Work completed: translated the existing Markdown files, added the language rule to `AGENTS.md`, and checked that Markdown files contained no Cyrillic text.
- Relevance: English files can now serve as common documentation for academic and industrial collaborators.

## 2026-10-07 — Initial technical vision and risks

- Request and context: the user described the technical vision for an optical neuromorphic-computing start-up based on time-delay reservoir computing (TDRC), OEO feedback, sparse reservoir connectivity, SBS, multichannel operation, and a possible future fully optical loop.
- Decision: separate confirmed architecture from experimental ambitions and unresolved physical questions.
- Technical content recorded:
  - reservoir computing uses nonlinear, sparsely connected nodes with a linear trained readout rather than a conventional fully trained layered neural network;
  - virtual nodes are time-multiplexed in a TDRC and rely on system dynamics for memory;
  - the OEO loop provides modulation, delay, detection, optional amplification, and filtering;
  - SBS is introduced through a counter-propagating pump in nonlinear fibre and can support filtering, gain, and multichannel operation;
  - fully optical loop closure and pump-programmed masking are longer-term / validation-dependent directions.
- Work completed: created structured technical entries and an open-question backlog in `Project_Memory.md`.

## 2026-10-07 — Tasks, commercialisation logic, and target outcome

- Request and context: the user explained that Nonlinear Channel Equalisation (NCE) is the existing test task and identified time-series prediction, including Lorenz 63 and Mackey–Glass, as additional TDRC tasks. The user also clarified that a specific customer is not yet known.
- Decision: position the spin-off as a route to application discovery and external partner engagement, rather than claim a finished product-market fit.
- Technical and commercial content recorded:
  - NCE is a demonstrated baseline task;
  - one-step, multi-step, and autonomous prediction are relevant benchmark modes;
  - processing is most compelling when information already exists in the optical domain, avoiding inefficient conversions of originally digital data;
  - relevant application spaces include fibre sensing, LiDAR / ranging, and other optical sensor systems.
- Grant direction agreed: the concrete target is a multichannel SBS-enhanced OEO with a pump-programmed mask. Fully optical loop closure remains a longer-term ambition and is not a committed grant deliverable.

## 2026-10-07 — Demonstrated results, physical constraints, and partner routes

- Request and context: the user supplied further experimental and strategic detail, including two-frequency generation with two SBS pumps, observed bifurcation / chaos, a preferred two-channel benchmark demonstration, the current signal path, and available institutional networks.
- Technical facts recorded:
  - the current fibre has an approximately 45 MHz Brillouin resonance bandwidth and an approximately 30 ns transient response;
  - the post-modulator signal path is circulator → nonlinear fibre → second circulator → optional delay line → photodetector;
  - the system can in principle accept optical inputs, including non-coherent signals; the key concern is costly conversion of originally digital data into an analogue optical representation;
  - the preferred demonstration may run two tasks in parallel, such as NCE plus Mackey–Glass or two chaotic-prediction tasks.
- Network and product direction recorded: potential access includes the Max Planck Institute for the Physics of Light, PhoenixD, European academic groups, a Fraunhofer-network route, and laser-processing conference contacts. The physical development path is laboratory setup → preferred rack-mountable prototype → longer-term compact accelerator/module.

## 2026-10-07 — Application and feature note system

- Request and context: the user asked for separate, Obsidian-friendly notes for each potential application and conceptual technological feature, with explicit bottlenecks. The user corrected an earlier framing of radio-over-fibre: analogue RoF is a strong fit when an RF waveform is already transported optically.
- Decision: create `Applications/` and `Features/` directories, with one English Markdown note per application or capability.
- Work completed:
  - application notes created for RoF, laser-process monitoring, distributed fibre sensing, LiDAR / ranging, free-space optical communications, optical communications, and inspection / spectroscopy;
  - feature notes created for the SBS-enhanced OEO, pump-programmed input mask, multichannel operation, pump-controlled nonlinearity, and fully optical loop closure;
  - every note includes a short description, project fit, bottlenecks, and validation questions where relevant.
- Grant engagement decision: within an 18-month grant, access to real data and an understanding of the partner's processing pipeline are realistic core outcomes; application requirements and a letter of support are desirable; a full joint experiment is not assumed.

## 2026-10-07 16:36:15 +02:00 — Journal redesign and timestamp policy

- Request and context: the user requested a more detailed journal, with entries that make the substance of the discussion understandable, and requested temporal markers rather than date-only headings.
- Decision: expand the journal into a substantive project log; apply full Europe/Berlin timestamps only to new entries rather than fabricate timestamps for earlier conversation.
- Work completed: expanded earlier entries from the available record and updated `AGENTS.md` with the new journal-maintenance standard.

## 2026-10-07 16:39:19 +02:00 — Journal voice and attribution

- User: I requested that journal entries be written from my first-person perspective, with explicit attribution of my requests and the AI's actions.
- AI: I updated `AGENTS.md` to require `User:` and `AI:` labels in new journal entries. The user-facing narrative will use first person for the user's statements and requests.

## 2026-10-07 16:48:57 +02:00 — Seed/pump architecture and deployment features

- User: I described how the common laser output is split and used to generate seed and pump paths through single-sideband modulators. I specified the 9.73 GHz Brillouin separation, the multi-channel seed / pump frequency plan, SSM frequency limits, the current 5 GHz photodetector and 4 GHz oscilloscope, and the Lorentzian SBS filter response. I also identified two deployment concerns: conditioning external optical input into a compatible seed-pump pair and recovering / recirculating the approximately 1 W optical pump.
- AI: I updated `Technical_Specification.md` with the seed/pump scheme, multi-frequency example, interface limits, adjustable reservoir parameters, and Lorentzian filter response. I created `Features/External_Input_Seed_Pump_Conditioning.md` and `Features/Pump_Recuperation.md`, each with purpose and bottlenecks. I also added a technical-dictation rule to `AGENTS.md` so compact spoken numerical sequences are normalised to their contextual decimal values and units.

## 2026-10-07 16:56:21 +02:00 — Risk-note format and diagram representation

- User: I confirmed the two-channel frequency mapping. I clarified that external seed/pump conditioning is an integration limitation, not a product feature. I also requested that bottlenecks be written as understandable causal risks rather than vague instructions, and asked for a structured way to share and interpret setup flowcharts without relying on raster-image analysis.
- AI: I moved the external-input note to `Limitations/Seed_Pump_Input_Conditioning.md`, updated the documentation link, recorded confirmation of the frequency mapping, and added a causal risk-writing standard to `AGENTS.md`.

## 2026-10-07 17:04:32 +02:00 — Critical reassessment of analogue radio-over-fibre

- User: I asked for a critical analysis of whether analogue radio-over-fibre is genuinely the right application. I described the intended architecture: multiple antennas convert analogue received signals to light, transport them to a central module, the SBS reservoir performs useful processing before digitisation, and only then does electronic processing continue.
- AI: I checked the architecture against research on analogue RoF, centralised radio access, and radar-over-fibre. The result is a conditional fit: the architecture exists and is especially plausible for centralised radar / phased-array systems, but the 45 MHz SBS bandwidth, seed-pump compatibility, analogue-link dynamic range, and the requirement to reduce the amount of post-reservoir digitisation are decisive constraints. I updated `Project_Memory.md` and rewrote the RoF application note accordingly.

## 2026-10-07 17:17:08 +02:00 — ADC/DAC terminology, RoF task map, and Canvas review

- User: I clarified that the global systems issue is not generic optical-electrical conversion. The key problem is DAC when originally digital data must be converted into an analogue optical signal solely to use the reservoir. I confirmed that a compact output may be a decision, a low-dimensional feature, or a single control signal. I asked for the proposed RoF tasks to be documented and requested a consistency check of `Setup basic.canvas`.
- AI: I recorded the DAC-versus-ADC terminology and compact-output principle in `AGENTS.md` and `Project_Memory.md`. I added a task table to `Applications/Radio_over_Fibre.md`, removed repeated seed/pump-integration emphasis and the distracting simple-filter comparison from that application note, and read `Setup basic.canvas` as a structured graph. Its physical paths match the described basic setup; `Technical_Specification.md` now records the topology and notes that an optional delay line and optional electronic amplifier are not shown in the current Canvas.

## 2026-10-07 17:19:07 +02:00 — HNLF as the primary delay element

- User: I clarified that `HNLF` means Highly Nonlinear Fiber. In the current basic configuration, the HNLF itself is long enough to provide the delay, so it was not shown as a separate delay-line block in the Canvas. An additional delay line can be inserted as an optional configuration element.
- AI: I updated `Technical_Specification.md` to expand the HNLF acronym, state its role as the primary delay element, and distinguish the optional additional delay line from the basic setup shown in `Setup basic.canvas`.

## 2026-10-07 17:28:14 +02:00 — Obsidian linking and causal risk review

- User: I asked for every `Bottlenecks and risks` section in `Applications/` and `Features/` to be rewritten as genuine causal risks: if a condition fails, the application or feature must fail or lose its purpose. I also asked that notes use Obsidian wikilinks to existing source notes rather than repeat technical details, and noted the duplicate-title issue caused by Obsidian's inline file-title display.
- AI: I removed duplicated H1 titles from all application and feature notes, rewrote every risk list into explicit if–then consequences, added links to `[[Technical_Specification]]`, `[[Project_Memory]]`, and related feature notes, and removed the remaining simple-analogue-filter comparison from the RoF validation plan. I updated `AGENTS.md` with the permanent Obsidian-note and wikilink conventions.

## 2026-10-07 17:40:04 +02:00 — First proposal draft: Section 1a

- User: I asked to begin drafting the grant proposal section by section, with one file for each of Sections 1a, 1b and 1c. I requested an initial attempt at answering the questions in `Grant_Structure.md`, followed by critical review and targeted questions where the available information is insufficient.
- AI: I created `Proposal/1A.md` and drafted the three required parts of Section 1a: the problem, solution and ERC-project origin; breakthrough innovation potential; and the high-risk/high-gain case. The file includes a separate internal drafting-notes section with workspace links and five targeted questions that must be answered before the section can become submission-ready. I added the `Proposal/` folder convention to `AGENTS.md`.

## 2026-10-07 17:41:42 +02:00 — Originating ERC project identified

- User: I provided publicly sourced identification of the ERC project underlying this PoC application: SOUND-PC — Computing with Light and Sound, led by Birgit Stiller at the Max Planck Society, awarded in 2024 under panel PE7.
- AI: I recorded the project in `Project_Memory.md` and replaced the originating-project placeholder in `Proposal/1A.md`. The grant number, official project webpage, and final one-sentence description of SOUND-PC's scientific objective remain to be confirmed.

## 2026-10-07 17:48:29 +02:00 — Task portfolio and broad partner-discovery strategy

- User: I clarified that pump-programmed masking is exploratory. I decided not to preselect one or two applications because the PoC must search broadly for industrial partners and application requirements. I also requested a separate task layer for TDRC benchmarks, including Lorenz-63 and multivariate time-series prediction, and explained that multivariate inputs can improve prediction or enable more complex forecasting.
- AI: I created `Tasks/` with notes for Lorenz-63 prediction, Mackey–Glass prediction, Nonlinear Channel Equalisation, and multivariate time-series prediction, plus a linked task portfolio index. I updated `Proposal/1A.md` to frame pump-programmed masking as exploratory, explain broad application and partner discovery, and position the SBS contribution as new controllable degrees of freedom added to already established OEO/TDRC task capability. I added the `Tasks/` convention to `AGENTS.md`.

## 2026-10-07 18:06:08 +02:00 — External proposal-audience rewrite

- User: I explained that the grant text must persuade an external funding audience rather than read like an internal discussion. I asked for a broader, more ambitious narrative around optical neuromorphic computing as an alternative computing paradigm, with specific PoC commitments kept credible and subordinate to that ambition. I also requested much shorter and clearer prose.
- AI: I created an explicit internal-versus-external audience rule in `AGENTS.md`. I rewrote `Proposal/1A.md` as a concise external-audience draft focused on the opportunity, the photonic-computing vision, direct optical processing, tangible outcomes, and partner discovery. I moved technical links, evidence tracing, and future additions into the separate internal file `Proposal/1A_Notes.md`.

## 2026-10-07 20:48:17 +02:00 — Initial drafts of Sections 1b.i and 1b.ii

- User: I asked to begin Section 1b and requested that the missing assessment of potential end users be drafted from the application directions already developed. I then clarified that only Sections 1b.i and 1b.ii should be drafted now; Section 1b.iii must wait.
- AI: I created external-audience drafts in `Proposal/1B_i.md` and `Proposal/1B_ii.md`. They present a spin-off-oriented innovation pathway, platform and task validation, multichannel/adaptive processing, broad partner discovery, an end-user assessment, and IP/exploitation activity. I created `Proposal/1B_Notes.md` for internal links and unresolved details, and added the scope limit excluding 1b.iii to `AGENTS.md`.

## 2026-10-07 21:03:47 +02:00 — LiDAR and autonomous systems added to end-user assessment

- User: I requested that LiDAR be added explicitly to the end-user assessment, with emphasis on self-driving vehicles and robotics as a visible example of reducing machine-vision and perception workload through optical processing.
- AI: I added a dedicated LiDAR, robotics and autonomous-vehicle row to the end-user table in `Proposal/1B_ii.md`. The existing application note `Applications/LiDAR_and_Optical_Ranging.md` remains the detailed internal reference.

## 2026-10-08 08:37:19 +02:00 — GitHub repository preparation

- User: I requested a README and a `.gitignore` file in preparation for turning the project folder into a GitHub repository. I specified that PDF files must not be uploaded.
- AI: I created `README.md` with a concise project overview and repository map, and added `.gitignore` with a repository-wide `*.pdf` exclusion. Markdown, Obsidian Canvas, and other working materials remain trackable.

## 2026-10-07 16:41:34 +02:00 — Dedicated technical specification

- User: I asked for a dedicated file containing the technical specification of the experimental setup because the general project record was not sufficiently precise for technical reference. I provided the current SBS bandwidth, Brillouin frequency shift, fibre length, delay, configurable delay-loop options, and available AWG configurations.
- AI: I created `Technical_Specification.md` as the technical single source of truth. I separated physical constraints, current configuration, configurable parameters, AWG limitations, and missing information required for a complete specification. I also linked this file from `AGENTS.md` and `Project_Memory.md`.
