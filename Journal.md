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

## 2026-10-08 09:46:05 +02:00 — Zotero local-library access

- User: I asked how to make my local Zotero library available to the AI. I noted that most PDF attachments may not be stored locally, although the bibliographic records are present in Zotero.
- AI: I checked the Zotero integration status, enabled Zotero's local API preference, and created a backup of the previous preference file. The API has not started because Zotero was not restarted automatically; the user must fully quit and reopen Zotero. PDF attachments are not required for metadata search, citation lookup, or BibTeX export.

## 2026-10-07 16:41:34 +02:00 — Dedicated technical specification

- User: I asked for a dedicated file containing the technical specification of the experimental setup because the general project record was not sufficiently precise for technical reference. I provided the current SBS bandwidth, Brillouin frequency shift, fibre length, delay, configurable delay-loop options, and available AWG configurations.
- AI: I created `Technical_Specification.md` as the technical single source of truth. I separated physical constraints, current configuration, configurable parameters, AWG limitations, and missing information required for a complete specification. I also linked this file from `AGENTS.md` and `Project_Memory.md`.
## 2026-10-08 09:48:47 +02:00

User: I confirmed that Zotero had been closed after the earlier configuration step and that I had restarted it.

AI: I verified that the Zotero local API is now reachable and that the connector is running. The project can access the bibliographic metadata stored in the local Zotero library even when attachment PDFs are not stored locally. An initial inventory command exposed a Windows console-encoding issue only; rerunning it with UTF-8 output confirmed access to the library records. Future work can search the library by topic, author, title, or tag; selected references can be exported as BibTeX or used to support proposal drafting.

## 2026-10-10 11:11:37 +02:00 — Challenges folder and structural-maintenance rule

User: I asked to rename the `Limitations/` folder to `Challenges/`. I also requested a durable working rule: when I ask to rename or move project material, the change must be reflected everywhere it affects the workspace, including the project guidance.

AI: I renamed the folder to `Challenges/`, updated current documentation references in `README.md` and `Project_Memory.md`, and added a repository-wide structural-maintenance rule to `AGENTS.md`. Historical journal entries retain their original `Limitations/` wording because they record the name in use at the time.

## 2026-10-10 11:20:02 +02:00 — Git-aware structural changes

User: I clarified that this project is now tracked as a Git repository. I requested that any future file or folder removal or move be performed through Git so that the repository retains an accurate history. I said that I would correct the current rename manually.

AI: I added the Git-aware structural-change rule to `AGENTS.md`: use Git operations such as `git mv` and `git rm` for tracked renames, moves, and removals, while still updating all affected workspace references. I did not alter the current folder rename.

## 2026-10-10 11:44:12 +02:00 — Peer landscape for comparison and outreach

User: I asked for a new `Peers/` folder to track both organisations with which we might establish application-validation links and optical-neuromorphic / photonic-computing ventures against which we can compare ourselves. I named Lightmatter and Lightelligence as initial examples and described a Spanish programmable-photonics company with a reconfigurable hexagonal mesh. I asked for a serious broader search.

AI: I created `Peers/` and an internal landscape index. I identified the Spanish company as iPronics, a Universitat Politècnica de València spin-off with documented programmable hexagonal-mesh work. I added separate evidence-backed notes for Lightmatter, Lightelligence, iPronics, Q.ANT, Lumai, and Akhetonics, distinguishing their public product claims from the project's internal positioning assessment. I also added Laser Zentrum Hannover as a concrete prospective laser-process-monitoring validation contact, while making clear that no partnership or access is established. `AGENTS.md`, `README.md`, and `Project_Memory.md` now recognise this workspace category.

## 2026-10-10 12:40:23 +02:00 — Peer-note attribution and Zotero evidence test

User: I asked for peer notes to make the subject of each statement unambiguous: what an external organisation says or demonstrates must be clearly separated from what it means for us, how we compare ourselves, and what we should check. I also asked to add research publications where possible instead of relying only on companies' self-descriptions, and to test the Zotero integration by adding the sources to a new `Spinoff` collection.

AI: I added an explicit peer-note attribution rule to `AGENTS.md` and rewrote all current notes with reader-clear headings separating their public record, independent technical evidence, implications for our project, our positioning, outreach hypotheses, and our risks. I added a curated source file, `Peers/Peer_Research_References.bib`, containing four DOI-verified papers. Zotero imported all four entries into the selected `Spinoff` collection: Shen et al. (2017; Lightmatter scientific lineage), Hua et al. (2025; Lightelligence PACE system), On et al. (2024; iPronics hexagonal mesh), and Spall et al. (2020; Lumai scientific lineage). The notes explicitly state when a paper supports a precursor or application fit rather than independently validating a current commercial product.

## 2026-10-10 12:42:41 +02:00 — PDF attachments deferred

User: After confirming that the Zotero records had been imported, I initially asked for PDF attachments to be added as well, then decided to defer that work for now.

AI: I did not download or attach any PDFs. The four imported records retain their DOI metadata in the `Spinoff` collection, so open-access PDFs can be attached later to selected items without repeating the bibliographic search.

## 2026-10-10 12:47:28 +02:00 — Startup tags requested for Zotero references

User: I asked for the imported Zotero references to be tagged with the startup to which each publication relates.

AI: I mapped the intended tags as `Lightmatter`, `Lightelligence`, `iPronics`, and `Lumai` for the four imported records. The available local Zotero API and Connector can read records and create imports but cannot update tags on existing items, while the Zotero Desktop window is not exposed to the available UI-control surface. I did not create duplicate records with tags or modify Zotero's database directly. The tag update remains pending a writable Zotero UI or API route.

## 2026-10-10 12:49:45 +02:00 — Spin-off Zotero group library detected

User: I created a new Zotero group library for the spin-off and asked whether it was visible through the integration.

AI: I verified that the group library `Spin-off` is locally synchronised, visible as group library `L5` (group ID `6712327`), and marked editable. A separate collection named `Spin-off` still exists inside `My Library`; these are distinct Zotero targets and must not be confused when importing or organising references.

## 2026-10-10 12:52:20 +02:00 — Group-library tags verified

User: I removed the former personal-library collection, moved the references into the `Spin-off` group library, added startup tags, and asked whether the tags were visible.

AI: I verified four synchronised records in the editable `Spin-off` group library. Their tags are visible and correct: `Lightmatter` on Shen et al. (2017), `Lightelligence` on Hua et al. (2025), `iPronics` on On et al. (2024), and `Lumai` on Spall et al. (2020). The group-library item keys are distinct from the earlier personal-library imports, confirming that the current records belong to the shared library.

## 2026-10-10 13:09:06 +02:00 — Founder-led peer evidence and Keren Bergman identified

User: I asked for a second evidence pass on the companies already in `Peers/` for which no publication had previously been found: identify their co-founders and locate topic-relevant academic work, prioritising papers with a co-founder as last author. I also asked the AI to investigate Wolfram H. P. Pernice and any startups he is connected to. Finally, I described a US woman leading a lab in server optical interconnects and asked the AI to identify her; I subsequently confirmed that she is Keren Bergman.

AI: I corrected and extended the peer evidence. For Q.ANT, I identified founder Michael Förtsch and added his 2015 whispering-gallery-resonator publication as research-background evidence, explicitly not as validation of the current NPU. For Akhetonics, I identified co-founders Michael Kissner and Leonardo Del Bino and added their 2024 JLT architecture paper plus Del Bino's earlier optical-memory research; the note now distinguishes those scientific precursors from commercial-product evidence. I created a founder map for Wolfram Pernice and separate notes for Salience Labs, Pixel Photonics, and Xscape Photonics. The evidence confirms Pernice as co-founder of Salience and Pixel; Linq Photonics and coreX currently document advisory / mentor roles only, despite Linq's "3X serial founder" wording. I identified Keren Bergman as co-founder of Xscape Photonics and recorded an independent last-author Nature Photonics paper on a massively scalable Kerr-comb silicon-photonic link. I also added DOI-verified reference records to `Peers/Peer_Research_References.bib` without importing them into Zotero or attaching PDFs, because no new Zotero write request was made.

## 2026-10-10 13:24:45 +02:00 — Person-to-company relations and further founder search

User: I asked for the peer landscape to show explicit person-to-startup relationships whenever I name an individual. I requested Obsidian hashtags for Wolfram Pernice and Keren Bergman, asked to add Shanhui Fan, Marin Soljačić, and Dirk Englund to the Lightmatter and Lightelligence notes, and asked the AI to investigate Tobias Kippenberg's and Kerry Vahala's current startup activity.

AI: I added `#Wolfram_Pernice` to Pernice, Salience Labs, and Pixel Photonics, and `#Keren_Bergman` to Xscape Photonics. I added a named-people section to both Lightmatter and Lightelligence that distinguishes documented company roles from shared academic lineage and absence of evidence: Englund is Lightmatter's technical advisor; Soljačić is a Lightelligence co-founder; the 2017 foundational paper includes Englund and Soljačić; no formal role for Shanhui Fan at either company was established in the checked sources. I created a Kippenberg note recording co-founderships at LIGENTEC, DEEPLIGHT, LUXTELLIGENCE, and EDWATEC. I created a Vahala note recording his current high-Q resonator research and the negative finding that no current startup role was established in this evidence pass. The landscape index was updated accordingly.

## 2026-10-10 13:29:01 +02:00 — Peer graph refocused on companies

User: I clarified that `Peers/` must contain company notes, not standalone person notes. I explained that founder status is secondary: the relevant question is whether a company involving or emerging from a named researcher's laboratory does something useful in optics and computing. I asked for the previous additions to be reorganised on that basis and specifically asked to remove the separate Pernice card.

AI: I removed the standalone notes for Wolfram Pernice, Tobias Kippenberg, and Kerry Vahala using Git because they were not appropriate graph nodes. I retained the useful information by creating company-centred notes: Linq Photonics and coreX for the Pernice ecosystem, plus LIGENTEC, DEEPLIGHT, LUXTELLIGENCE, and EDWATEC for the Kippenberg ecosystem. Each note records the named research connection, the company’s optical role, its relevance to the SBS project, and causal risks. I did not create a Vahala company note because this search found no current startup relationship supported by sufficient evidence. The `Peers` index now links only company / organisation notes. I also updated `AGENTS.md` so that future peer-landscape work keeps researchers inside organisation notes unless the user explicitly requests a different graph structure.
