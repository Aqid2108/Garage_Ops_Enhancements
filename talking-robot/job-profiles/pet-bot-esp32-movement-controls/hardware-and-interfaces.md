# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| ESP32 board / custom PCB | 3.3 V GPIO; board input depends on exact design | Maintain a reviewed pin map and protect every input from overvoltage. |
| Four geared DC motors | Nominal motor voltage TBC | Confirm direction, stall current and safe duty cycle before full integration. |
| Motor drivers | Motor rail follows motor rating; logic must accept 3.3 V | Use one four-channel or two dual-channel boards only after current sizing. |
| Two ultrasonic sensors | Exact sensor voltage TBC | Alternate triggers; level-shift any 5 V Echo output before ESP32 input. |
| Two downward IR sensors | Exact sensor voltage/output TBC; output must be 3.3 V-safe | Calibrate on the real table and lighting. |
| Raspberry Pi link | USB serial or 3.3 V-safe UART | Implement commands, feedback, heartbeat and timeout. |

## Checks before work begins

- [ ] Pin map matches the actual board and wiring.
- [ ] Every sensor output is safe for 3.3 V GPIO.
- [ ] Command timeout stops the motors without Raspberry Pi assistance.
- [ ] Reverse motion is limited because no rear IR edge sensor is installed.
