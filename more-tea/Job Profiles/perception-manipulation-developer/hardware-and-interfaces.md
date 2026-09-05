# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Camera or depth camera | USB/device-specific supply; TBC | Record model, calibration, mounting and compute load. |
| Robot arm and gripper | Voltage/current depends on selected actuators; TBC | Confirm torque, travel, load and controller before use. |
| STS3215 servos, if selected | Exact servo variant voltage TBC | Verify torque/speed/travel and use a dedicated servo power rail. |
| Serial servo controller, if selected | Controller input/interface TBC | Document bus, IDs, baud rate, limits and power arrangement. |
| Jetson | Carrier-board input TBC | Run perception and MoveIt 2 without starving navigation resources. |
| Arm mount/stow | Mechanical and centre-of-gravity interface | Keep arm within a safe envelope and navigation footprint. |

## Checks before work begins

- [ ] Navigation acceptance is recorded before physical integration.
- [ ] Component-and-voltage register is complete for the arm chain.
- [ ] Servo/actuator torque and load are verified.
- [ ] Arm power is isolated from navigation compute.
- [ ] Base and arm stop conditions are documented.
