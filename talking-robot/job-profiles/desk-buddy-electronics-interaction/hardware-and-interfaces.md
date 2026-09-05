# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Raspberry Pi 5, 8 GB | 5 V DC input | Provide stable compute power and USB/device connections. |
| Microphone / microphone array | 5 V USB | Confirm input level, device name and placement. |
| Speaker amplifier and speakers | Amplifier supply TBC | Document speaker impedance/power and safe volume. |
| Display / touchscreen | Supply and interface TBC | Document power, HDMI/DSI/USB interface and mounting. |
| STS3215 serial bus servos | Exact variant voltage TBC | Set IDs, limits, speed and safe travel; use a separate power rail. |
| Serial servo controller board | Controller input/interface TBC; USB or UART to Pi | Document ports, bus wiring and power arrangement. |
| Mute / motion-stop control | Logic/interface TBC | Provide immediate local control independent of the LLM. |

## Checks before work begins

- [ ] The component-and-voltage register is complete.
- [ ] Servo voltage matches the exact STS3215 variant.
- [ ] Servos are not powered from the Raspberry Pi.
- [ ] Speaker impedance and amplifier rating are compatible.
- [ ] Mute and servo-stop controls work without the LLM.
