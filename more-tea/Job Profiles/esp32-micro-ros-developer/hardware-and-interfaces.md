# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Custom ESP32 PCB | 3.3 V GPIO; regulated input TBC | Maintain pin map, firmware and electrical limits. |
| Four 12 V motors with encoders | 12 V motor rail; encoder signals must be 3.3 V-safe or shifted | Control motor speed and read direction/counts. |
| Motor drivers | 12 V power domain; logic must accept 3.3 V | Confirm enable, direction/PWM and current-limit behaviour. |
| Emergency stop | Independent motor-disable path | Read/report state, but do not make software the only stopping method. |
| Jetson micro-ROS link | USB serial, UART or approved transport | Define messages, connection/reconnection and timeout. |

## Checks before work begins

- [ ] All ESP32 pins and connector voltages are documented.
- [ ] Encoder voltage is safe for 3.3 V GPIO.
- [ ] Motor outputs stop on lost command/transport.
- [ ] Emergency stop disables movement independently.
