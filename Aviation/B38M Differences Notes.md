### The Engines

- CFMI LEAP-1B.
- Dual-rotor, axial-flow high bypass turbofan
- N1 is consisted of a fan and a low pressure compressor and N2 is consisted of a High pressure compressor and a high pressure turbine. They are both mechanically independent.
- Each engine is regulated by a dual channel EEC.
- The primary engine indications are: N1 and EGT
- The secondary engine indications are: N2, Oil Pressure, Oil Temperature, Fuel Flow and Engine Vibration. the secondary engine indications are automatically displayed when an engine start lever is moved to cutoff, N2 is below idle or any secondary indications are exceeded.
- A full authority EEC is installed for each engine with 2 independent channels for each one, that are alternated for each flight. EEC controls thrust using N1 via normal and alternate control modes. The control modes can be manually changed via the overhead switches.
- EEC Normal Mode:
    - Sensed Flight condition & bleed air demand to calculate N1.
    - Uses fuel flow to match actual N1 to calculated N1 setting.
- EEC Alternate Mode:
    - Soft:
        - Changed to automatically if there’s no signal source for normal operation
        - `ALTN` switch is illuminated ON
        - Uses last flight conditions for parameters
        - Remains on until retarding thrust to idle or manually selection ALTN.
    - Hard:
        - Reversion to the alternate mode thrust schedule
        - Provides equal or grater thrust for a thrust lever position in normal mode
- IDLE Selection by the EEC is automatic:
    - Ground idle, flight idle, approach idle and icing idle.
    - If EEC loses the signal source, approach idle is selected from 19000 ft and below.
- `FUEL FILTER BYPASS` → Overhead Engine Panel.
- `OIL FILTER BYPASS` → Engine Display.
- Engine Starting:
    - Start requires electrical and pneumatic power.
    - Engine bleed air valve is closed and start valve is opened by battery electrical power.
    - Starter rotates the N2 through the accessory gearbox
    - When the start switch is moved to GRD, the EEC performs `Bowed Rotor Motoring (BRM)` before the engine start lever is moved to idle. This is because the N1 and N2 start shafts bow after shutdown due to thermal buildup. BRM is active for 6 - 90 seconds on the ground only. `Motoring` is displayed on the N2 gauge from 18% N2 to 24% N2
    - After moving the engine start lever to idle, the EEC runs tests for the TCMA and EOS functions. Fuel flow indicates zero and the engine shutoff valve open and closes repeatedly, causing the `ENG VALVE CLOSED` to illuminate bright blue continuously until the test ends. Then, both fuel valves open and fuel is introduced to the engine.
    - Starter cutout speed on the LEAP-1B is ~63% N2.
- Engine ignition system:
    - Each engine has 2 igniter plugs, and the EEC uses the system (L, R or BOTH) selected by the ignition select switch.

### The APU

- A self contained gas turbine engine
- Starts and operates up to the airplane’s maximum certified altitude.
- Supply bleed air for both packs on the ground and one pack on the air.
- The APU has an inlet door on the right side of the aft fuselage/tail cone that has 3 positions: closed, flight open and ground open. The operation of the door is automatic.
- Fuel is supplied from the left side of the fuel manifold if an electric AC pump is on. If no AC pump is on, fuel is suction fed from tank 1.
- Starting and shutdown:
    - Automatic start sequence started moving the start switch to START.
    - APU GEN OFF BUS illuminates when the APU is ready to receive electrical load.
    - The start cycle automatically terminates if the APU does not reach proper speed.
    - The APU should be operated for 2 full minutes before using it as an air source.
    - The APU should be operated for 1 full minute without bleed air load before shutdown - this time delay is achieved automatically when the switch is moved to the OFF position.