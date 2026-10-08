## Application in brief

LiDAR and related ranging systems generate optical returns that encode distance, motion, and scene information. A reservoir could perform a narrowly defined early processing task before the main electronic compute stage.

## Why it fits the project

- Optical ranging is a potential optical-native input source.
- The value proposition is reduced energy use and downstream electronic-compute burden, not merely faster LiDAR processing.
- Candidate functions include temporal pre-processing, event detection, classification, tracking support, and sensor-health monitoring.

## Bottlenecks and risks

- If the intended function is not narrowed to a task such as event detection, classification, tracking support, or sensor-health monitoring, then “LiDAR processing” is too broad to validate or commercialise.
- If the necessary distance, phase, frequency, or time-of-flight information becomes available only after photodetection, then the reservoir cannot provide the intended optical-domain pre-processing.
- If relevant temporal dynamics do not fit the SBS response in [[Technical_Specification]], then the current platform cannot process the useful LiDAR signal.
- If optical conditions such as reflectivity, ambient light, weather, motion, or alignment make the output unstable, then the system cannot support reliable ranging or perception.
- If the reservoir output cannot connect to a defined perception or control decision, then reducing electronic compute has no system-level value.
- If no partner can provide representative optical-ranging data or a bench testbed, then the direction cannot be evaluated beyond synthetic data.
