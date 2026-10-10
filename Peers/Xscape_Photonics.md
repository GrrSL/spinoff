## Snapshot

- **Obsidian tags:** #Keren_Bergman
- **Organisation:** Xscape Photonics (United States)
- **Role in this landscape:** strategic comparator for silicon-photonic interconnects at the GPU / memory boundary.
- **Founding connection:** Keren Bergman is a co-founder and board advisor; the company was spun out of Columbia silicon-photonics research.
- **Publicly stated direction:** multi-colour silicon-photonic links for AI-data-centre fabrics, specifically GPU-to-GPU and GPU-to-memory escape-bandwidth bottlenecks.
- **Evidence checked:** 2026-10-10.

## Their public record

Xscape states that its platform uses integrated multi-wavelength laser technology to relieve escape-bandwidth limitations in AI hardware. The company positions its optical fabric around GPU-to-GPU and GPU-to-memory connectivity, rather than optical computation itself. Its public material identifies Keren Bergman, Michal Lipson, Alexander Gaeta, Yoshitomo Okawachi, and Vivek Raghunathan as the founding team.

Sources: [Xscape company description](https://www.xscapephotonics.com/), [Xscape leadership and technology background](https://www.xscapephotonics.com/about-us), [Columbia account of the spin-out](https://www.ee.columbia.edu/news/xscape-photonics-secures-44-million-transform-ai-data-centers).

## Independent technical evidence

Rizzo *et al.*, ["Massively scalable Kerr comb-driven silicon photonic link"](https://doi.org/10.1038/s41566-023-01244-7), *Nature Photonics* (2023), reports a silicon-photonic data link based on a Kerr-comb source, WDM transmitter, and receiver; Keren Bergman is the last author. This is strong evidence for the Columbia research lineage and the microring / multi-colour interconnect direction. It is **not** independent proof of every current Xscape platform specification or commercial product claim.

## What this means for our project

Xscape is a useful counterpoint to optical neuromorphic computing: it pursues a clear data-movement bottleneck at high scale, while our reservoir must earn its place by transforming a dynamic analogue signal before a costly full-rate conversion. The common lesson is to identify precisely where optical hardware changes a system constraint.

## Our positioning relative to Xscape

We should not position an SBS reservoir as a replacement for GPU fabric. The meaningful comparison is architectural: Xscape moves large digital data efficiently; we seek to reduce or interpret native optical / RF data locally and emit a compact output. This comparison sharpens the distinction in [[Project_Memory]] between transport, DAC-before-processing, and ADC-after-processing.

## Our risks and checks

- If a proposed use case only moves standard digitised data between processors, then Xscape-style optical interconnects address a more direct bottleneck than a reservoir. The SBS proposition needs native analogue dynamics or a compact decision requirement.
- If we imply that a scientific comb-link demonstration validates current Xscape hardware, then we would conflate precursor research with the company's product. Public product specifications must remain attributed to Xscape.
