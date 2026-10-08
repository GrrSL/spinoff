## Task in brief

Nonlinear Channel Equalisation (NCE) asks a processor to recover an original transmitted sequence after an optical-fibre channel has introduced nonlinear distortion and dispersion. It is the project's existing demonstrated task.

## Why it matters for this project

- NCE directly tests nonlinear temporal processing on a communications-relevant signal.
- It provides a known baseline while new SBS-specific capabilities are evaluated.
- It can be run in parallel with a prediction task to demonstrate [[Features/Multichannel_Operation]].

## Compact output

- Recovered symbol / bit estimate.
- Equalisation error or symbol-error metric.

## Bottlenecks and risks

- If the SBS reservoir does not improve or at least preserve equalisation performance while adding the intended new functionality, then the SBS enhancement has not produced a useful extension of the established OEO task.
- If input and output scaling, temporal alignment, or train/test protocol are not controlled, then apparent equalisation performance cannot be attributed reliably to the reservoir.
- If the channel model or experimental link does not represent the intended application regime, then the result remains a laboratory benchmark rather than evidence of an application pathway.

