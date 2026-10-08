# Project Memory

## Purpose

- This file stores reusable user-supplied or user-confirmed project information.
- Status labels distinguish confirmed facts from working hypotheses and information requiring verification.

## Technology

### P-000 — Originating ERC research project

- Project: **SOUND-PC — Computing with Light and Sound**.
- Principal Investigator: **Birgit Stiller**.
- Host organisation: **Max Planck Society (Max-Planck-Gesellschaft zur Förderung der Wissenschaften e.V.)**.
- ERC panel: **PE7**.
- Award year: **2024**.
- Source: user, who retrieved the information from a public source, 2026-10-07.
- Status: recorded as the ERC-funded project from which the current PoC proposal is derived; grant number and official project webpage still need to be added.

### T-003 — Product and technology direction

- Statement: the intended start-up will develop optical neuromorphic computing technology.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Possible proposal use:
  - Sections 1a.i–1a.ii — problem, solution, value proposition, and innovation potential.

### T-004 — Reservoir-computing model

- Statement: the computing model is reservoir computing rather than a conventional layered neural network with trainable vector-matrix multiplications and nonlinearities at every layer.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Details:
  - The reservoir contains many nonlinear nodes with sparse, rather than necessarily all-to-all, connectivity.
  - A subset of reservoir-node states is sampled as the output representation.
  - Training is confined to a linear output classifier (readout).
- Possible proposal use:
  - Sections 1a.i, 1a.ii, and 1b.i.

### T-005 — Time-delay reservoir computer

- Statement: the reservoir is implemented as a time-delay reservoir computer (TDRC).
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Details:
  - Virtual neurons are time-multiplexed rather than spatially separated physical objects.
  - Their effective coupling arises through an inertial or transient process in the physical system.
  - Sparse connectivity and the absence of strictly separated layers give the system an internal state, i.e. memory across multiple processing steps.
- Possible proposal use:
  - Sections 1a.i, 1a.ii, and 1b.i–1b.ii.

### T-006 — Baseline optoelectronic oscillator implementation

- Statement: the baseline physical implementation is an optoelectronic oscillator (OEO) loop.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Architecture:
  - A modulator converts an electrical feedback voltage into optical intensity nonlinearly.
  - An optical delay line provides delay; it can be a fibre spool.
  - A photodetector, optional electronic amplifier, and electronic filter close the feedback loop.
  - The filter provides coupling between neighbouring virtual neurons.
- Possible proposal use:
  - Sections 1a.i and 1b.i–1b.ii.

### T-007 — Brillouin-enabled OEO innovation

- Statement: stimulated Brillouin scattering (SBS) is introduced using an additional nonlinear-fibre spool and a counter-propagating optical pump.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Mechanism and expected effect:
  - The pump transfers energy to the principal optical signal through a narrowband SBS process governed by a frequency-offset condition.
  - SBS combines the filtering and amplification functions that are otherwise separate principal components of the OEO implementation.
  - Filter position is controlled through the pump configuration.
  - A multiwavelength / multi-tone pump could create parallel wavelength channels in the same OEO system.
- Maturity: the basic SBS-enabled concept described here has been realised experimentally.
- Possible proposal use:
  - Sections 1a.i–1a.iii and 1b.i–1b.iii.

### T-008 — Fully optical feedback-loop ambition

- Statement: a development objective is to remove the electronic part of the loop and realise fully optical feedback, potentially using an optical-fibre resonator interacting with a pump.
- Source: user, 2026-10-07.
- Status: working development objective; feasibility requires validation.
- Motivation:
  - Optical-to-electrical and electrical-to-optical conversions consume energy.
  - Reducing or eliminating these conversions supports the low-energy value proposition of optical neuromorphic computing.
- Key technical uncertainties:
  - Whether the SBS process alone provides sufficient nonlinearity.
  - Whether pump depletion can provide usable nonlinearity at accessible operating conditions.
  - Whether interaction between parallel instances can be achieved in a fully optical configuration.
- Possible proposal use:
  - Sections 1a.iii, 1b.ii–1b.iii, and 1c.

### T-009 — Parallelism and coupling

- Statement: multiple wavelength channels / OEO instances are a potential route to parallel processing.
- Source: user, 2026-10-07.
- Status: confirmed as a development direction; the operational design requires validation.
- Details:
  - A two-wavelength pump could create two parallel channels.
  - In an OEO implementation with electronic detection and common modulation, channels are expected to interact through detection and modulator crosstalk.
  - Reproducing beneficial inter-channel coupling in a fully optical configuration is an open technical question.
- Possible proposal use:
  - Sections 1a.ii–1a.iii and 1b.ii.

### T-010 — Pump-programmed input mask

- Statement: standard TDRC virtual nodes are created by multiplying the input data by a discrete input mask. A potential SBS-enabled improvement is to encode this mask in the pump.
- Source: user, 2026-10-07.
- Status: working hypothesis requiring validation.
- Potential benefit:
  - Pump-programmed masking could reduce or avoid a separate input-mask stage.
  - It may enable optimisation of the mask as an alternative or complement to training the linear readout classifier.
- Possible proposal use:
  - Sections 1a.ii–1a.iii and 1b.ii–1b.iii.

## Demonstrated Results and Benchmarks

### R-001 — Nonlinear Channel Equalisation

- Statement: the system has been tested on the Nonlinear Channel Equalisation task.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Task description: a bit stream travelling through an optical-fibre data channel undergoes nonlinear distortion and dispersion; the computational task is to recover the original message.
- Possible proposal use:
  - Sections 1a.i–1a.ii — initial evidence of relevance to optical data processing.
  - Sections 1b.ii–1b.iii — baseline validation and benchmark plan.

### R-002 — SBS-enhanced OEO generation and nonlinearity

- Statement: the SBS-enhanced OEO has been operated as an oscillator / generator with two pumps, producing simultaneous generation at two frequencies.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Supporting evidence: experimental graphs are available.
- Statement: sufficient nonlinearity has been observed to produce a bifurcation and induce chaotic dynamics following a pulse-triggered process.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Relevance:
  - Chaotic dynamics can provide high-dimensional nonlinear projection, in which small input changes can produce large output changes.
  - This is relevant to distinguishing or classifying inputs and to benchmarks generated by chaotic systems.
- Possible proposal use:
  - Sections 1a.i–1a.iii and 1b.ii.

### R-003 — SBS bandwidth and response-time constraint

- Statement: in the fibre currently used, the Brillouin resonance bandwidth is approximately 45 MHz and the associated transient process is approximately 30 ns.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Implication: the SBS bandwidth / response time is a fixed physical constraint for the current platform. Delay and other design parameters may be adjusted, but this resonance property cannot be freely changed within the present fibre choice.
- Relevance:
  - It constrains the temporal bandwidth of candidate applications and benchmarks.
  - It is a critical parameter for assessing compatibility with fibre sensing, communications, and high-speed optical processing.

### R-003a — Technical specification reference

- Statement: the platform's detailed technical parameters are maintained in `Technical_Specification.md`.
- Source: user, 2026-10-07.
- Status: confirmed documentation decision.
- Current recorded additions: 9.73 GHz Brillouin frequency shift, 20 m current fibre length, approximately 380 ns current delay, configurable multi-loop delays, AWG configurations, seed/pump generation, and electronic-interface limits.

### T-011 — External-input conditioning and pump recuperation

- Statement: practical external deployment may require a module that derives a compatible SBS seed-pump pair from external optical input.
- Source: user, 2026-10-07.
- Status: working development direction; a key deployment concern.
- Statement: SBS pump operation currently requires on the order of 1 W, and pump recuperation through an optical pump loop is a desirable longer-term feature to reduce externally injected pump power.
- Source: user, 2026-10-07.
- Status: working development direction; resource- and stabilisation-dependent.
- Documentation: see `Limitations/Seed_Pump_Input_Conditioning.md` and `Features/Pump_Recuperation.md`.

### R-004 — Current signal path and optical access

- Statement: in the current setup, the signal path after the modulator is: circulator, nonlinear fibre, second circulator, optional delay line, then photodetector.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Detail: the circulators separate the seed / signal from the counter-propagating pump.
- Implication: the optical signal is physically accessible after modulation and before photodetection, including around the nonlinear-fibre stage.

### R-005 — Input-signal compatibility principle

- Statement: the system can in principle accept optical input signals, including signals that are not necessarily coherent.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Constraint: the principal input-side concern is not optical coherence; it is the energy and complexity penalty of converting originally digital data into a suitable analogue optical representation solely for reservoir processing.

### R-006 — Laser-process prototype data access

- Statement: for a laser-process-monitoring prototype, the team expects to be able to access any relevant available data streams, including reflected light.
- Source: user, 2026-10-07.
- Status: working expectation; requires confirmation with the prospective domain partner.

## Candidate Computational Tasks

### A-001 — Time-series prediction

- Statement: a priority class of TDRC tasks is time-series prediction, including Lorenz 63 and Mackey–Glass benchmarks.
- Source: user, 2026-10-07.
- Status: confirmed project direction.
- Planned task modes:
  - One-step prediction of a recurrently generated sequence, requiring the system to retain relevant past information.
  - Multi-step-ahead prediction, where the target is shifted several steps relative to the input.
  - Autonomous prediction, where each predicted output is fed back as the input for the next prediction step.
- Possible proposal use:
  - Sections 1a.i–1a.ii and 1b.ii–1b.iii.

### A-003 — Parallel dual-task demonstration

- Statement: the preferred demonstration is to solve two time-series tasks in parallel on two channels, for example Lorenz 63 and Mackey–Glass, or Nonlinear Channel Equalisation and Mackey–Glass.
- Source: user, 2026-10-07.
- Status: confirmed experimental direction.
- Selection principle: retain the two-task combination that gives the strongest experimental result.
- Possible proposal use:
  - Sections 1a.ii and 1b.ii–1b.iii.

### A-002 — Control-oriented use cases

- Statement: prediction capabilities may be relevant to control systems that continuously observe data and make successive decisions, for example autonomous stabilisation.
- Source: user, 2026-10-07.
- Status: working application direction.
- Illustrative example: flight stabilisation of a quadcopter.
- Possible proposal use:
  - Sections 1a.i–1a.ii — societal or industrial relevance.

## Commercialisation and Integration Direction

### C-001 — Application-discovery spin-off strategy

- Statement: the spin-off is intended to establish relationships with potential users and technology holders, propose the technology as an enhancement rather than a finished solution, and obtain real-world material on which to test the concept.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Rationale: a credible application cannot be selected solely from theoretical claims; it must be tested against an external partner's needs and data.
- Possible proposal use:
  - Sections 1a.ii, 1b.i–1b.ii, and 1c.

### C-002 — Optical-domain processing constraint

- Statement: the main practical constraint for optical neuromorphic computing is input-output conversion. If data originate electronically, electro-optical conversion before processing and optical-electrical conversion afterwards can negate expected energy advantages.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Implication: the most credible applications process information that is already optical, before its conversion into the electrical domain.
- Illustrative opportunity areas:
  - distributed fibre sensing for railway-condition monitoring, including stress and vibration sensing;
  - LiDAR signal processing in autonomous systems;
  - potentially other sensor-originated optical streams.
- Exclusions / limitations:
  - Directly attaching to and processing arbitrary internet-cable traffic is not currently feasible.
  - High-frequency trading is a speculative option with an unresolved data-embedding problem because the source data are digital.
- Possible proposal use:
  - Sections 1a.i–1a.ii — problem, customer context, and value proposition.

### C-003 — Integration flexibility

- Statement: the technology should be sufficiently flexible to integrate with a customer's existing optical setup, for example by processing LiDAR information optically before it is converted to electronics.
- Source: user, 2026-10-07.
- Status: confirmed design principle.
- Possible proposal use:
  - Sections 1a.i–1a.ii and 1b.i.

### C-004 — Customer status and candidate markets

- Statement: no specific customer has yet been identified.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- User-identified candidate areas:
  - high-frequency trading;
  - self-driving systems using LiDAR;
  - sensing systems using optical fibre.

### C-005 — Proposed market hypotheses for validation

- Source: agent-generated hypotheses, 2026-10-07.
- Status: requires user validation and external market discovery. These are not customer commitments or confirmed product-market-fit claims.
- Selection criterion: prioritise settings in which information already exists as an optical signal and a local, low-latency response has value.
- Ranked hypotheses:
  1. **Coherent optical communications and optical transceivers**
     - Why it fits: the demonstrated Nonlinear Channel Equalisation task is directly adjacent to receiver-side compensation of nonlinear distortion and dispersion.
     - Partner profile: optical-transceiver, coherent-DSP, and telecom-equipment companies; research groups running advanced optical links.
     - Caveat: a practical offering must show an advantage over mature electronic DSP and avoid creating additional conversion overhead.
  2. **Distributed fibre-optic sensing**
     - Why it fits: fibre-sensing systems generate high-volume time-series signals from an optical infrastructure; anomaly detection, prediction, classification, and event localisation may be relevant.
     - Example contexts: rail, pipelines, power cables, structural health, perimeter security, and geotechnical monitoring.
     - Partner profile: fibre-sensing instrument vendors, infrastructure operators, and system integrators.
     - Caveat: the exact point at which useful processing can remain optical must be established for each sensing modality.
  3. **FMCW LiDAR and other coherent optical ranging systems**
     - Why it fits: they produce optical or optoelectronic temporal signals and have a premium on latency, power, and compactness.
     - Partner profile: LiDAR developers, robotics / autonomous-systems companies, and industrial-automation suppliers.
     - Caveat: the technical use case must be specific, such as signal pre-processing, classification, tracking, or sensor-health monitoring.
  4. **Free-space optical communication links**
     - Why it fits: atmospheric channels introduce time-varying distortion; equalisation, classification, and prediction could be relevant before conventional downstream processing.
     - Partner profile: satellite-communication, defence-communications, and optical-terminal developers.
     - Caveat: this is likely a longer sales cycle and may involve restricted markets.
  5. **Industrial optical inspection and laser-process monitoring**
     - Why it fits: optical signals from laser manufacturing, spectroscopy, or high-speed inspection could benefit from immediate classification or prediction close to the sensor.
     - Partner profile: machine-vision, laser-manufacturing, spectroscopy, and industrial-automation suppliers.
     - Caveat: fit depends on whether the relevant optical waveform can be accessed before conversion and whether the task needs reservoir memory.
  6. **Radio-over-fibre and microwave-photonic signal processing**
     - Why it fits: the OEO / photonics architecture is naturally adjacent to high-bandwidth analogue signal processing and time-series classification.
     - Partner profile: mobile-network infrastructure, satellite communications, radar, and test-and-measurement companies.
     - Caveat: it may require electro-optical input encoding, so the energy proposition is weaker unless an optical signal is already present.

### C-006 — Deprioritised candidate: high-frequency trading

- Statement: high-frequency trading is a possible but currently speculative market direction because the source data are digital and the data-embedding problem is unresolved.
- Source: user, 2026-10-07.
- Status: working possibility; deprioritised until a credible optical-input and latency argument is defined.

### C-009 — Critical assessment of analogue radio-over-fibre

- Statement: analogue radio-over-fibre is a strong application hypothesis because it can carry an analogue RF waveform optically from remote antennas to a central processing unit before ADC.
- Source: user discussion and literature review, 2026-10-07.
- Status: promising but conditional; not yet a validated project-market fit.
- Strong-fit architecture: remote antenna / antenna-array elements create or carry analogue RF / intermediate-frequency signals, transport them optically to a central unit, and the SBS reservoir performs a defined pre-ADC operation that reduces the electronic processing burden.
- Global system-design principles confirmed by user:
  - The central conversion problem is not generic optical-electrical conversion. It is the need to perform DAC when originally digital data must be converted into an analogue optical waveform solely for reservoir processing.
  - A strong application has a native analogue optical / RF input and a compact output: a decision, feature, or control signal instead of a full-rate reconstruction of the original input.
- Critical conditions:
  - The reservoir must process a signal band compatible with its approximately 45 MHz SBS response, such as an IF, a selected sub-band, or a sufficiently slow envelope; it is not automatically suitable for raw wideband RF waveforms.
  - The output must be a lower-rate feature set, classification result, detection decision, or other reduced representation before ADC; digitising the full waveform unchanged after reservoir processing would not establish the claimed conversion or energy advantage.
  - External seed-pump conditioning is an acknowledged engineering limitation and is documented separately; it is not the main criterion for selecting the present application direction.
- Candidate first use case: centralised radar-over-fibre / phased-array processing of analogue IF or sub-band signals for event detection, interference classification, channel / scene-state classification, or short-horizon prediction.
- Documentation: see `Applications/Radio_over_Fibre.md`.

### C-007 — Laser-process monitoring and control

- Statement: laser welding and related laser material-processing systems are a high-priority application hypothesis.
- Source: user, 2026-10-07.
- Status: confirmed application direction; task definition requires discovery with domain experts.
- Rationale:
  - Laser welding involves interacting solid, liquid, and gaseous phases, as well as turbulent phenomena.
  - Process-quality problems can include droplet / spatter formation and gas-bubble formation.
  - Complex simulations are used to understand and manage these processes.
  - The nonlinear and potentially chaotic dynamics make this a conceptually promising context for a dynamical reservoir-computing system.
- Potential functions to validate with partners:
  - early detection of process instability or defect formation;
  - classification of process regimes;
  - prediction of adverse process events from optical emissions or reflected-light time series;
  - closed-loop process control, subject to latency and actuation constraints.
- Opportunity: relevant researchers in the Hannover area may be reachable through existing conference and local-network contacts.
- Possible proposal use:
  - Sections 1a.i–1a.ii, 1b.i–1b.ii, and 1c.

### C-008 — Additional optical-domain application hypotheses

- Source: agent-generated hypotheses, 2026-10-07.
- Status: requires user and partner validation.
- **Fast optical inspection and spectroscopy**
  - Potential role: classify spectra or time-dependent optical signatures, detect anomalies, or estimate a process state before high-volume data are passed to electronic processing.
  - Open question: identify a measurement modality where temporal memory and 45 MHz-scale SBS dynamics are useful.
- **Free-space optical communications**
  - Potential role: compensate or predict time-varying channel effects and classify channel conditions.
  - Open question: identify a partner-relevant scenario and determine whether the SBS temporal bandwidth matches its modulation and fading dynamics.
- **LiDAR and optical ranging**
  - Potential role: reduce electronic processing load by performing a defined pre-processing, classification, or event-detection operation on optical / optoelectronic temporal signals before the main electronic compute stage.
  - Clarification: the proposition is not simply faster LiDAR processing; it is lower energy and lower downstream compute burden for a narrowly defined task.
  - Open question: determine which optical signal can be intercepted and which computation can be performed before mandatory detection.

## Product and Integration Roadmap

### P-001 — Prototype trajectory

- Statement: the current platform is a laboratory setup. The preferred near-term product form is a rack-mountable prototype assembled from integrated, off-the-shelf components; the long-term aspiration is an optical accelerator comparable in deployment model to a GPU card.
- Source: user, 2026-10-07.
- Status: confirmed development direction.
- Scenarios:
  - Minimum outcome: laboratory demonstrator.
  - Preferred intermediate outcome: rack-mountable prototype.
  - Long-term outcome: compact optical accelerator card / module.

### P-002 — Required integration partnerships

- Statement: compact implementation will require collaboration with partners able to provide integrated optical components, such as tunable add-drop filters based on ring resonators for wavelength-channel separation.
- Source: user, 2026-10-07.
- Status: confirmed dependency.
- Implication: the proposal should frame system integration and partner engagement as a workstream rather than assume fully in-house implementation.

## Reachable Networks and Partner-Discovery Assets

### N-001 — Institutional network

- Statement: the project is connected to the Max Planck Institute for the Physics of Light and is in the process of moving part of the group to Hannover.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Statement: the project can access the PhoenixD Excellence Cluster network in Hannover.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Statement: the team has broad potential access to European academic research groups through the Max Planck and supervisory network.
- Source: user, 2026-10-07.
- Status: confirmed by user.

### N-002 — Additional relationship routes

- Statement: a contact in the Fraunhofer network may provide an industry-adjacent introduction route.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Statement: laser-cutting / laser-processing researchers who presented at a conference may be reachable.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Recommended outreach sequence:
  1. Re-contact laser-processing presenters to ask for a short technical discovery conversation, not a product pitch.
  2. Use PhoenixD and Max Planck contacts to locate expertise in integrated photonics, optical sensing, and photonic packaging.
  3. Ask the Fraunhofer contact for an introduction to the institute or group closest to laser-process monitoring, fibre sensing, or photonic integration.
  4. Convert the most engaged technical contact into a letter of support or intent for the proposal, if the relationship matures sufficiently.

## Grant Success Target

### G-001 — Qualitative technology milestones

- Statement: the current target for the grant is a multichannel SBS-enhanced OEO with a pump-programmed mask; fully optical loop closure will not be claimed as a grant objective at this stage.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Intended sequence of qualitative milestones:
  1. OEO implementation.
  2. SBS-enhanced OEO.
  3. Dual-channel SBS-enhanced OEO.
  4. Dual-channel SBS-enhanced OEO with a pump-programmed mask.
  5. Longer-term ambition: a fully optical closed loop.
- Evaluation principle: progress is currently framed as qualitative technological capability steps rather than fixed numerical performance targets.
- Note: numerical metrics should be identified and added later where they become technically meaningful, especially for commercial positioning.
- Possible proposal use:
  - Sections 1b.iii and 1c.

### G-002 — Grant duration and external-engagement target

- Statement: the grant duration is 18 months.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Realistic external-engagement target: obtain access to relevant real-world data and understand how the data are currently processed.
- Desirable additional outcomes: application requirements and, if the relationship matures, a letter of support.
- Not assumed within the grant: a full joint experimental campaign with an external partner.

### G-003 — Proposal narrative principle

- Statement: the proposal should present a broad, high-ambition vision for optical computing while committing to concrete, credible technical deliverables.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Implementation: use the multichannel SBS-enhanced OEO with pump-programmed mask as the concrete delivery focus, while positioning it as a platform for optical neuromorphic processing across relevant applications.

## Open Questions Backlog

- Q-001: Which concrete application(s), benchmark task(s), and end users will be prioritised for the proof of concept?
- Q-002: What experimental evidence and quantitative performance results already exist for the SBS-enabled OEO implementation?
- Q-003: Which real optical-data partner or user category should be approached first for the proof of concept?
- Q-004: Which numerical measurements can be reported credibly at each qualitative milestone, even if they are not fixed success thresholds?
- Q-005: What currently known solution can provide sufficient nonlinearity if SBS alone is inadequate, and when should it be disclosed in the proposal?
- Q-006: How will the input be encoded, the output read out, and the proposed system be trained in the fully optical configuration?
- Q-007: What is the evidence that inter-channel coupling is beneficial for the target tasks, and how will controllable coupling be measured?
- Q-008: Does the pump-programmed-mask hypothesis preserve the required temporal resolution and controllability of the mask?
- Q-009: What IPR, prior publications, existing prototypes, facilities, collaborators, or letters of support are available?
- Q-010: What is the intended commercialisation pathway: spin-out formation, licensing, or another route?
- Q-011: In the current laboratory setup, at what point can the optical signal be accessed before photodetection, and what signals can be injected without adding a separate high-power / high-speed modulator chain?
- Answer recorded: see R-004. The remaining question is which practical external optical sources can be coupled into that path with acceptable power, wavelength, modulation format, and synchronisation requirements.
- Q-012: Which candidate task is closest to the dynamics already demonstrated: equalisation, prediction, classification, anomaly detection, or another temporal task?
- Q-013: Is a fibre-sensing application technically compatible with the current SBS-enhanced OEO bandwidth, wavelength range, and optical-power regime?
- Q-014: What form factor is envisioned for a first prototype: a laboratory system, fibre-spool module, rack-mounted instrument, photonic integrated circuit, or a hybrid route?
- Q-015: Which types of organisations can the team realistically approach during the grant for data, application requirements, or a letter of support?
- Answer recorded: see N-001 and N-002. The next step is to identify named contacts and choose a first outreach target.

### T-000 — Project-level technical description

- Statement: the broader project uses an **optoelectronic oscillator** as a **time-delay reservoir computer** and employs **stimulated Brillouin scattering**.
- Source: user, 2026-10-07.
- Status: confirmed by user.
- Scope: this is a project-level formulation. It may be reused for the ERC PoC proposal and later related work, including the dissertation, subject to context-specific refinement.
- Possible proposal use:
  - Section 1a.i — the problem, solution, and origin of the idea.
  - Section 1a.ii — breakthrough innovation potential and differentiation.
  - Sections 1b.i–1b.ii — approach, methodology, validation, and technical risks.

### T-001 — Time-delay reservoir computer

- Statement: the system to be developed / future start-up spin-off is a time-delay reservoir computer.
- Source: user, 2026-10-07; initially provided as an example of the statements to preserve.
- Status: superseded by and consolidated into T-000.

### T-002 — Stimulated Brillouin scattering

- Statement: the system is expected to use stimulated Brillouin scattering.
- Source: user, 2026-10-07; initially provided as an example of the statements to preserve.
- Status: superseded by and consolidated into T-000; the exact technical role still needs to be specified.
