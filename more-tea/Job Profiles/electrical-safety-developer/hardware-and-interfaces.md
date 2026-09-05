# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| 12 V battery system | 12 V nominal; actual operating range TBC | Record chemistry, capacity, charge limits, connector and main protection. |
| Four 12 V motors | 12 V motor rail | Measure typical and stall current. |
| Motor drivers | 12 V power; 3.3 V-compatible control | Confirm per-channel continuous/peak rating and thermal performance. |
| Jetson power branch | Input depends on carrier board; TBC | Use the correct regulator and prevent motor-induced brownouts. |
| ESP32 PCB | 3.3 V logic; board input TBC | Document every external port voltage and protection method. |
| RPLIDAR S2 | 5 V USB/device supply | Provide stable protected power and connection. |
| IMU and touchscreen | Exact supply/interface TBC | Confirm models before regulator or connector selection. |
| Emergency stop and fuses | Independent motor-power/enable path | Stop the base without depending on ROS 2 or micro-ROS. |

## Checks before work begins

- [ ] Component-and-voltage register is complete.
- [ ] Motor stall current is measured.
- [ ] Every branch has suitable wire, connector and protection ratings.
- [ ] Jetson, logic, motor and later arm rails are separated appropriately.
- [ ] Emergency stop works under load.
