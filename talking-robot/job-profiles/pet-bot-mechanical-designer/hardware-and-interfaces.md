# Hardware and Interfaces

The values below identify the electrical domain the member will encounter. **TBC** means the exact component or rating must be confirmed from the selected part's datasheet before connection or purchase.

| Component / interface | Voltage or signal domain | What this role must do |
| --- | --- | --- |
| Four motors and wheels | Mechanical interface; electrical rating owned by PCB role | Record motor body, shaft, fastener, wheel and mounting dimensions. |
| Two ultrasonic sensors | No mechanical voltage work | Provide unobstructed front-left/front-right fields of view. |
| Two IR sensors | No mechanical voltage work | Mount downward near front corners with adjustable height/angle. |
| Raspberry Pi, ESP32 and drivers | Keep electrical clearances and airflow | Provide mounting, ventilation and service access. |
| Battery and emergency stop | Keep terminals protected | Provide restraint and immediate user access to the stop control. |
| STS3215 expression mechanism | Dedicated servo wiring space | Provide travel clearance, hard-stop protection and cable routing. |

## Checks before work begins

- [ ] All dimensions come from measured parts or approved drawings.
- [ ] Sensor sightlines are unobstructed.
- [ ] Battery cannot move during driving.
- [ ] Emergency stop is reachable.
- [ ] No moving part can pinch a cable.
