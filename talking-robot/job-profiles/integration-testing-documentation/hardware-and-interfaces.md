# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Both Raspberry Pi systems | 5 V compute rails | Record hardware revision, device connections and boot/recovery results. |
| Pet Bot ESP32 and drive system | 3.3 V logic plus TBC motor rail | Track command, heartbeat, sensor and stop acceptance. |
| Desk Buddy servo/audio/display system | Mixed 5 V, TBC servo and TBC amplifier/display rails | Confirm each owner's voltage and interface record exists. |
| Safety controls | Independent local controls | Witness and record emergency stop, mute and motion-stop tests. |

## Checks before work begins

- [ ] Every interface has one named owner.
- [ ] Every powered device appears in a voltage register.
- [ ] Acceptance tests are repeatable from a clean start.
- [ ] Failures are assigned rather than silently worked around.
