# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| RPLIDAR S2 | 5 V USB/device supply | Mount level with clear 360° view and stable USB identification. |
| IMU | USB 5 V or device-specific supply; TBC | Record orientation, rate, calibration and interface. |
| Jetson USB/interfaces | 5 V USB plus protected host interfaces | Prevent port changes, loose cables and intermittent devices. |
| Sensor mounts | Mechanical interface | Document xyz/rpy relative to base_link. |

## Checks before work begins

- [ ] Exact IMU model and voltage/interface are recorded.
- [ ] LiDAR has no body obstruction.
- [ ] Frame names and transforms match the physical mounts.
- [ ] Topic timestamps and rates remain stable during motion.
