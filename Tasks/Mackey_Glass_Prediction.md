## Task in brief

Mackey–Glass is a delayed nonlinear dynamical system that produces complex and, for suitable parameters, chaotic time series. It is a standard benchmark for testing whether a reservoir can retain and transform delayed temporal information.

## Why it matters for this project

- The task directly probes the interaction of delay, memory, and nonlinearity in a time-delay reservoir.
- It complements [[Tasks/Lorenz_63_Prediction]]: Lorenz-63 is a coupled three-variable system, while Mackey–Glass is commonly studied as a delayed scalar series.
- It can be compared with the project's existing nonlinear channel-equalisation task in [[Tasks/Nonlinear_Channel_Equalisation]].

## Candidate experiments

- One-step prediction.
- Multi-step-ahead prediction.
- Autonomous prediction after an initial teacher-forced segment.
- Parallel execution with Lorenz-63 or NCE on separate channels.

## Bottlenecks and risks

- If the configured delay and node spacing in [[Technical_Specification]] do not retain the relevant temporal history, then the reservoir cannot approximate the delayed Mackey–Glass dynamics.
- If autonomous feedback becomes unstable, then the experiment can demonstrate only teacher-forced prediction rather than sustained generation.
- If the benchmark is evaluated with inconsistent train/test splits or unreported prediction horizons, then performance cannot be compared credibly with other reservoir implementations.

