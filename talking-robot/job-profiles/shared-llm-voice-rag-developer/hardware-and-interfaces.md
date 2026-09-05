# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Raspberry Pi 5, 8 GB | 5 V DC input through a suitable USB-C supply | Keep inference, audio and retrieval within the available compute and memory. |
| USB microphone / microphone array | 5 V USB | Confirm device name, input level, sample rate and reconnect behaviour. |
| Amplified speaker system | Supply depends on selected amplifier; TBC | Confirm output device, safe volume and power requirement. |
| Display / touchscreen | Supply and interface depend on selected model; TBC | Show system state, sources and errors without blocking voice. |
| Pi-to-ESP32 / servo interface | USB or 3.3 V-safe UART | Send validated high-level requests; never bypass local safety logic. |

## Checks before work begins

- [ ] Exact microphone, speaker amplifier and display model are recorded.
- [ ] Every USB/audio device has a stable software identifier.
- [ ] No LLM output can directly command raw motor power or unrestricted servo motion.
