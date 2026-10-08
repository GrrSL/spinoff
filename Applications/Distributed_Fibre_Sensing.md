## Application in brief

Distributed fibre-optic sensing turns optical-fibre backscatter into spatially and temporally resolved information about strain, vibration, temperature, or disturbance along an asset.

## Why it fits the project

- The measurement infrastructure is intrinsically optical and generates time-series data.
- Brillouin terminology and physics are familiar to the prospective sensing community.
- Candidate applications include rail monitoring, pipelines, power cables, structural health, perimeter security, and geotechnical monitoring.
- Potential reservoir functions include event classification, anomaly detection, temporal prediction, and local pre-processing.

## Bottlenecks and risks

- If the selected sensing modality has no optical integration point before its mandatory detector or interrogator electronics, then it does not provide the native analogue optical input required by the system-level principle in [[Project_Memory#C-009 — Critical assessment of analogue radio-over-fibre]].
- If the sensing wavelength, pulse format, optical-power regime, or required temporal bandwidth is incompatible with the SBS platform described in [[Technical_Specification]], then the present reservoir cannot be inserted without changing the physical platform.
- If SBS processing perturbs the sensing pulse, backscatter interpretation, or spatial resolution, then it damages the measurement system it is supposed to augment and the application is not viable.
- If reservoir memory does not improve a specific event-detection, classification, or prediction task over a static method, then distributed sensing does not need a TDRC.
- If labelled fault events and acceptable false-alarm targets are unavailable, then no credible demonstration of operational value can be made.
- If environmental drift and changing fibre conditions cause unstable output that cannot be calibrated, then the system cannot meet infrastructure-monitoring reliability requirements.
