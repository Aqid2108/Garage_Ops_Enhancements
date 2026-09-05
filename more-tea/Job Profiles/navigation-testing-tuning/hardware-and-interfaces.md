# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Complete four-wheel base | 12 V motor domain with independent stop | Test in a controlled area with a spotter and clear stop access. |
| Jetson and ESP32 | Compute/3.3 V logic domains | Record versions, startup state and communication health. |
| LiDAR and IMU | 5 V USB/device-specific interfaces | Record data rate, dropouts and recovery. |
| 10-inch touchscreen | Supply/interface TBC | Test goal selection, cancel and operator feedback. |

## Checks before work begins

- [ ] Each test states setup, steps, expected result and pass/fail rule.
- [ ] Emergency stop is checked before movement.
- [ ] Software versions and hardware configuration are recorded.
- [ ] Failed tests include an owner and retest link.
