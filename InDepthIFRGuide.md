# **Universal In-Depth IFR Guide**

Chronological workflow for Instrument Flight Rules (IFR) Flights, generalized for various aircraft types and variants.


## 1. Pre-Flight Preparation and Ground Setup

### 1.1 Meteorological and Flight Planning
- **Weather Minima:** Check actual meteorological conditions at the departure, destination, and alternate aerodromes to ensure they meet operational minima. EASA enforces strict Aerodrome Operating Minima (AOM), which are determined by the aircraft's approach category, the available ground lighting facilities, and the precision of the navigation equipment.
  - *Aircraft Categories and Minima Application:* Aircraft approach categories are established based on the indicated airspeed at the runway threshold ($V_{AT}$). This speed is calculated as 1.3 times the stalling speed ($V_{S0}$) in the maximum certificated landing configuration.
    
    | Aircraft Category | $V_{AT}$ Range | Typical Aircraft Classifications |
    | :--- | :--- | :--- |
    | Category A | Less than 91 kt | Light single-engine (e.g., C172), light twins |
    | Category B | 91 kt to 120 kt | Multi-engine pistons (e.g., PA-34), light turboprops |
    | Category C | 121 kt to 140 kt | Mid-size corporate jets, short-haul airliners |
    | Category D | 141 kt to 165 kt | Large transport category aircraft |
    | Category E | 166 kt to 210 kt | Specialized high-speed military or transport |

  - *Straight-in Approaches:* The required Runway Visual Range (RVR) or visibility is a function of the Decision Height (DH) or Minimum Descent Height (MDH) and the available approach lighting systems (from Full Approach Lighting Systems [FALS] to No Approach Lighting Systems [NALS]).

    | DH or MDH (ft) | FALS (RVR m) | IALS (RVR m) | BALS (RVR m) | NALS (RVR m) |
    | :--- | :--- | :--- | :--- | :--- |
    | 200–210 | 550 | 750 | 1,000 | 1,200 |
    | 211–240 | 550 | 800 | 1,000 | 1,200 |
    | 241–250 | 550 | 800 | 1,000 | 1,300 |
    | 251–260 | 600 | 800 | 1,100 | 1,300 |
    | 261–280 | 600 | 900 | 1,100 | 1,300 |

- **Alternates:** Select suitable take-off and destination alternates equipped with conventional navaids in case of GNSS failure, ensuring you are not solely reliant on satellite-based guidance. 
  - *Alternate Selection (EASA):* Under EASA Part-NCO (Non-Commercial Operations), the selection of destination alternates is mandatory unless specific, stringent meteorological criteria are met. An alternate is not required if the destination is an isolated aerodrome, or if the forecast weather from one hour before to one hour after the Estimated Time of Arrival (ETA) indicates visual meteorological conditions (VMC) featuring a ceiling of at least 2,000 ft (or circling height plus 500 ft, whichever is greater) and a ground visibility of at least 5 km. SideNote: Commercial Air Transport (Part-CAT) operations enforce much stricter alternate requirements, often mandating two destination alternates if the weather falls below specific thresholds or if meteorological information is unavailable.
- **NOTAMs:** Review standard NOTAMs, SBAS NOTAMs (for Satellite-Based Augmentation System availability like the European Geostationary Navigation Overlay Service EGNOS).

### 1.2 Equipment and GNSS Setup
To operate effectively within Performance-Based Navigation (PBN) environment, you should understand the underlying mechanisms of GNSS. These systems operate on the principle of one-way ranging. Because aircraft receivers lack atomic clocks, a minimum of four satellites is required to mathematically solve for three-dimensional position (latitude, longitude, altitude) and receiver clock bias.

- **GNSS Augmentation Systems:** Raw GNSS signals are subject to atmospheric interference, clock errors, and ephemeris errors (8 to 13 meters accuracy). To achieve the precision necessary for vertical approach guidance, augmentation is required:
  - *ABAS (Aircraft-Based Augmentation System):* Relies on onboard systems like Receiver Autonomous Integrity Monitoring (RAIM) to monitor signal integrity.
  - *SBAS (Satellite-Based Augmentation System):* Ground stations monitor GNSS errors and transmit corrective signals via geostationary satellites. SBAS enables Localizer Performance with Vertical guidance (LPV) approaches.
  - *GBAS (Ground-Based Augmentation System):* Ground stations at the aerodrome broadcast corrections via VHF data links, enabling ultra-precise CAT II/III equivalent approaches.
- **Database Check:** Verify that the aeronautical database is current (valid AIRAC cycle) and that intended approaches are selectable. Operating with an expired database prohibits the use of RNAV terminal procedures, as undocumented changes to waypoint coordinates or approach angles can lead to catastrophic terrain conflicts.
- **RAIM Prediction:** For non-SBAS receivers (or when SBAS is unavailable), perform a Receiver Autonomous Integrity Monitoring (RAIM) check to ensure satellite coverage is adequate from 15 minutes before to 15 minutes after ETA. While four satellites provide a 3D position, five satellites are required for Fault Detection (FD) to alert the crew of an error. Six satellites are required for Fault Detection and Exclusion (FDE), allowing the receiver to actively isolate the faulty satellite and continue navigating.
- **System Initialization:**
  - Monitor the auto-test function on start-up. (On electromechanical HSIs or digital CDIs, this is verified by a needle deflection and the sequential showing of warning flags).
  - Check system settings: CDI scaling set to 'automatic', correct map datum (e.g., WGS84), and appropriate units of measure.
  - Select display fields to show Desired Track (DTK), Groundspeed (GS), and Distance to next waypoint (DIS) if possible or check this information is accessible to you.
- **Radio Setup (NAV 1 / NAV 2):**
  - Set up the maximum number of navaids. If a procedure requires two, set and identify both. Set remaining required navaids on standby. Optimal radio management minimizes cognitive overload during high-workload phases. Try to "work backwards" from the destination approach to the en-route structure.
  - Generally, use NAV 2 as the primary en-route navigation source (initial arrival routing, or intercepting the final approach course) and NAV 1 for approach or assist navigation (primary approach facility). Setting this early prevents rushing to tune and identify frequencies during the descent.
  - Ensure no "red flags" are displayed on active instruments. Be cautious when switching frequencies to avoid losing needle indications and preventing a sudden, disorienting loss of guidance.
  - Avoid using two navaids to display the same thing. 

## 2. Take-Off Clearance and Briefing


### 2.0 EASA/ICAO Clearance Structures (CRAFT)
Prior to taxi, the flight crew must obtain an IFR clearance from Air Traffic Control (ATC). Standard ATC clearances globally utilize the same format to ensure no critical parameters are omitted. Pilots receive, copy, and read back clearances using the CRAFT acronym:
- **C - Clearance Limit:** The geographical point to which the aircraft is cleared (typically the destination aerodrome).
- **R - Route:** The initial departure routing, which is generally a Standard Instrument Departure (SID) or specific radar vectors.
- **A - Altitude:** The initial climb altitude or flight level (e.g., "Climb initially 5,000 feet").
- **F - Frequency:** The departure control radio frequency to contact immediately upon becoming airborne.
- **T - Transponder:** The 4-digit squawk code to identify the aircraft on the radar screen.

### 2.1 The Departure Briefing
The departure briefing must be completed before declaring ready for departure. It ensures situational awareness and compliance with standard procedures.
- **Identify:** Aerodrome name, approach plate date, and name of the SID/Runway in use.
- **Routing & Setup:** Review the take-off path, initial routing, and verify radio aid selections.
- **Restrictions:** Note any departure restrictions such as climb gradients, altitude caps, or speed limits.
- **Obstacle Clearance:** Note the Minimum Sector Altitude (MSA).
- **Contingencies & Emergencies:**
  - Check minimum climb gradients against aircraft performance charts (especially important for multi-engine aircraft evaluating one-engine-inoperative scenarios).
  - Determine the plan for an emergency (e.g., engine failure) in VMC vs. IMC. Priorities: 1. Fly the aircraft, 2. Navigate (proceed visually, follow SID, or divert to low MSA), 3. Communicate (declare emergency).

## 3. Standard Instrument Departure (SID) Procedures

### 3.1 Flying the Departure
- **Configuration:** Maintain standard speeds and configurations as dictated by the aircraft's specific Standard Operating Procedures (SOPs).
- **Tracking:** Utilize intercept techniques to join desired radials or courses.
- **Departures (Outbound):** Intercept angles are generally 45°. If the difference between the current course and desired course is less than 15°, apply the difference as the intercept angle. If it is a large turn (Offset Departure > 90°), fly the heading of the desired radial, wait until abeam the station, turn 45° towards the station, and intercept.
- **Monitoring:** Cross-check conventional navaids against GNSS displays to confirm navigational accuracy and mitigate the risks of automation-induced complacency or localized GPS jamming.


### 3.2 Take-Off Procedures and ATC Communications
Executing an instrument take-off requires the pilot flying (PF) to make an immediate, decisive transition from visual external cues to the internal instrument scan the moment the aircraft rotates. The scan utilizes the "hub-and-spoke" method, centered heavily on the Attitude Indicator to establish the initial pitch target, rapidly cross-checking the Airspeed Indicator, Altimeter, and Heading Indicator to confirm performance.

Standard ATC communications during departure under ICAO and EASA rules utilize precise phraseology to dictate altitude profiles. When cleared on a SID containing published altitude constraints, ATC will issue the command, "Climb via SID to Level". This instructs the crew to follow the lateral path and comply with all published intermediate vertical constraints up to the cleared level. Conversely, if ATC states "Climb unrestricted to Level," all intermediate altitude restrictions on the SID are cancelled, allowing a continuous climb. ATC instructions override published procedures but it does not hurt to ask if they are contradicting or over-ride any published restrictions. 

## 4. En-Route and Cruise Phase

### 4.1 Establishing Cruise
- **Power Settings:** Transition to the appropriate cruise power setting (Low, Medium, or High Cruise) per aircraft SOP.
- **Altitude Changes:** Unless dictated by ATC or obstacle clearance, establish a standard maximum rate of climb or descent (e.g., 500 to 1,000 ft/min) to transition between flight levels smoothly. This minimizes passenger discomfort and prevents Traffic Collision Avoidance System (TCAS) Resolution Advisories, which can be triggered by excessive vertical closure rates near the assigned altitude.
- **En-Route Communications:** In procedural (non-radar) airspace, accurate position reporting is essential. Standard phraseology dictates a specific sequence: Aircraft Identification, Position, Time, Flight Level, Next Position with ETA, and the Ensuing Significant Point.

### 4.2 Monitoring Progress and Clearances
- **Obstacle Clearance:** Ensure a minimum obstacle clearance of 600m (1969 ft) over high/mountainous terrain and 300m (984 ft) elsewhere.
- **RNP Specifications:** Modern airspace utilizes Required Navigation Performance (RNP) specifications, which define the accuracy required for a given segment. For example, RNP 1 requires the aircraft to remain within 1.0 Nautical Mile of the centerline for 95% of the flight time. Unlike older RNAV specifications, RNP requires onboard performance monitoring and alerting; if the navigational accuracy degrades beyond the RNP limit (e.g., due to satellite loss), the avionics will issue a Loss of Integrity (LOI) alert to the crew.
- **Altimeter Corrections:** Pressure altimeters are calibrated entirely to the International Standard Atmosphere (ISA). When the ambient temperature is significantly colder than ISA, the atmospheric pressure decreases more rapidly with altitude. Consequently, the altimeter will over-read, meaning the true altitude of the aircraft will be significantly lower than the indicated altitude, silently compromising terrain clearance.
  - Adjust minimum altitudes for temperature (add 4% for every 10°C below standard). More precisely, if the aerodrome temperature is 0°C or colder, corrections must be calculated and added to the Minimum Descent Altitude (MDA) or Decision Altitude (DA), as well as all step-down fixes inside the Final Approach Fix (FAF). These corrections are extracted from the ICAO Cold Temperature Error Table (Doc 8168). Pilots must advise ATC if they are applying temperature corrections to published intermediate altitudes to ensure ATC can maintain vertical separation standards.
  - Adjust for wind over mountainous terrain (add 500 ft for every 10 kts of wind above 30 kts, up to 2000 ft).


### 4.3 EASA En-Route Fuel Calculations (Part-NCO vs. Part-CAT)
Fuel planning in EASA airspace is heavily bifurcated based on the nature of the operation. Both Commercial Air Transport (Part-CAT) and non-commercial operations (Part-NCO) require the calculation of distinct fuel blocks, but the regulatory rigidity and specific reserve requirements differ significantly.

The fundamental structure of an IFR fuel plan consists of the following blocks:

| Fuel Block | Description | Calculation Basis |
| :--- | :--- | :--- |
| **Taxi Fuel** | Fuel consumed prior to takeoff. | Fixed allowance based on typical ground delays and APU usage. |
| **Trip Fuel** | Fuel required from departure to the destination. | Includes climb, cruise, descent, and the instrument approach. |
| **Contingency** | Fuel to compensate for unforeseen factors. | Varies by regulation (Part-CAT vs. Part-NCO). |
| **Alternate** | Fuel to execute a missed approach and fly to the alternate. | Missed approach, climb, cruise, descent, and landing at alternate. |
| **Final Reserve** | The inviolable, protected fuel reserve. | Varies by engine type and regulation. |
| **Extra Fuel** | Discretionary fuel added by the PIC. | Must account for maximum structural takeoff mass. |

- **Contingency Fuel Differences:** Under Part-CAT, contingency fuel is strictly defined, most commonly as 5% of the planned trip fuel, or the fuel required to fly for 5 minutes at holding speed at 1,500 ft above the destination, whichever is greater. Part-NCO is more performance-based; while it lacks a rigid statutory percentage for contingency, the Pilot-in-Command (PIC) is legally mandated to account for expected deviations, winds, and delays, making 5% a standard operational best practice.
- **Final Reserve Fuel Differences:** The Final Reserve is the absolute minimum fuel required upon touchdown. If a pilot calculates in-flight that they will land with less than the Final Reserve, they are legally obligated to declare a "MAYDAY FUEL" emergency to secure immediate priority handling.

### 4.4 Emergency Procedures: Loss of Communications (SERA.14083)
A loss of two-way radio communications (RCF) while operating in IMC presents a highly complex emergency. The procedures for operating with RCF in European airspace were profoundly updated via the Standardised European Rules of the Air (SERA.14083), becoming effective in May 2025.
- **Transponder Codes:** If standard troubleshooting fails to restore contact, the crew must rely on transponder codes to broadcast their state (squawk 7600).
- **Routing:** If the failure occurs in IMC, adhere to a strict routing protocol (often summarized by the acronym AVE-F):
  1. **Assigned:** Fly the route last assigned by ATC.
  2. **Vectored:** If on radar vectors, fly direct to the fix, route, or airway specified in the vector clearance.
  3. **Expected:** Fly the route ATC advised to expect in a further clearance.
  4. **Filed:** Fly the route filed in the flight plan.
- **The New 20-Minute Rule:** Under the updated SERA.14083, the previous distinction between radar (7 minutes) and non-radar environments has been entirely eliminated. An IFR flight must now maintain the last assigned speed and level (or the minimum flight altitude, if higher) for a period of 20 minutes following the aircraft's failure to make a required report, or the moment the transponder is set to 7600. Following the expiration of the 20-minute period, the aircraft adjusts its altitude and speed in accordance with the filed flight plan, ultimately commencing descent and executing the approach at the destination as close to the expected time of arrival (ETA) as possible.

## 5. Arrival and STAR Procedures
The arrival phase systematically transitions the aircraft from the high-altitude en-route structure into the terminal environment, typically via a Standard Terminal Arrival Route (STAR).

### 5.1 Top of Descent (TOD) Calculation
Calculate the TOD to reach the Minimum Holding Altitude (MHA) at the Initial Approach Fix (IAF). Efficient kinetic energy management requires you to accurately calculate this to ensure correct airspeed.
- **By Distance:** Altitude to lose divided by 1000, multiplied by 3 (e.g., to lose 3,500 ft: 3.5 x 3 = 10.5 NM prior to fix).
- **By Rate of Descent (3° glide):** Half of the Groundspeed multiplied by 10 (e.g., 100 kts GS / 2 = 50 x 10 = 500 fpm).
- **Deceleration Calculation:** As a rule of thumb for deceleration, crews should add 1 NM of level flight for every 10 knots of airspeed that must be reduced prior to the IAF.

### 5.2 The Descent Briefing
This must be completed before reaching the TOD to ensure the you remain cognitively ahead of the aircraft:
1. **STAR/Routing:** Review the STAR (aerodrome, plate date, identifier, routing, and altitude restrictions) or radial/MSA to the IAF.
2. **Expected Approach:** Identify the planned approach.
3. **Transition Level:** Brief the transition level to ensure timely QNH setting and prevent altitude busts.
4. **MSA/TAA:** Review the Minimum Sector Altitude or Terminal Arrival Altitude (which replaces the MSA and provides 1,000 ft of obstacle clearance or 2,000 ft in mountainous areas within a 25 NM radius of the IAF).
5. **Weather:** Confirm ceiling/visibility are above minima for straight-in or circling.
6. **TOD Check:** Specify the TOD distance relative to the relevant navaid.
7. **Fuel & Alternates:** Verify remaining fuel is sufficient for a diversion, ensuring the Final Reserve (45 minutes) will remain completely intact upon touchdown.

**ATC Communications:** When ATC issues an arrival clearance, the phraseology "Descend via STAR to Level" mandates that you manage the descent to strictly comply with all intermediate published altitude and speed constraints on the arrival.

## 6. Approach Procedures

### 6.1 Understanding Approach Types
Instrument approaches are fundamentally classified by the type of electronic guidance they provide:
- **2D Approaches (Non-Precision):** Provide lateral guidance only (e.g., LNAV, LP, VOR, NDB, LOC). Vertical path is managed by the pilot via mathematics or step-down fixes. Often flown using a Continuous Descent Final Approach (CDFA) technique, converting Minimum Descent Altitude (MDA) into a Decision Altitude (DA).
  - *CDFA and DDA:* Historically, 2D approaches were flown using the "dive and drive" method—descending rapidly to the MDA, levelling off, and flying horizontally toward the MAPt. EASA and ICAO now strongly mandate the CDFA technique for 2D approaches. CDFA simulates a 3D glidepath by calculating a continuous rate of descent from the FAF directly to the runway threshold. Because the aircraft is descending continuously under CDFA, treating the MDA as a DA would result in the aircraft breaching the hard MDA floor during the go-around maneuver. To prevent this, operators add a margin (typically 50 feet) to the published MDA, creating a Derived Decision Altitude (DDA). The go-around is initiated precisely at the DDA.
- **3D Approaches (APV/Precision):** Provide both lateral and vertical guidance electronically by ground transmitters or augmented satellites (e.g., ILS, GLS, LNAV/VNAV, LPV).

### 6.2 The Approach Briefing
Must be completed before reaching the IAF:
1. **Chart Identification:** Confirm plate and date.
2. **Airport Elevation:** Establishes the altitude for stabilized approach criteria.
3. **Navaid Selection:** Set active and standby frequencies on NAV 1/2 to anticipate changes and reduce workload.
4. **Procedure Review:**
  - *Horizontal:* Holding radial/entry, IAF, IF, FAF distances, and inbound courses.
  - *Vertical:* Minimum altitudes for all fixes, glide slope check altitudes, and continuous Rate of Descent calculation.
5. **Minima:** State the DA or MDA for straight-in or circling.
6. **Missed Approach:** Review the exact missed approach procedure.

*Approach Terminology Definitions:*
- **IAF (Initial Approach Fix):** The point where the initial approach segment begins, transitioning the aircraft from the en-route structure to the approach procedure.
- **IF (Intermediate Fix):** The point where the intermediate segment begins, utilized to align the aircraft with the final approach course and configure for landing.
- **FAF / FAP (Final Approach Fix / Point):** The point where the final approach segment begins, and the final descent to the runway commences.
- **MAPt (Missed Approach Point):** For a 2D approach, this is the geographic point (often a DME distance or navaid) at which the missed approach must be initiated if the runway is not in sight. For a 3D approach, the MAPt is the physical point in space where the glidepath intersects the DA.
- **AAL (Above Aerodrome Level):** Altitude expressed relative to the elevation of the aerodrome, critical for determining the height at which the aircraft must be stabilized.

### 6.3 Flying the Approach Segments
- **Arrival Segment:** Reduce to approach speed approximately 2 minutes before the IAF.
- **Initial/Intermediate Segment:**
  - Verify the procedure is correctly loaded and activated in the GNSS receiver.
  - Configure aircraft (e.g., approach flaps) 1.5 NM prior to the FAF.
  - Extend landing gear and perform pre-landing checks 1.0 NM prior to the FAF (or at 1 dot below glideslope for 3D approaches).
- **Final Approach Segment:**
  - Monitor CDI/HSI scaling (automatically increases sensitivity on GNSS approaches).
  - For 2D approaches, adhere strictly to step-down fixes before reaching MDA.
  - For 3D approaches, maintain within half-scale deviation of lateral and vertical paths.

### 6.4 Stabilized Approach Criteria
A stabilized approach is the aviation industry's primary defense against Controlled Flight Into Terrain (CFIT) and runway excursions. An approach is stabilized, and may continue, if the following are met by 1,000 ft AAL (IMC) or 300 ft AAL (VMC) [or 500 ft AAL in VMC according to some operators]:
- Landing gear down and locked.
- Flaps selected for landing.
- Landing checklists complete.
- Power setting appropriate (above idle).
- Bank angle not exceeding 10°.
- Speed between VREF and VREF + 10 kts (corrected for wind) [or up to + 20 kts adjusted for wind gusts].
- Rate of descent not exceeding 1,000 fpm.
- Lateral/Vertical deviation within 1 dot (Precision) or +/- 5° (Non-Precision).
- If unstabilized below these altitudes, an immediate go-around is mandatory.

### 6.5 Holding and Course Reversals
If an aircraft approaches an IAF from an angle that prohibits a direct turn onto the approach course, a formal course reversal is required.
- **Holding Entries:** Based on a 70°/110°/180° sector model (Parallel, Offset/Teardrop, Direct) with a 5° flexibility margin.
- **Holding Timing & Wind Correction:**
  - Adjust the outbound leg time so the inbound leg takes exactly 1 minute (or 1.5 min above 14,000 ft).
  - Wind drift: Apply three times the inbound drift correction to the outbound leg (the "rule of three" to ensure the aircraft remains within the protected airspace).
- **DME Arcs:** Turn 90° to the radial to enter. Turn 10° periodically to maintain the arc (adjusting the heading by 10° every time the bearing pointer drifts 10° past the wingtip). Anticipate joining/leaving the arc using turn radius calculations based on groundspeed (the 60:1 rule). If groundspeed indication is unavailable, a standard 1.0 NM lead distance for high-performance aircraft, or a 0.5 NM lead for light aircraft, serves as a safe alternative.

### 6.6 Deciphering Approach Plates (Jeppesen)
Accurately interpreting approach charts is a critical skill. Jeppesen charts, the gold standard in aviation, are highly structured into four primary geographic sections to facilitate rapid data extraction.
- **Header:** Contains administrative, communication, and primary procedural data. It lists communication frequencies in the chronological order of use (ATIS, Approach, Tower, Ground). The central briefing block is paramount; it isolates the primary navaid frequency, the final approach course, the DA/MDA, the Airport Elevation (the highest point of the usable landing area), and the Touchdown Zone Elevation (TDZE).
- **Plan View:** Provides a top-down, horizontal representation of the procedure. It displays the lateral routing from the IAF, through the Intermediate Fix (IF), to the FAF. It illustrates holding patterns, course reversals (procedure turns), the MSA or TAA, and highlights significant topographical terrain or isolated obstacles.
- **Profile View:** Represents the vertical path of the approach. It details the minimum altitudes for every segment.
- **Minima Section:** Located at the bottom, this section outlines the required Decision Altitude (DA) or Minimum Descent Altitude (MDA), along with the required visibility or RVR. Minima are segmented horizontally by aircraft approach category (A, B, C, D) and specify whether the approach authorizes straight-in landing or requires a circling maneuver.

### 6.7 Conventional Approach Techniques and Geometry
While GNSS approaches dominate modern IFR, proficiency in conventional navigation remains a regulatory requirement and a critical fail-safe.
- **Instrument Landing System (ILS) - 3D:** The ILS provides the highest precision of conventional approaches. The localizer provides highly sensitive lateral guidance, while the glideslope provides vertical guidance, typically at a 3.0° angle. The crew intercepts the localizer (usually at a 30° angle) using NAV 2 or heading mode, ensuring the CDI needle begins to center before engaging the approach mode. The glideslope must always be intercepted from below to prevent the autopilot from capturing a false, steeper glideslope lobe reflecting off the ground.
- **VOR and NDB Approaches - 2D:** VOR approaches rely on tracking specific VHF radials. Because VOR signals diverge outward from the station, the sensitivity of the CDI increases dramatically as the aircraft approaches the transmitter. NDB (Non-Directional Beacon) approaches, flown using an Automatic Direction Finder (ADF), are the least accurate. The ADF needle simply points to the station; it does not track a beam. Pilots must continuously calculate wind drift to fly a specific track (a QDM to the station, or a QDR from the station). NDBs are highly susceptible to errors such as coastal refraction, terrain shielding, and thunderstorm interference.

### 6.8 Missed Approach Procedures and Go-Around Philosophy
The missed approach is a highly demanding maneuver requiring an immediate, aggressive transition from a low-energy descent to a high-energy climb. The psychological readiness to execute a go-around must be firmly established during the approach briefing to combat "plan continuation bias."
- **Execution Procedure:** ICAO Doc 8168 designs missed approach procedures assuming a nominal climb gradient of 2.5%. If an aircraft cannot meet this gradient (e.g., due to an engine failure, icing, or heavy gross weight), the approach cannot be safely flown in IMC, and an alternative destination must be sought.

