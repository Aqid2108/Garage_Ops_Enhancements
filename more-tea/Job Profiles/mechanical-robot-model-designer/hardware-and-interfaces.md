# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Four-wheel chassis | Mechanical interface | Measure wheel radius/diameter, effective track width, wheelbase and ground clearance. |
| RPLIDAR S2 | Keep 360° view clear | Mount level and record xyz/rpy. |
| IMU | Rigid low-vibration mount | Record orientation and position. |
| Jetson and cooling | Carrier/power constraints from electrical role | Provide mounting, airflow and maintenance access. |
| 10-inch touchscreen | Supply/interface owned by electrical role | Provide reachable viewing angle and protected cable route. |
| Later arm/gripper | Load and centre-of-gravity TBC | Provide safe stow only after navigation acceptance. |

## Checks before work begins

- [ ] All geometry is measured on the actual platform.
- [ ] LiDAR view is unobstructed.
- [ ] IMU orientation is documented.
- [ ] Emergency stop remains reachable.
- [ ] Later arm cannot be installed before navigation acceptance.
