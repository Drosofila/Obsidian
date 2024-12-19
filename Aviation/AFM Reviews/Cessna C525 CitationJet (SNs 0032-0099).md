# Limitations

- 

# Normal Procedures

# Performance

# Systems

## 1 - Aircraft General

- Engines: Williams International **FJ-44-1A** @ 1900 LBS thrust.
- Wingspan: 46.38 ft / 
---
- Electrical System: 29V, two starter-generators, AC power provided by 2 inverters.
- Fuel System: 2 equal sides, one for each engine, cross-feed possible.
- Thrust attenuators mounted on the engines allow for assisted deceleration and avoidance of excessive use of brakes during taxi.
- De-icing:
	- Wings and nacelle: Hot bleed air
	- Horizontal Stabilizer: inflatable boots
	- Windshield: 
		- Primary: bleed air
		- Secondary: Isopropyl alcohol
	- Probes: electrical heating
- Hydraulic system: 2 engine driven pumps and one independent system for the landing gear. Pneumatic backup.
- Flight Controls: Conventional cable-pulley, mechanical and electrical elevator trim, hydraulically operated speed brakes and flaps.
- Pressurization: from bleed air, ram air and vapor cycle A/C.

## 2 - Electrical Power Systems

- Battery: Nickel-Cadmium, **25V**, 28Ah
- Starter Generators: 
	- 2 engine-driven starter generators on each gearbox
	- Primary source for power supply for each DC bus
	- 30VDC regulated to **29VDC**, 300 amperes.
	- Share the load equally (within 10% of the total load) via equalizer during normal operations.
- External Power: Should be regulated to 29VDC with an output between 800 and 1100 amperes.
- Distribution
	- 10 buses
---
- Control
	- Battery: BATT, ON, EMER
	- Generators: L/R GEN, OFF, RESET
---
- Operation
	- Generator Switches:
		- GEN → if a battery start is intended
		- OFF → if a GPU start is intended
			- On GPU starts, start both engines, remove GPU and then connect the generators - this way both engines are started using GPU power and not generator assisted start.
---
- AC Power
	- 2 Static Inverters: 26VAC/115VAC, 400 Hz
	- One bus 26V, second bus 115V
	- Inverters: Convert 29DC → AC, max 250 VA output
		- On during the before taxi checklist (activated and tested) and off before engine shutdown.
	- One inverter is fully capable of powering both AC buses.

## 3 - Lighting

- Landing/Recognition/Taxi Lights:
	- Mounted Below the fuselage
	- Each light is a fixed-position sealed beam lamp.
	- Landing: brightest illumination for landing
	- Recog/Taxi: lower illumination through a resistor (extending lamp life)

## 4 - Master Warning Systems


## 5 - Fuel System

- General:
	- 2 tanks, one for each wing
	- Each tank feeds its respective engine
	- One electrical and one ejector pump per engine
- Tanks:
	- Wet wing, integral to each wing
	- Total usable fuel is 3220 lbs / 238 US Gal per wing
	- NACA Vents
	- 8 Drains total
- Boost Pumps
	- Electrical DC 
	- Centrifugal
	- One for each tank
- Ejector Pumps
	- One for each wing
	- Powered by fuel flow (jet or motion pumps)
- Crossfeed Valve
	- Electrically opened solenoid springloaded closed in the loss of normal DC power
	- Controlled by the crossfeed switch
		- Selecting a tank:
			- Turns the electrical boost pump on the tank on
			- Opens the crossfeed valve
			- Pumps fuel to the opposite engine + sump
		- The heavy wing is always selected to balance fuel
		- FUEL CROSFEED light illuminates
- Shutoff Valves
	- Firewall: controlled by the red LH/RH FIRE switches
- Controls
	- Fuel Boost Pumps Switches:
		- 3 Positions: On - Off - Normal
		- In the Normal position the pumps are operated automatically throughout the flight during engine start and low fuel pressure in the supply line.
	- Crossfeed Selector:
		- Selects the tank from which fuel is to to be taken and the engine to be supplied.
- Indications:
	- Quantity:
		- Capacitance probes
		- DC power
		- Fuel flow indication is disable until throttles are advanced to idle
- Operation
	- Maximum fuel imbalance:
		- Normal: 200 lbs
		- Emergency: 600 lbs
	- Crossfeed system does not work when the boost pump switch is on the off position
	- If both boost pumps are energized (indicator lights) during crossfeed, crossfeed will not occur - cycle the non-selected tank switch to on then back to normal
	- Likewise, crossfeed can be avoided by running both boost pumps continuously
	- Balance fuel below FL290 → the crossfeed system might not work above this altitude

## 7 - Powerplant

- General:
	- Williams-Rolls FJ44-1A
	- 1900 lbs of thrust
- Ignition starts automatically during start and when engine anti-ice is selected on
- Engine start abort conditions:
	- False Start → no ITT or FF within 10 s
	- Hot Start → ITT rapidly approaching 1000C
	- No N1 rotation by 12% N2
	- Hung Start → Slow or no rotation after ITT rise and before reaching idle rpm
- 