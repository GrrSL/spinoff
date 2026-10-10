## Snapshot

- **Organisation:** Q.ANT (Germany)
- **Role in this landscape:** European commercial comparator for a photonic processor delivered in conventional computing form factors.
- **Publicly stated product route:** Native Processing Unit (NPU) based on the LENA architecture, offered through PCIe-compatible and rack-mountable systems.
- **Evidence checked:** 2026-10-10.

## Their public record

Q.ANT announced its first commercial photonic NPU in late 2024 and described PCIe compatibility. Its 2025 announcement presents NPU 2 and a 19-inch server solution for AI and high-performance workloads, including native nonlinear processing claims. These are vendor statements and must be independently checked before being repeated as performance facts.

Sources: [company and founder profile](https://qant.com/about-us/), [first commercial NPU announcement](https://qant.com/press-releases/q-ant-launches-first-commercial-photonic-processor-for-energy-efficient-high-performance-computing-and-real-time-ai-applications/), [NPU 2 announcement](https://qant.com/press-releases/q-ant-unveils-its-second-generation-photonic-processor-to-power-the-next-wave-of-ai-and-hpc/).

## Independent technical evidence

Q.ANT identifies Dr Michael Förtsch as its founder and CEO. We found his earlier peer-reviewed work on narrow-band photon-pair generation in a crystalline whispering-gallery-mode resonator: Förtsch *et al.*, *Physical Review A* (2015), DOI [10.1103/PhysRevA.91.023812](https://doi.org/10.1103/PhysRevA.91.023812). Förtsch is the first author, not the senior last author.

This paper is evidence of the founder's research background in nonlinear and resonant photonics. It does **not** document the current LENA/NPU architecture, its claimed nonlinear-processing capabilities, or advertised system performance. No peer-reviewed paper independently validating the complete commercial platform was identified in this search; those specifications remain Q.ANT's own claims.

## What this means for our project

For our project, Q.ANT is particularly useful as a commercialisation comparator because it describes a progression from photonic processor to PCIe and 19-inch server products—the same broad form-factor ladder we are considering. The application and computational model differ: Q.ANT targets AI / HPC arithmetic, while our SBS TDRC aims to identify an application-specific analogue temporal-processing role.

## Our positioning relative to Q.ANT

We should borrow the deployment discipline (defined host interface, system form factor, and measurable workload) without adopting an unsupported claim of general-purpose photonic compute. Our first credible product may be a rack-mountable signal-processing instrument rather than a universal processor card.

## Our risks and checks

- If the PoC remains defined only by optical hardware novelty, it will be difficult to compare with product-oriented peers such as Q.ANT. A target workflow, input, compact output, and success metric are required.
- If a PCIe-card ambition requires conversion of native optical / RF signals into digitised host data before reservoir processing, the project may lose its central system advantage. The signal boundary must remain explicit.
