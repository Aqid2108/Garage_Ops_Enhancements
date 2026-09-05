# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Motor battery | Voltage and capacity TBC after motor selection | Record chemistry, voltage range, connector, fuse and safe charging method. |
| Four DC motors | Nominal voltage TBC | Record typical and stall current for driver and wiring selection. |
| Motor-driver system | Motor rail TBC; 3.3 V-compatible control | Confirm per-channel continuous and peak current ratings. |
| ESP32 PCB | 3.3 V logic; regulated input TBC | Document ICs, pinout, external port voltages and protection. |
| Raspberry Pi 5 | 5 V DC input | Provide a stable compute branch isolated from motor noise and brownouts. |
| STS3215 servo branch | Exact servo variant voltage TBC | Use a dedicated supply; do not power servos from the Raspberry Pi. |
| Emergency stop and fuses | Placed in the relevant battery/motor branches | Provide independent isolation and fault protection. |

## Checks before work begins

- [ ] The component-and-voltage register is complete.
- [ ] Every connector shows voltage, polarity and current limit.
- [ ] Motor stall current is known before driver approval.
- [ ] Compute, motor and servo rails are separately protected.
- [ ] Emergency stop is tested under load.
