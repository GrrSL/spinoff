## Application in brief

Analogue radio-over-fibre transports an analogue RF or intermediate-frequency (IF) waveform on an optical carrier between a remote radio element and a central unit. The architecture of interest is:

```text
Remote antennas → analogue RF / IF signals → optical-fibre transport → SBS reservoir → reduced electronic output / ADC
```

This is materially different from converting stored digital data into an optical signal just to use an optical processor. Here, the signal can already exist as an analogue optical waveform before the reservoir.

## Why it is a genuine fit

- Remote-antenna and centralised-processing architectures are real RoF use cases.
- Radar-over-fibre and coherent MIMO radar are particularly relevant: multiple remote transmit / receive elements can exchange RF signals with a common central unit over standard single-mode fibre.
- A reservoir could perform a defined temporal operation before full digitisation, such as event detection, interference classification, channel / scene-state classification, short-horizon prediction, or feature extraction.
- Multiple optical channels and pump-controlled nonlinearities could be relevant to multiple antenna elements, frequency sub-bands, or differently configured processing paths.

## Most plausible first technical wedge

**Centralised radar-over-fibre or phased-array processing of an analogue IF or selected sub-band.**

The remote front end performs the RF reception and any necessary frequency conversion. The analogue IF or sub-band is transported optically to the central unit. The SBS reservoir produces a lower-rate decision or feature representation before conventional electronic processing.

This wedge is more credible than claiming direct processing of every raw high-bandwidth RF waveform.

## What must be true for the value proposition to hold

- The relevant signal must remain analogue and optical until it reaches the reservoir.
- The reservoir must perform a useful operation before ADC.
- The reservoir output must reduce downstream electronic work: for example, a classification, detection flag, low-rate feature vector, or selected event window.
- The useful signal bandwidth and temporal dynamics must fit [[Technical_Specification]], or be made to fit through IF conversion or sub-band selection.

## Candidate pre-ADC tasks

| Task | Meaning | Typical input to the reservoir | Compact output | Problem addressed |
|---|---|---|---|---|
| Event detection | Decide whether a relevant temporal event has occurred. | A time window of analogue IF / sub-band waveform from one or more antenna paths. | Detection flag, confidence score, or event timestamp. | Avoid full-rate processing of long periods containing no relevant event. |
| Interference classification | Identify the presence or type of interference. | IF / sub-band waveform, potentially from multiple antenna elements. | Interference class, confidence score, or mitigation trigger. | Select a response before expensive downstream processing is applied. |
| Modulation / waveform recognition | Identify the type or regime of an incoming RF waveform. | A bounded time window of the analogue signal. | Class label or low-dimensional feature vector. | Support signal awareness, routing, or selection of a suitable downstream receiver mode. |
| Channel or scene-state classification | Infer a propagation, target, or operating state from temporal RF behaviour. | One or several synchronised IF / sub-band streams. | State label or state estimate. | Help a central radar / antenna system choose processing, tracking, or resource-allocation behaviour. |
| Short-horizon prediction | Predict a near-future signal-derived quantity from recent dynamics. | Recent temporal history of IF / sub-band features. | Predicted scalar, risk score, or control value. | Support anticipatory control, tracking, or adaptive configuration. |
| Beam / receiver quality control | Estimate whether a channel, beam, or antenna path needs adjustment. | Signal-quality features or temporal waveform from antenna elements. | Low-rate steering, gain, filter, or handover control signal. | Reduce the amount of continuous high-rate electronic monitoring required. |

These tasks are candidates, not commitments. Their suitability depends on the available signal representation, SBS-compatible bandwidth, and a partner-relevant use case.

## Bottlenecks and risks

- If the candidate RoF waveform has bandwidth or temporal dynamics substantially beyond the SBS response in [[Technical_Specification]], then the reservoir cannot directly process the full waveform as intended; the system would need an IF, sub-band, envelope, or a different physical mechanism.
- If the full analogue waveform is digitised after the reservoir with essentially unchanged sampling rate and bit depth, then the main ADC and data-movement burden remains; no credible system-level energy advantage has been demonstrated.
- If analogue-link noise, intermodulation distortion, phase noise, or limited dynamic range dominates the received waveform, then reservoir performance may be limited by the transport link rather than by the computational architecture.
- If multiple antenna channels are combined without stable timing and phase relationships, then spatial information can be lost and multi-antenna processing may become unreliable.
- If the initial use case is framed as generic 5G / 6G fronthaul, then mature digital fronthaul alternatives and stringent linearity / EVM requirements create a difficult competitive baseline.

## Validation plan

1. Choose one pre-ADC task with a low-rate or reduced-dimensional output: for example interference classification or radar event detection.
2. Define an input signal representation compatible with [[Technical_Specification]]: IF, sub-band, or envelope.
3. Define task-level success metrics, including task accuracy, latency, and the downstream sampling / processing requirement.
4. Identify a radar, phased-array, microwave-photonics, or RoF partner with an appropriate testbed.

## Evidence that the architecture exists

- A 2024 study reports a coherent MIMO radar-over-fibre network in which a common central unit exchanges RF signals over standard single-mode fibre with remote radar transmitters and receivers: [Adaptive Beamforming Applied to Coherent MIMO Radar-over-Fiber Systems](https://doi.org/10.1109/RADARCONF2458775.2024.10549749).
- A 2019 photonic MIMO-radar demonstrator describes remote antenna elements connected through optical fibre and reports 100 MHz signal bandwidth in an outdoor surveillance scenario: [Photonics for Coherent MIMO Radar: an Experimental Multi-Target Surveillance Scenario](https://doi.org/10.23919/IRS.2019.8768096).
- Analogue RoF has also been investigated for centralised 5G fronthaul, but research explicitly discusses the trade-off with digitised RoF and system scalability: [Towards a Scaleable 5G Fronthaul: Analog Radio-over-Fiber and Space Division Multiplexing](https://doi.org/10.1109/JLT.2020.3004416).
