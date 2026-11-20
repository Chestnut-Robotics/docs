# Aero UMI specifications

Current production revision.

## Kinematics and matching

| Specification | Value |
|---|---|
| Matched hand | 18-DoF Aero Hand, joint for joint |
| Degrees of freedom | 18 (15 measured + 3 coupled) |
| Tracked axes | Four fingers: 3 each (MCP abduction/adduction and flexion, PIP flexion) · thumb: 3 (CMC abduction/opposition, MCP and IP flexion) |
| Mapping | Direct joint-to-joint passthrough to the 15 active DoF of Aero Hand |

## Joint sensing and accuracy

| Specification | Value |
|---|---|
| Encoders | Miniature absolute magnetic encoders on all 15 measured joints, resistant to EMI and vibration |
| Angular resolution | ≤ 0.05° (14 to 16 bit) |
| Joint repeatability | 0.1° |
| Tracking accuracy (MPJPE) | ≤ 5.0 mm as worn · ≤ 2.0 mm calibrated |
| Calibration | Factory product-of-exponentials calibration with real-time deflection compensation |

## Tactile

| Specification | Value |
|---|---|
| Channels | About 500: 54–57 per fingertip, 213 on the palm |
| Modules | Six: five fingertips and the palm |
| Force resolution | 0.1 N |
| Force axes | Normal and 2D shear (3-axis) |
| Sensor type | Conformal flexible piezoresistive arrays |
| Sensing range | 0.1–20 N |
| Refresh rate | 70–100 Hz |

## Data, sync and tracking

| Specification | Value |
|---|---|
| Clock | Single hardware-triggered clock line, no OS scheduling jitter |
| Cross-stream alignment | < 1 ms, verified on every episode |
| Streams | Hand joint angles · tactile force · wrist 6-DoF pose · wrist RGB (optional) · head module streams when fitted |
| Wrist 6-DoF tracking | Optical-inertial fusion, sub-millimeter trajectory accuracy |
| Connectivity | USB-C wired · Wi-Fi 6E wireless |
| Output | Packets with hardware timestamps, over ROS 2, ZeroMQ or gRPC |

## Ergonomics and environment

| Specification | Value |
|---|---|
| Weight | 320 g, including cables and straps |
| Hand size fit | Optimized for 50th-percentile adult male hands, fits 40th to 70th, sliding joints adapt to finger length |
| Time to put on | < 10 s, hook-and-loop straps |
| Continuous capture | 8 h, with hot-swappable spare battery |
| Operating environment | 0–45 °C, 10% to 90% RH, non-condensing |

See [Tactile interface](tactile.md) for wiring and channel layout.
