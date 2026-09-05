# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Jetson Orin Nano | Carrier-board input TBC | Run the ROS 2 control and base interface. |
| ESP32 micro-ROS controller | 3.3 V logic | Receive commands and return wheel feedback through the agreed messages. |
| Four encoders | Signal domain defined by ESP32 owner | Use counts and timestamps with documented units. |
| Four-wheel base | 12 V motor domain | Model wheel order, radius, separation and skid-steer behaviour correctly. |

## Checks before work begins

- [ ] Wheel names/order match physical wiring.
- [ ] Units are SI and documented.
- [ ] Stale data is detectable.
- [ ] Transport loss produces a safe timeout rather than persistent motion.
