## Task in brief

Lorenz-63 is a canonical three-variable nonlinear dynamical system. It is defined by coupled variables \(x\), \(y\), and \(z\):

\[
\dot{x}=\sigma(y-x), \qquad
\dot{y}=x(\rho-z)-y, \qquad
\dot{z}=xy-\beta z.
\]

For commonly used parameter values, Lorenz-63 produces deterministic chaotic trajectories. Small differences in initial conditions lead to rapidly diverging trajectories even though the governing equations are deterministic. This makes it a demanding and widely used benchmark for temporal prediction and reservoir computing.

## Why it matters for this project

- The task tests nonlinear transformation and temporal memory in [[Features/SBS_Enhanced_OEO]].
- It can be run as one-step, multi-step-ahead, or autonomous prediction.
- It supports both single-variable and multivariate prediction experiments.
- It gives a controlled benchmark before the project moves to partner-specific application data.

## Experimental variants

| Variant | Input | Target | What it tests |
|---|---|---|---|
| Univariate one-step prediction | One observed Lorenz variable and recent history. | The next value of that variable. | Basic memory and nonlinear prediction. |
| Multi-step prediction | A current / past variable window. | Value several time steps ahead. | How prediction error grows with horizon. |
| Autonomous prediction | Initial observed trajectory, then previous prediction fed back as input. | Continued trajectory. | Whether the reservoir reproduces dynamics beyond teacher forcing. |
| Multivariate prediction | Two or three simultaneous Lorenz variables. | One target variable or the full state vector. | Whether joint variables improve state reconstruction and forecast accuracy. |
| Parallel-channel prediction | Separate or differently configured wavelength channels. | Two Lorenz components or two independent tasks. | [[Features/Multichannel_Operation]] and [[Features/Pump_Controlled_Nonlinearity]]. |

## Compact output

- Next-state scalar or a small state vector.
- Multi-step forecast trajectory.
- Error metric such as normalised root-mean-square error over a stated prediction horizon.

## Bottlenecks and risks

- If the virtual-node timing, delay, and nonlinear operating regime in [[Technical_Specification]] do not preserve enough relevant history, then the reservoir cannot reconstruct the Lorenz state and prediction will fail.
- If autonomous feedback causes errors to accumulate immediately, then the system may perform teacher-forced prediction but cannot demonstrate autonomous dynamical forecasting.
- If multivariate inputs cannot be encoded or combined without losing synchronisation between variables, then the multivariate variant cannot test the claimed benefit of joint observations.
- If the task is reported only for a favourable parameter setting or short horizon, then it does not demonstrate robust temporal-processing capability.

## Sources

- E. N. Lorenz, “Deterministic Nonperiodic Flow,” *Journal of the Atmospheric Sciences* (1963): [DOI](https://doi.org/10.1175/1520-0469(1963)020%3C0130:DNF%3E2.0.CO;2).
- Chaotic-series prediction studies commonly use Lorenz-63 together with Mackey–Glass as reservoir-computing benchmarks: [example study](https://doi.org/10.1016/j.mlwa.2022.100300).

