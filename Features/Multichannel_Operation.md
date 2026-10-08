## Feature in brief

Multiple pump wavelengths or tones can create multiple wavelength channels in the SBS-enhanced OEO. This enables parallel reservoir operation in a shared physical system.

## Potential value

- Run two temporal tasks in parallel, for example NCE and Mackey–Glass or two chaotic-prediction benchmarks.
- Increase processing throughput.
- Increase effective reservoir complexity.
- Process identical data on multiple channels under different operating conditions and combine the outputs.

## Bottlenecks and risks

- If wavelength placement, channel isolation, pump-power allocation, or frequency stability cannot be controlled, then nominally separate channels will drift or overlap and parallel operation will not be repeatable. See [[Technical_Specification#Seed and pump generation]].
- If crosstalk cannot be measured and controlled, then it is impossible to distinguish harmful channel contamination from useful engineered coupling; neither independent nor coupled operation can be claimed reliably.
- If every additional channel requires a separate laser, modulator, AWG, and electronic chain, then multichannel operation scales cost, power, and footprint nearly linearly and loses its system-level value. See [[Technical_Specification#Arbitrary waveform generators]].
- If simultaneous channels do not increase throughput, effective reservoir richness, or task performance relative to a single-channel baseline, then the feature does not justify its added complexity.
- If channel readout still requires full-rate digitisation of every channel, then the compact-output principle in [[Project_Memory#C-009 — Critical assessment of analogue radio-over-fibre]] is not met.
