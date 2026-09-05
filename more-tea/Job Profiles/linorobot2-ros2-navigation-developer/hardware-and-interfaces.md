# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Jetson Orin Nano, 8 GB | Input depends on carrier board; verify exact requirement | Run the Humble physical deployment and keep storage/cooling stable. |
| Custom ESP32 PCB | 3.3 V logic; board input TBC | Use the defined micro-ROS boundary; do not bypass it. |
| RPLIDAR S2 | 5 V USB/device supply | Consume a stable `/scan` topic with correct frame and device mapping. |
| IMU | USB 5 V or device-specific supply; TBC | Consume calibrated data through the sensor owner. |
| 10-inch touchscreen | Supply/interface TBC | Provide destination selection and status feedback. |
| Four-wheel base | 12 V motor domain; controlled through ESP32/drivers | Use velocity commands and odometry, not direct power commands. |

## Checks before work begins

- [ ] Jazzy learning workspace and Humble deployment are both reproducible.
- [ ] Hardware device names and frame names are stable.
- [ ] Navigation cannot override the emergency stop or ESP32 timeout.
- [ ] All shared code builds in the Humble compatibility floor.
