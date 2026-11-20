# Aero Hand specifications

Hardware revision R2.7.

## Structure

| Specification | Value |
|---|---|
| Fingers | 5 |
| Degrees of freedom | 18 (15 active + 3 coupled) |
| DoF distribution | Thumb 3 active, with opposition · index, middle and ring 3 active + 1 coupled each · little finger 3 active |
| Drive | Direct drive |
| Weight | ≤ 800 g |
| Dimensions | 198 × 103 × 43 mm (L × W × T) |
| Materials | Plastic and aluminum alloy frame · silicone fingertips and palm |

## Performance

| Specification | Value |
|---|---|
| Fingertip pinch force | 10 N max |
| Power grasp force | 45 N max |
| Closing speed | Full open to full close ≤ 0.5 s (2 Hz) |
| Repeatability | ±1.0 mm, measured at the fingertip |

## Sensing

| Specification | Value |
|---|---|
| Joint angle | 14-bit magnetic encoders, 0.05° accuracy |
| Joint torque | Estimated from motor current |
| Tactile | Six modules on the fingertips and palm |
| Tactile resolution | 0.1 N |

## Electrical and communication

| Specification | Value |
|---|---|
| Operating voltage | 20–50 VDC wide input |
| Continuous stall current | 6 A at 24 VDC |
| Standby power | < 7.2 W |
| Communication | CAN FD |
| Control frequency | 10 kHz low-level current loop · 200 Hz high-level communication |
| Connectors | XT30-M power · A1257H-CJT CAN FD |

## Software and control

| Specification | Value |
|---|---|
| Control modes | Position · velocity · torque/current (MIT mode) · impedance |
| Supported systems | Ubuntu · Windows · ROS 2 |
| SDK / API | C++ and Python libraries · URDF · teleoperation support |

## Environment and reliability

| Specification | Value |
|---|---|
| Operating temperature | −10 °C to +60 °C |
| Storage temperature | −20 °C to +70 °C |
| Operating humidity | 10% to 90% RH, non-condensing |
| Protection | IP54 |
| Shock | Passes 1 m drop test |
| Lifetime (MTBF) | > 300,000 full grasp cycles |

## Mounting and package

| Specification | Value |
|---|---|
| Mounting | Adapter flange for robot arms |
| In the box | Aero Hand · integrated power cable · 2 communication cables · CAN FD to USB converter board |

See [Electrical and communication](electrical.md) and [Tactile interface](tactile.md) for wiring.
