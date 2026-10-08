# Technical Specification — SBS-Enhanced OEO Reservoir Platform

## Scope and status

- This file is the technical reference for the current experimental platform and its configurable design space.
- Values labelled **current configuration** describe the setup presently used.
- Values labelled **physical constraint** are determined by the current physical mechanism or component choice.
- Values labelled **configurable** may be changed through redesign, component replacement, or experimental configuration.
- Source for the initial entries: user, 2026-10-07.

## Physical mechanism

- Platform: SBS-enhanced optoelectronic oscillator (OEO) operated as a time-delay reservoir computer.
- Nonlinear medium: **HNLF (Highly Nonlinear Fiber)** with counter-propagating pump and seed.
- Required Brillouin frequency shift: **9.73 GHz**.
- Brillouin resonance bandwidth: approximately **45 MHz**.
- Associated transient-response time: approximately **22 ns**.

## Seed and pump generation

- A single laser output is split into seed and pump paths.
- Both paths use single-sideband modulators (SSMs), implemented with Mach–Zehnder-modulator technology.
- Pump generation:
  - The pump frequency shift can be generated from an external RF source.
  - Alternatively, an AWG can generate a sinusoidal waveform to drive the pump SSM.
- Seed generation:
  - The main signal path is termed the **seed**.
  - The seed is generated / shifted through its own SSM.
- Current multi-frequency design principle:
  - Create multiple seed carriers by shifting the seed path by different RF frequencies.
  - Create corresponding pumps so that each seed-pump pair satisfies the required **9.73 GHz** Brillouin frequency separation.
  - The modulation envelopes on distinct seed carriers can carry different tasks in parallel.
- Illustrative two-channel mapping cited by the user:
  - seed shifts: **−2 GHz** and **−3 GHz**;
  - corresponding pump shifts: **+7.73 GHz** and **+6.73 GHz**;
  - each seed-pump pair therefore maintains a **9.73 GHz** separation.
  - Status: confirmed by user.

## Modulators and electronic interfaces

- Single-sideband modulator lower frequency limit: approximately **1 GHz**.
- Single-sideband modulator upper frequency limit: component-dependent, currently approximately **12 GHz** or **18 GHz**.
- Current photodetector bandwidth: **5 GHz**.
- Current oscilloscope bandwidth: **4 GHz**.
- Electronic amplification is selected to match the available electronic input signal and required drive level; no fixed amplifier specification is currently treated as a platform constraint.
- Modulator bias point, drive-voltage range, and half-wave voltage are not currently considered primary design constraints because suitable amplification and RF driving can be selected for the experimental configuration.

## Filter response

- The SBS filtering response is Lorentzian.

## Current delay-line configuration

- Current fibre length: **20 m**.
- Current loop delay: approximately **380 ns**.
- In the current basic setup, the HNLF is sufficiently long to serve as the primary delay element; it is therefore not drawn as a separate delay-line block in `Setup basic.canvas`.
- An additional separate delay line may be inserted as an optional configuration element to increase or otherwise modify the total delay.
- Current signal path after modulation:
  1. circulator;
  2. nonlinear fibre;
  3. second circulator;
  4. optional delay line;
  5. photodetector.
- The circulators separate the seed / signal from the counter-propagating pump.

## Current basic setup topology

- The structured implementation diagram is maintained in `Setup basic.canvas`.
- Seed branch:
  1. laser;
  2. optical splitter;
  3. seed SSM;
  4. pre-amplifier EDFA;
  5. first circulator;
  6. HNLF;
  7. second circulator;
  8. photodetector.
- Pump branch:
  1. laser;
  2. same optical splitter;
  3. pump SSM driven by an RF source in the basic configuration;
  4. high-power EDFA;
  5. second circulator;
  6. HNLF in the counter-propagating direction;
  7. first circulator;
  8. beam dump for depleted pump.
- Electrical feedback and input branch:
  - AWG output and photodetector feedback are combined before driving the seed SSM.
  - The photodetector output is also routed to the oscilloscope through a splitter / combiner.
- The diagram does not explicitly show the optional additional delay line or a selectable electronic amplifier. This is consistent with the current basic setup because the HNLF itself provides the primary delay; the additional delay line is a configuration variant.

## Configurable optical and feedback parameters

- Fibre length can be increased or decreased.
- Loop delay can therefore be changed.
- Fibre gain can be changed by replacing the fibre.
- Multiple feedback loops with distinct delays can be added.
  - Purpose: create temporally shifted signal paths / multiple delay contributions.
- Pump wavelength / frequency configuration can be used to create multiple channels.
- Pump power is expected to provide a control parameter for effective channel nonlinearity.
- Virtual-node count, node spacing, mask duration, and benchmark signal scaling are adjustable experimental parameters.
  - The team is already measuring performance across different settings to determine how prediction / classification accuracy changes.

## Arbitrary waveform generators

- Available AWG option A:
  - nominal sampling rate: **64 GSa/s**;
  - number of channels: **4**.
- Available AWG option B:
  - nominal sampling rate: **12 GSa/s**;
  - number of channels: **2**.
- Operational note: using more AWG channels reduces the available sampling rate. The exact channel-to-sampling-rate trade-off is not yet recorded here.

## Technical implications to track

- The approximately 45 MHz SBS resonance bandwidth and approximately 30 ns transient response constrain candidate signal bandwidths and virtual-node timing.
- The 9.73 GHz Brillouin frequency shift constrains pump-signal frequency placement.
- Delay length and multi-loop architecture are design variables that may affect reservoir memory, virtual-node separation, and coupling structure.
- AWG channel count and sampling rate constrain multichannel experiments and input-mask implementation.

## Information still required

- Laser wavelengths, linewidths, output powers, and tuning ranges.
- Pump power range at the nonlinear fibre and available power-control resolution.
- Modulator type, bandwidth, transfer function, drive-voltage range, and bias-control method.
- Photodetector bandwidth, responsivity, saturation level, and noise characteristics.
- Electronic amplifier and filter bandwidths, gains, and transfer functions.
- Data-acquisition / oscilloscope specifications and readout bandwidth.
- Fibre type, loss, nonlinearity, SBS gain coefficient, and temperature-stabilisation arrangement.
- Exact AWG channel-to-sampling-rate operating modes.
- Current virtual-node count, node spacing, mask duration, and benchmark signal scaling for each recorded experiment.
