## Feature in brief

Time-delay reservoir computers commonly create virtual nodes by multiplying the input with a discrete input mask. The proposed feature is to encode or control this mask through the SBS pump rather than through a separate conventional mask stage.

## Why the project can explore it

- SBS interaction is controlled by the pump configuration.
- The project uses SBS as an active functional element, not only as a passive fibre effect.
- Pump control may offer a route to influence the effective transformation applied to the input.

## Potential value

- Reduce or eliminate a separate input-mask operation.
- Provide a new degree of freedom for task-specific reservoir configuration.
- Explore mask optimisation as an alternative or complement to training the linear readout.

## Bottlenecks and risks

- If pump modulation does not produce a stable and sufficiently resolved effective input mask, then the intended replacement or enhancement of the conventional mask stage does not work.
- If the pump-controlled pattern cannot be synchronised with the virtual-node timing recorded in [[Technical_Specification]], then the mask is applied to the wrong temporal positions and reservoir operation is corrupted.
- If the observed change is only gain or filtering rather than a task-relevant mask transformation, then the feature is misidentified and provides no new computational degree of freedom.
- If required pump-control hardware, noise, or energy overhead exceeds the benefit of removing a separate mask stage, then the feature weakens rather than improves the system proposition.
- If pump-programmed masking does not improve a relevant benchmark or enable a capability unavailable with the conventional mask, then it is an interesting physical effect but not a useful feature.
