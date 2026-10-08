## Application in brief

Laser welding and related material-processing operations involve nonlinear, multi-phase dynamics: solid, liquid, gas, turbulence, and rapidly evolving melt-pool behaviour. Optical observations of the process may contain early signatures of instability and defects.

## Why it fits the project

- The underlying process can be nonlinear and dynamically complex, making it conceptually suitable for a nonlinear dynamical reservoir.
- A prototype could potentially access reflected laser light and other optical process signals.
- Reservoir tasks could include classification, anomaly detection, and short-horizon prediction from temporal optical signatures.
- The intended value is not generic simulation: it is fast process-state inference that can support quality monitoring and eventually control.

## Candidate tasks

- Detect unstable process regimes.
- Predict spatter / droplet formation, porosity, or gas-bubble-related defects.
- Classify weld quality or operating regime from reflected-light, emission, or spectral time series.
- Estimate a process state early enough to trigger corrective action.

## Bottlenecks and risks

- If no available optical signal contains predictive information about a meaningful defect or process instability, then the reservoir has no useful input and this application does not work.
- If the informative signal requires several sensors but their information cannot be combined within the available architecture, then a single-channel reservoir demonstration cannot solve the partner's actual monitoring problem.
- If labelled links between optical time series and weld-quality outcomes are unavailable, then prediction performance cannot be validated against a meaningful industrial target.
- If the combined observation, reservoir, readout, decision, and actuation delay exceeds the process-correction window, then the system cannot support control and can serve only as retrospective monitoring.
- If process dynamics relevant to the task do not fit the SBS temporal response in [[Technical_Specification]], then the present platform cannot capture the required behaviour.
- If apparent predictive accuracy is explained only by operating settings rather than early process signatures, then the model will fail when material, geometry, laser settings, or shielding conditions change.
- If safe optical access near high-power laser equipment or partner access to real data cannot be arranged, then the application remains an unvalidated hypothesis.

## Validation questions

- Which signal is already measured in a representative industrial or laboratory welding process?
- Which defect has a sufficiently frequent, well-labelled occurrence for a proof-of-concept dataset?
- What action would a partner take if the system detected risk early?
