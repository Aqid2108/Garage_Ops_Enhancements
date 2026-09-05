# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Raspberry Pi 5, 8 GB | 5 V DC input | Meet memory, CPU and temperature limits during continuous camera use. |
| Single-lens camera | USB 5 V or camera-interface supply, depending on model | Record resolution, frame rate, field of view and device path. |
| Pet Bot drive interface | Software command boundary only | Send bounded direction requests through the approved controls API. |

## Checks before work begins

- [ ] Camera model and interface are recorded.
- [ ] Recognition uses only approved people/data.
- [ ] Target loss produces a safe stop or no-request state.
- [ ] The vision process remains lightweight enough for the Raspberry Pi.
