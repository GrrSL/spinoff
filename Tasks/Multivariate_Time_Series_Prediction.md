## Task in brief

Multivariate time-series prediction uses several synchronised variables as input, rather than one scalar stream. The task is to predict one future variable, several future variables, a joint system state, or a compact control-relevant quantity from their shared temporal history.

## Why it matters for this project

- Real sensing and control systems often observe several coupled variables rather than one isolated signal.
- Multiple variables can contain complementary information about the underlying state, potentially improving prediction accuracy or forecast horizon.
- The task gives a principled reason to combine several channels, either as separate inputs or through [[Features/Multichannel_Operation]].
- It creates a bridge from standard chaotic benchmarks to application settings such as multi-sensor process monitoring, antenna arrays, and distributed fibre sensing.

## Candidate experiments

| Experiment | Inputs | Output | Purpose |
|---|---|---|---|
| Lorenz-63 state prediction | Two or three Lorenz variables. | One variable or the full next state. | Controlled test of whether joint variables improve forecasting. |
| Multiple delayed views | The same signal on several delays or nonlinear operating points. | Next value or task label. | Test complementary physical representations. |
| Parallel task streams | Different time series on different wavelength channels. | One output per stream. | Test throughput and independent operation. |
| Application data | Several synchronised sensor or antenna streams. | Forecast, event label, risk score, or control signal. | Connect the platform to a partner-relevant task. |

## Compact output

- Predicted scalar or state vector.
- Event class or risk score.
- One or several low-rate control signals.

## Bottlenecks and risks

- If variables are not synchronised in time, then their joint state is corrupted and multivariate prediction cannot exploit complementary information.
- If adding variables does not improve task accuracy, forecast horizon, robustness, or a partner-relevant metric, then multivariate operation adds complexity without computational value.
- If the number of input variables exceeds the available channel, timing, or readout capacity described in [[Technical_Specification]], then the experiment cannot scale beyond a small demonstration.
- If multichannel operation introduces uncontrolled crosstalk, then apparent multivariate performance cannot be attributed to deliberate joint processing. See [[Features/Multichannel_Operation]].

## Sources

- A comparative reservoir-computing study explicitly considers univariate and multivariate prediction and uses Lorenz-63 and Mackey–Glass benchmarks: [DOI](https://doi.org/10.1016/j.mlwa.2022.100300).

