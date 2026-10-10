## Snapshot

- **Organisation:** iPronics (Valencia, Spain)
- **Role in this landscape:** technical peer and possible future integration / ecosystem contact.
- **Origin:** founded in 2019 as a spin-off from Universitat Politècnica de València.
- **Relevant technology:** programmable silicon photonics; historical SmartLight research platform based on a hexagonal mesh of programmable Mach–Zehnder-interferometer cells; current public product focus on optical-circuit switching for AI infrastructure.
- **Evidence checked:** 2026-10-10.

## Their public record and identification

The user's description matches iPronics' programmable integrated-photonics work. A 2024 Nature Communications paper describes the iPronics SmartLight processor as a hexagonal mesh of 72 programmable unit cells, each based on a 2×2 Mach–Zehnder interferometer. The mesh can be configured into coupled-ring and other feedback topologies. iPronics' current commercial website presents the ONE platform as a programmable optical circuit switch for AI infrastructure.

Sources: [iPronics company page](https://ipronics.com/company/), [iPronics ONE product page](https://ipronics.com/product/), [programmable mesh demonstration](https://www.nature.com/articles/s41467-024-44939-3).

## Independent technical evidence

On *et al.* describe the iPronics SmartLight processor as a 72-cell hexagonal mesh of programmable Mach–Zehnder-interferometer unit cells and demonstrate reconfiguration into coupled-resonator topologies. This validates the research platform described here; it does **not** establish that iPronics' current ONE switching product is designed for SBS reservoir computing.

Source: [On et al., *Nature Communications* (2024)](https://doi.org/10.1038/s41467-024-44939-3). Imported into Zotero collection `Spinoff` as item `4BFJ4WBW`; source record: `Peers/Peer_Research_References.bib`.

## What this means for our project

For our project, this is the closest identified peer for the user's "hexagonal honeycomb" concept. They do not publicly present an SBS-enhanced fibre TDRC, but their work demonstrates how reconfigurable optical routing and feedback structures can become programmable hardware. It is relevant to our later integrated implementations, alternative optical-loop topologies, and prospective optical-system collaboration.

## Our outreach hypothesis

A technically focused conversation could explore whether programmable meshes are suitable for configurable feedback, coupling, or routing around a future integrated reservoir subsystem. This is exploratory; no shared product, compatibility, or partnership interest is established.

## Our risks and checks

- If the project requires SBS gain, a silicon-photonic mesh alone does not provide the present fibre-based SBS functionality. A future architecture would need a compatible nonlinear / acoustic element or retain an external SBS stage.
- If cumulative mesh loss and phase control prevent stable feedback at the required operating point, a resonator-like topology would not substitute directly for the current fibre loop. This must be assessed at a system level, not inferred from topology alone.
- iPronics' current commercial focus is optical switching. Any relevance to reservoir computing or a joint system is a research hypothesis, not a stated product direction.
