## Feature in brief

SBS operation requires substantial pump power, currently on the order of **1 W**. In the present approach, much of the pump power is discarded after interaction. Pump recuperation would create a closed optical pump loop so that stored circulating pump power can reduce the required externally injected power.

## Potential value

- Reduce external pump-power demand.
- Improve the system-level energy proposition of an SBS-based reservoir.
- Make high-pump-power operation more practical for a future compact system.

## Intended principle

- Form an optical feedback loop for the pump.
- Inject sufficient power to build and maintain the desired circulating pump level.
- Reuse the circulating optical pump instead of discarding most pump power after one pass.

## Bottlenecks and risks

- If optical loop loss and coupling inefficiency exceed the useful recirculated power, then pump recuperation cannot reduce the approximately 1 W external pump requirement documented in [[Technical_Specification]].
- If laser-to-cavity locking cannot maintain a stable pump-loop resonance, then circulating pump power fluctuates and the SBS operating point cannot be controlled.
- If frequency drift, thermal effects, phase instability, or unwanted cavity modes add excessive noise or instability, then pump recuperation degrades rather than improves SBS operation.
- If the recirculating pump destabilises the reservoir or exceeds safety and component limits, then the feature is not deployable.
- If implementation resources exceed the current grant scope, then this remains a longer-term option and must not become a committed deliverable.
