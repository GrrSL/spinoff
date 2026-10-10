## Snapshot

- **Organisation:** Lumai (United Kingdom)
- **Role in this landscape:** strategic comparator for hybrid optical-digital AI-inference systems.
- **Publicly stated product:** Lumai Iris, a data-centre optical AI-inference server based on an optical matrix multiplier and a hybrid digital-optical architecture.
- **Evidence checked:** 2026-10-10.

## Their public record

Lumai presents Iris as an optical-computing system for real-time billion-parameter LLM inference, with a hybrid architecture in which optics addresses the compute bottleneck and digital electronics perform the remaining functions. Its website attributes performance and energy figures to the company and offers Iris Nova for data-centre evaluation.

Sources: [Lumai technology](https://lumai.ai/technology), [Lumai Iris product](https://lumai.ai/product), [April 2026 announcement](https://lumai.ai/resources/lumai-launches-the-worlds-first-optical-computing-system-for-real-time-billion-parameter-llm-inference).

## Independent technical evidence

Spall *et al.* demonstrate a fully reconfigurable coherent free-space optical vector--matrix multiplier. The authors include Lumai's co-founders, and the paper supports the scientific lineage of their optical-matrix-computing approach. It does **not** independently validate the current Lumai Iris server or the vendor's present performance figures.

Source: [Spall et al., *Optics Letters* (2020)](https://doi.org/10.1364/OL.401675). Imported into Zotero collection `Spinoff` as item `ZHEFLRHT`; source record: `Peers/Peer_Research_References.bib`.

## What this means for our project

For our project, Lumai is a strong counterexample to a simplistic "all-optical or nothing" story. It explicitly presents a hybrid architecture and focuses on a concrete workload boundary. We can use this as a commercial framing lesson: photonics should take the portion of the problem where it is advantageous, while electronics retain the rest.

Their hardware approach is otherwise distant from our SBS TDRC: Lumai focuses on large optical matrix multiplication for data-centre inference, not physical recurrent dynamics for sensor-adjacent temporal processing.

## Our risks and checks

- If the project cannot name a workload in which recurrence and native analogue inputs outperform or simplify a conventional pipeline, it risks being compared unfavourably with matrix-accelerator businesses.
- If conversion overhead dominates the proposed use case, the general lesson from hybrid systems is not that photonics has failed; it is that the processing boundary has been placed incorrectly. The project must validate that boundary with a partner's data flow.
