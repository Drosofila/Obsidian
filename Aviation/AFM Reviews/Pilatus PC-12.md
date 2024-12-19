# Limitations

## Speeds:

- Vmo: 236 KIAS
- Vfe: 163/130 KIAS
- Vlo: 177 KIAS
- Vle: 236 KIAS

## Engine:

- MAX SHP: 1200
- MAX Torque: 44.34 PSI (Yellow Band), 46.9 PSI Climb (Green Band)
- MAX ITT:
	- 800C for takeoff
	- 760C for climb (Usually set below 720C)
	- 1000 (3s) during engine start
- MAX RPM: 1700

- Fuel: Jet-A

## Weights:

- Max. Ramp Weight: 9965 lbs
- Max. Takeoff Weight: 9921 lbs
- Max. Landing Weight: 9921 lbs
- Max. Baggage Weight: 300 lbs

## Fuel:

- 

# Normal Procedures

## Checklist Draft

BEFORE START

Preflight inspection
Doors
Fuel Quantity
Circuit Breakers
Gust Lock
Oxygen Lever
ECS
PCL
Condition Lever
Beacon Light

BEFORE TAXI

Generators
Avionics
Inertial Separator
ECS
Pressurization
Flaps
Autopilot
Pusher Test
Flight Controls
Flight Instruments
Taxi Light

BEFORE TAKEOFF

Trims
Flaps
De-ice systems
Transponder
Condition Lever
CAWS
Takeoff runway

CLIMB CHECKLIST

Landing Gear
Flaps
Yaw Damper
Climb Power
Taxi and Landing Lights

CLIMB CHECKLIST BELOW THE LINE

Inertial Separator
Pressurization
Recognition Lights


APPROACH CHECKLIST

Approach Briefing
Fuel Quantity
Pressurization

APPROACH CHECKLIST BELOW THE LINE

Atimeters
Inertial Separator
Ice Protection

LANDING CHECKLIST

Flaps
Landing Gear
Yaw Damper
Pressurization

SHUTDOWN CHECKLIST

Parking Brake
ECS and cooling system
Avionics
Generators
Condition Lever
Oxygen Lever
Batteries

## Airspeeds for Normal Operation

- Vr: 
	- Flaps 15 = 79 KIAS
	- Flaps 30 = 73 KIAS
- Vx = 110 KIAS
- Vy = 120 KIAS
- Cruise Climb Speed - Pusher in Ice Mode = 135 KIAS
- FIKI Holding Speeds - 140 to 170 KIAS
- Landing and Approach Speeds:
	- Flaps 0 = 118 KIAS
	- Flaps 15 = 98 KIAS
	- Flaps 30 = 89 KIAS
	- Flaps 40 = 84 KIAS


## Receiving Flow

[[PC12 Receiving Flow]]

```ad-info
title: Flow Overview

- The goal of this flow is to check systems inital condition, run the initial preflight checks and energize the airplane for start.
- This flow begins at the LH Circuit Breaker Panel and ends after turining on the STBY Bus to get weather and clearance.


```

| Item                    |   Action   | Notes                                                 |
| :---------------------- | :--------: | :---------------------------------------------------- |
| LH CB Panel             |   CHECK    |                                                       |
| LH EFIS                 |   NORMAL   |                                                       |
| EPS                     | TEST + ARM | Give the test light 5 s to confirm normal BATT charge |
| AHRS                    |   SLAVE    |                                                       |
| Landing Gear            |    DOWN    |                                                       |
| Oxygen                  |     ON     |                                                       |
| Trim + Flap Interrupt   |   NORMAL   |                                                       |
| ALTN Flap               |   NORMAL   |                                                       |
| PWR Quadrant            |   CHECK    |                                                       |
| Flaps                   |     UP     |                                                       |
| Lights                  |   NORMAL   |                                                       |
| Shutoff and Manual Gear |   STOWED   |                                                       |
| ECS                     |    OFF     |                                                       |
| Temperature Sel         |    SET     |                                                       |
| Pressurization          |    SET     |                                                       |
| RH EFIS                 |   NORMAL   |                                                       |
| RH CB Panel             |   CHECK    |                                                       |

---

| Item               | Action | Notes                |
| :----------------- | :----: | :------------------- |
| BATT 1 + 2         |   ON   |                      |
| Nav Lights         |   ON   |                      |
| Fire Test          |  TEST  | CAWS and Aural       |
| Fuel Pumps         |  TEST  | CAWS and Audible Hum |
| Inertial Separator |  OPEN  |                      |
| Ventilation System |  OFF   |                      |
| STBY Bus           |   ON   |                      |

> [!example] Get ATIS and Clearance
> 

| Item           | Action | Notes |
| :------------- | :----: | :---- |
| EIS            |  TEST  |       |
| Fuel Totalizer | RESET  |       |
| CAWS           | CHECK  |       |
| Oxygen         | CHECK  |       |
| BATT Volts     | CHECK  |       |
| Beacon         |   ON   |       |
| Start Area     | CLEAR  |       |
|                |        |       |

> [!check] Before Start Checklist
> 




```ad-info
title: Flow

Test EIS + Fuel Totalizer Reset -> CAWS -> Oxygen Check -> BATT Voltage Check -> Beacon Light -> Start Area Clear -> Starter Engage

```

## Engine Start

```ad-abstract
title: Start Procedure


```

```ad-caution
title: Limitations

- Stable Engine Start: ITT Stable < 800C, NG > 50%, Oil temperature and pressure normal
- 10 seconds limit between moving lever to GND IDLE and ITT + NG rise
- Initial ITT below 150C

```

## After Start

[[PC12 After Start]]

```ad-summary
title: Flow Overview

- This flows comes after a good engine start, with parameters within minimums.
- This flows starts at the generators and ends when setting the flight instruments and navigation for takeoff
- The goal is to establish AC power from the generators to the plane, set up the ventilation systems and check the final systems required for takeoff

```

| Item               | Action  | Notes                               |
|:------------------ |:-------:|:----------------------------------- |
| Generator 2        |   ON    | Generator 2 first, then generator 1 |
| Generator 1        |   ON    |                                     |
| Avionics 1         |   ON    |                                     |
| Avionics 2         |   ON    |                                     |
| STBY Bus           |   OFF   |                                     |
| Ventilation System |   SET   |                                     |
| ECS                |  AUTO   |                                     |
| Flaps              |   15    |                                     |
| Fuel Totalizer     |  RESET  |                                     |
| Autopilot          |  TEST*  |                                     |
| Pusher Test        | TEST**  | Requires flaps 15, PCL > 5 PSI      |
| Flight Controls    |  CHECK  |                                     |
| Flight Instruments | CHECKED |                                     |

> [!check]  Before Taxi Checklist

```ad-question
title: Test Procedures

*AP Test: Press the test switch until you can hear the aural, then engage the AP and check if it can be overpowered by control inputs, then disengage AP.

** Pusher Test: Set PCL to 5-10PSI, press and hold the test switch, check CAWS Pusher Ice ON, check pusher and audio warning 3 times, interrupt the pusher with the yoke and then release the test switch. Check elevator movement.

```


## Before Takeoff

```ad-summary
title: Flow

- This flow is performed right before entering the RWY for TO
- The goal is to set the plane for takeoff

```

| Item            |        Action        | Notes |
| :-------------- | :------------------: | :---- |
| Flaps           |       15 (30)        |       |
| Trims           |      SET FOR TO      |       |
| Condition Lever |      HIGH IDLE       |       |
| Lights          | LDG + STROBE + RECOG |       |
| Yaw Damper      |     CONFIRM OFF      |       |
| Transponder     |         ALT          |       |
| CAWS            |        CHECK         |       |

```ad-hint
title: FAT/FLY

**F**laps-**A**nd-**T**rim / **F**light Idle, **L**ights, **Y**aw Damper OFF

```

```ad-check
title: Before Takeoff Checklist


```

> [!info] Rotation Speed: 80 KIAS
> 

## After Takeoff

```ad-summary
title: Flow

- Gear UP -> Lights OFF -> YD ON
- (100 KIAS) Flaps UP -> CLB PWR Set

```

> [!info] Flaps UP -> Accelerate to Vy = 120 KIAS

> [!info] Gear UP → Accelerate to Cruise Climb = 150 KIAS
> 

> [!check] Climb Checklist - To The Line
> 
## Climb

- Monitor Engine Instruments
- Climb at 150 KIAS for normal ops (140 KIAS above 18000 ft)
- Monitor Pressurization System

 ```ad-warning
title: Climb Limitations

- Set Climb PWR to MAX torque or MAX ITT of 720C

```

```ad-abstract
title: 10000 ft Flow

Inertial Separator OFF -> Recognition Light OFF -> Pressurization Check

```

> [!check] Climb Checklist - Below The Line
> 

## Cruise

- Check Pressurization
- Monitor Flight Plan and Fuel Consumption
- Set PCL to Cruise PWR according to performance tables
- Monitor pressurization
- Close initial separator if possible

```ad-warning
title: Cruise Limitations

- Pressurization: Cabin pressure differential must be < 5.75 PSI - values above that indicate a pressurization control system malfunction.
- Set Cruise Power to 685C ITT

```

## Descent

```ad-abstract
title: Flow

- Set pressurization controller to landing altitude + 500 ft.
- Brief Approach
- Set Up Instruments for approach

```

> [!check] Approach Checklist to the line
> 

```ad-abstract
title: 10000 ft Flow

- Open Inertial Separator
- Turn On Recog Lights
- Check Pressurization

```

> [!check] Approach Checklist Below The Line
> 

## Approach

- Set Altimeters as required
- Recheck fuel remaining according to FP

```ad-abstract
title: Flow

- Gear Down
- Landing + Taxi Lights Down
- Flaps - 15*
- AP + YD OFF
```

> [!check] Landing Checklist
> 

## After Landing

```ad-abstract
title: Flow

- Pedestal: Condition lever - GND Idle -> Flaps UP
- Overhead: Lights - As Required -> All Anti-Ice systems OFF
- FO Panel - XPDR As Required

```

| Item             |   Action    | Notes |
| :--------------- | :---------: | :---- |
| Condition Lever  | GROUND IDLE |       |
| Flaps            |     UP      |       |
| Lights           | AS REQUIRED |       |
| Anti Ice Systems |   ALL OFF   |       |
| Transponder      | AS REQUIRED |       |
| Trims            |    RESET    |       |

## Shutdown

```ad-abstract
title: Flow

- ECS - OFF
- Overhead: Lights - OFF -> Cooling and Heating System - OFF -> AV1 + 2 - OFF -> GEN 2 -> 1 - OFF
- Contition Lever - CUTOFF
- Oxygen Lever - OFF
- BAT 1 + 2 - OFF
- EPS - OFF
- Control Locks and Window Shades - Install

```

| Item               |     Action     | Notes                |
| :----------------- | :------------: | :------------------- |
| ECS                |      OFF       |                      |
| Ventilation System |      OFF       |                      |
| Avionics           |      OFF       |                      |
| Generator 2        |      OFF       | Turn Gen 2 OFF first |
| Generator 1        |      OFF       |                      |
| Condition Lever    | FEATHER CUTOFF |                      |
| Oxygen             |      OFF       |                      |
| Fuel Used          |      NOTE      |                      |
| Batteries          |      OFF       |                      |
| Control Locks      |    INSTALL     |                      |
| Window Shades      |    INSTALL     |                      |

> [!check] Shutdown Checklist
> 

## Maneuvers

### Visual Approach

- Downwind Leg (**Double 15**):
	- PCL: 15 PSI
	- Flaps: 15
- Abeam Threshold
	- Gear Down + Taxi and Landing Lights
	- PCL: 8-10 PSI
- Base Leg
	- Flaps: 30
	- Vref = 89 KIAS
- Final
	- Landing Checklist
	- Flaps as required (40 if maximum performance landing)

> [!caution] Monitor AOA during all phases of the visual approach
> 

# Performance

# Systems

## 