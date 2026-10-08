## Feature in brief

Changing pump power is expected to change the effective level of nonlinearity in an SBS-enhanced channel. Different channels may therefore be configured with different nonlinear operating regimes.

## Potential value

- Tune a channel for the nonlinear dynamics needed by a particular task.
- Run different task types in parallel with different nonlinearities.
- Process the same input through multiple nonlinear transformations, potentially enriching the combined representation.

## Bottlenecks and risks

- If changing pump power changes only gain, noise, or saturation rather than the useful nonlinear transformation, then pump power is not a control of computational nonlinearity and this feature does not exist.
- If bifurcation behaviour, hysteresis, or stability boundaries prevent repeatable operating points, then the nonlinearity cannot be selected reliably for a task.
- If changing one pump changes the operating point of another channel unpredictably, then independent multichannel configuration in [[Features/Multichannel_Operation]] is not possible.
- If no task-level metric or calibration maps pump setting to useful performance, then the feature cannot be used intentionally rather than by trial and error.
