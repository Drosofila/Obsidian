### Types of Final Approach Phase

- Per ICAO Doc 8168 Vol 1, Chapter 5, there are 4 types of Final Approach Phase: Non-Precision Approach (NPA) with FAF, NPA Without FAF, Approach with vertical guidance (APV) and Precision Approach.
- NPA with FAF: Final Approach Begins at the FAF and ends at the MAPt. The FAF is a fix sited on the final approach track at a distance allowing final approach configuration selection and the start of final descent toward the MDA(H). Optimum distance is 5 NM.
- NPA without FAF: Sometimes the type and location of the navaid don’t allow for the establishment of a FAF. In these NPAs there is no FAF published and the descent to MDA(H) is started once the aircraft is inbound the final approach track.
- APV: Approach procedures that use Baro-VNAV or SBAS for Glide Path. These approaches are published with DA(H).
- Precision Approach: The final approach phase in precision approaches starts at the FAP, when to aircraft intercepts the GS and starts the descent towards DA(H). Outer marker and DME fixes can be published for altitude checks.

### APV: DA(H) and FAP on Baro-VNAV non-precision approaches

- Per ICAO Doc 8168 Vol. 1, Section 4, Chapter 1:

![[image.png]]

- Baro-VNAV approaches use the barometric altimeter information from the aircraft to follow a determined descent path toward the runway on the final approach phase. Since the real height flown by the aircraft when referencing the barometric altimeter is highly dependent on the actual OAT, it’s possible for the aircraft to starkly deviate from the intended flight path. Therefore, for Baro-VNAV approaches there are OAT limits published.
- Per ICAO Doc 8168 Vol. 1, Section 4, Chapter 1:

![[image 1.png]]

- The Vertical Guidance Sensitivity and tolerance per ICAO Doc 8168, Section 4, Chapter 1:

![[image 2.png]]

### FAA/NavCanada Differences and Peculiarities

- There’s a naming divergence between FAA and ICAO. ICAO names all these approaches as RNP since the requirements are actually performance based and not related to a specific type of equipment (Such as GPS). However, in the US and Canada most airports had procedures developed for general aviation use commonly named RNAV (GNSS) [id]. These procedures are usually based off GPS (sometimes with WAAS) as source of navigation since GA aircraft usually have only one IFR approved GPS receiver as single source of navigation outside of radio aids and don’t include IRS, DME-DME, etc. available to provide or improve navigation performance. The other subsequent procedures are usually named RNP (AR) [id] and are developed for use by more complex aircraft with a range of navigational equipment (usually airliners) and are Authorization Required procedures.
- FAA refuses to change their naming structure because ~~they are fascists~~ the changes would preclude too much “unnecessary costs”.
- There are different ways to fly these approaches depending on the approach type and available equipment: LNAV/VNAV, LNAV only (CDFA), LPV (Using WASS/EGNOS). Each of these allow for different minimums to be published by the state.
- VDA = Vertical Descent Angle for the approach. Jeppesen charts usually include VDA position/altitude tables either published by state or derived from VDA.
- GPA = Glide Path Angle. Usually present in LPV approaches with WAAS/EGNOS vertical guidance.

### Chart Examples

- An example from the chart 12-1 RNAV (GNSS) Z rwy 13 approach for CYWG showing in the profile view the GPA/VDA altitudes and distance/altitude table, FAF, and MAP. Note that there’s a DA(H) published for both the LPV and LNAV/VNAV procedures and a MDA(H) for the LNAV only procedure. The first two ones are VDAs while the last one is a normal NPA with FAF.

![[image 3.png]]

- An example from the chart 12-20 RNAV (RNP) Y rwy 13 approach for CYWG. This approach is published for the same RWY as the previous example, however this one does not require the use of GNSS as a primary navigation source and only requires the aircraft to be able to comply with the RNP 0.3. In the chart you can see that there is no FAF but a FAP published at 2200 ft at MESRO and the only minimums published is a DA(H) for a 3 degree straight in landing.

![[image 4.png]]

- Comparing these approaches we can observe the effectiveness of the GNSS system and how low (close enough to achieve the same operational minimums of an ILS approach in the LPV) the minimums can get when using the system.
- FAF vs FAP: The FAF is a **fix** determined in space (three dimensional) used for non-precision approaches to allow altitude-position cross check since non-precision approaches only provide azimuth guidance. The FAP is a point not determined in space, but when the aircraft starts it’s descent from the Intermediate phase of the approach into the final phase. Usually present in ILS/GLS/LPV approaches or non-precision approaches where there’s no way to establish a FAF (only one navaid already being used for a IAF/IF for example).
- An example from the chart 11-1 ILS or LOC rwy 4R for KMDW. The chart is valid for either an ILS CAT I or a LOC approach. You can see the FAF (for the LOC app) published at CITGO/2400’, which is the same altitude to be flown if you are flying the ILS CAT I approach, however the FAP in the ILS CAT I is whenever you capture the glide slope, leaving the Intermediate approach phase and starting your descent for the final approach phase. In this case, this can be anywhere from ALQUE to CITGO depending on ATM congestion. Again, there’s a DA(H) published for the ILS CAT I and a MDA(H) for the LOC. Note that the ILS CAT I DH in this case is 250 ft AGL, and we know that the operational procedure design DH for an ILS CAT I is 200 ft. The 50 extra feet in this DH are derived from the obstacle clearance requirements for the state (TERPS in the US) that surpassed the operational 200 ft DH. Also note that before the MAP for the precision approach there’s a VDP - Visual Descent Point published at 1.2 DME from IHKH identified by a stylized “V”. The VDP determines the point in the non-precision approach that a visual descent must be initiated to guarantee a stable standard 3 degree angle descent to cross the threshold at the TCH.

![[image 5.png]]

- Now an example from the chart 21-2 ILS or LOC rwy 9L for KORD:

![[image 6.png]]

On the plan view there are some points worthy of note. First the highest obstacle, identified by the bold arrow at 1508 ft to the right of the flight path. Second the black five-point star symbol to the left of the flight path - this indicates a hazard beacon. Third, there are numerous airports underlying the approach into O’Hare, identified by the grey circle with 6 chevrons (the star indicates that the airport has a beacon). In this specific approach, none of the the unidentified man-made obstacles are lighted.

On the profile view you can see the FAF for the LOC approach at ZENAH at 2300’, which is also the same altitude for the ILS CAT I approach to be flown at ZENAH. Again, the ILS CAT I has a FAP instead of a FAF defined at the point where the GS is captured, which can be anywhere from JHONN to ZENAH is this case (provided that the signal beam is strong enough). There’s an IM defined 0.3 NM from ISAJ for the ILS CAT I. For the LOC approach the VDP is defined at 1.0 NM from ISAJ and the MAP is at the RWY threshold, 0.1 NM from ISAJ. The MAP can also be determined by timing from ZENAH per the published timing table. This time, the DH for the ILS is equal to the nominal procedure operational DH for an ILS CAT I (no obstacle restrictions).

- Now the chart 21-2A ILS CAT II & III rwy 9L at KORD:

![[image 7.png]]

This approach is for the same runway and relies on the same navaid as the previous one, however there’s no LOC only approach and the procedure design minimums follow the CAT II & III parameters. You can see that there is no FAF published and the FAP is once again wherever you are cleared to capture the GS and start your final descent. Note that for CAT III There are no published DA(H) and as long as the RVR is greater than 600 ft (RVR 6) and the aircraft and crew are current the approach can be flown. For the CAT II the standard procedure design minimums of 100 ft DH are published along with the 1200 ft RVR.

- Now an example from the chart 13-1 VOR A for KBIS (No Runway Specified):

![[image 8.png]]

This is a VOR approach and does not make use or requires anything other than a working standard IFR radio navigation equipment suite to be flown (HSI, VOR CDI, RMI). This procedure is also not intended for a straight in approach for specific runway, but is rather a instrument approach that requires a circle to land after MDA is reached and/or visual contact with the field is stablished and can be maintained - stated by the “circle-to-land” on the minimums section and the white C inside a black diamond over the speed categories.

The procedures has three different IAFs: ODUFA and ODUBY are fixes defined by radial and DME readings from the BIS VOR and are the starting point of 7 NM DME arcs to intercept the final approach azimuth. The remaining IAF is the BIS VOR itself, which has a bold hold published to allow joining aircraft to intercept the final approach course. Note that the VOR acts both as a IAF and the FAF for the approach. Since this is not a straight in approach there’s not a VDP published and the MAP is defined by 2.9 DME from BIS or timing. There are 3 different MDA(H) published for the different approach categories.

- An example from the chart 21-1 ILS or LOC Z rwy 16 at YMML shows a FAF with a altitude for the LOC approach different from the altitude of the GS:

![[image 9.png]]

The GS interception at 3000’ is at 8.1 DME from IMS - that is, the FAP for the ILS CAT I and the FAF for the LOC is at 5.7 DME from IMS at 2100’, while the GS altitude for the same fix is at 2240’.

The [77LOC] is a database identifier for that position/pseudo fix.

- This is an example from the chart 13-1 VOR rwy 10 at CYZF:

![[image 10.png]]

This is a VOR approach with a standard left hand procedure turn with the maximum PT distance determined by DME, the descent point determined by DME and the MAP at YZF. There’s no FAF published for this approach (this fact is even stated in the briefing strip). Comparing with the state published chart you can see that there is no VDP published but rather a altitude/distance table for the final azimuth based on a 3 degree angle where 5.3 NM corresponds to the 2200’ recommended altitude during the intermediate approach phase. Therefore, Jeppesen does not publish the FAP or VDP in the chart.

![[image 11.png]]

- Another example from the chart 12-10 RNAV (GPS) X rwy 31 at KLGA:

![[image 12.png]]

The approach name, in a FAA fashion, states that this is a RNAV approach that requires GPS signal to be flown. Note that the chart doesn’t state any PBN requirements like RNP, RF and assumes basic terminal GNSS performance. The FAF is at GACAR at 2200’ and there is no vertical guidance such as VNAV or LPV(WAAS), so only a MDA(H) is published for all categories. After the FAF the descent angle is a non-standard 3.20 degrees and after the MAP the are two other altitude check GPS waypoints even though the visual contact with the ground is already stablished at this stage.