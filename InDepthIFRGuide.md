# **Universal In-Depth IFR Guide**

Chronological workflow for Instrument Flight Rules (IFR) Flights, generalized for various aircraft types and variants.

## 1. Pre-Flight Preparation and Ground Setup

### 1.1 Meteorological and Flight Planning
- **Weather Minima:** Check actual meteorological conditions at the departure, destination, and alternate aerodromes to ensure they meet operational minima.
// Add EASA IFR minimas for different airspaces as Table
- **Alternates:** Select suitable take-off and destination alternates equipped with conventional navaids in case of GNSS failure.
// Add a little note explaining what GNSS is
- **NOTAMs & NANUs:** Review standard NOTAMs, SBAS NOTAMs (for Satellite-Based Augmentation System availability), and Notices to Navstar Users (NANUs) for scheduled outages or interference.
// Never heard of NANU’s where did you find this information? If it is in the SOP’s then leave it here but add some context what it is and where to find the information needed.. 

### 1.2 Equipment and GNSS Setup
- **Database Check:** Verify that the aeronautical database is current (valid AIRAC cycle) and that intended approaches are selectable.
// How to check the databases? Should be when the GPS starts that it displays the cycle right? 
- **RAIM Prediction:** For non-SBAS receivers (or when SBAS is unavailable), perform a Receiver Autonomous Integrity Monitoring (RAIM) check to ensure satellite coverage is adequate from 15 minutes before to 15 minutes after ETA.
// again how to do this? Usually within the GPS system look for the RAIM prediction.. 
- **System Initialization:**
  - Monitor the auto-test function on start-up.
  // usually a needle deflection that you can see on the instrument
  - Check system settings: CDI scaling set to 'automatic', correct map datum (e.g., WGS84), and appropriate units of measure.
  //how to check and what exactly should it be set to? 
  - Select display fields to show Desired Track (DTK), Groundspeed (GS), and Distance to next waypoint (DIS).
 // on standard garmin devices this is hard to do and adjust. Maybe just checking that the information is reasonable correct should be good? 
- **Radio Setup (NAV 1 / NAV 2):**
  - Set up the maximum number of navaids if possible, at least the first two to be used. If a procedure requires two, set and identify both. Set remaining required navaids on standby.
  - Generally, use NAV 2 as the primary en-route navigation source and NAV 1 for approach or assist navigation.
  - Ensure no "red flags" are displayed on active instruments. Be cautious when switching frequencies to avoid losing needle indications. // Always have one instrument set to be followed while you adjust the next instrument. Work “backwards” for the setup from the approach on NAV1 to the intercept on NAV2 before that etc.. 

## 2. Take-Off Clearance and Briefing

### 2.1 The Departure Briefing
The departure briefing must be completed before declaring ready for departure. It ensures situational awareness and your setup and understanding of the procedure.
- **Identify:** Aerodrome name, approach plate date, and name of the SID/Runway in use.
- **Routing & Setup:** Review the take-off path, initial routing, and verify radio aid selections. // Vertical and Horizontal turns and climbs / descends and altitude changes 
- **Restrictions:** Note any departure restrictions such as climb gradients, altitude caps, or speed limits. // look for side marks and restrictions 
- **Obstacle Clearance:** Note the Minimum Sector Altitude (MSA). 
- **Contingencies & Emergencies:**
  - Check minimum climb gradients against aircraft performance charts (especially important for multi-engine aircraft evaluating one-engine-inoperative scenarios). // note it down if applicable to tell ATC you can or cannot comply 
  - Determine the plan for an emergency (e.g., engine failure) in VMC vs. IMC. Priorities: 1. Fly the aircraft, 2. Navigate (proceed visually, follow SID, or divert to low MSA), 3. Communicate (declare emergency).

## 3. Standard Instrument Departure (SID) Procedures

### 3.1 Flying the Departure
- **Configuration:** Maintain standard speeds and configurations as dictated by the aircraft's specific Standard Operating Procedures (SOPs).
- **Tracking:** Utilize intercept techniques to join desired radials or courses.
- **Departures (Outbound):** Intercept angles are generally 45°. Use Company rules to intercept if needed. 
- **Monitoring:** Cross-check conventional navaids against GNSS displays to confirm navigational accuracy.


## 4. En-Route and Cruise Phase

### 4.1 Establishing Cruise
- **Power Settings:** Transition to the appropriate cruise power setting (Low, Medium, or High Cruise) per aircraft SOP.
- **Altitude Changes:** Unless dictated by ATC or obstacle clearance, establish a standard maximum rate of climb or descent (e.g., 500 ft/min) to transition between flight levels smoothly.

### 4.2 Monitoring Progress and Clearances
- **Obstacle Clearance:** Ensure a minimum obstacle clearance of 600m (1969 ft) over high/mountainous terrain and 300m (984 ft) elsewhere. // where did you find this information? 
- **Altimeter Corrections:**
  - Adjust minimum altitudes for temperature (add 4% for every 10°C below standard).
  - Adjust for wind over mountainous terrain (add 500 ft for every 10 kts of wind above 30 kts, up to 2000 ft).
 
    

## 5. Arrival and STAR Procedures

// Add standard Terminology explanations like what stages are there to an approach and what are they called and from where to where are they. What’s the difference between MDA and DA and height and altitudes etc.. Standard mistakes and missing information for students to avoid. 

### 5.1 Top of Descent (TOD) Calculation
Calculate the TOD to reach the Minimum Holding Altitude (MHA) at the Initial Approach Fix (IAF).
- **By Distance:** Altitude to lose divided by 1000, multiplied by 3 (e.g., to lose 3,500 ft: 3.5 x 3 = 10.5 NM prior to fix).
- **By Rate of Descent (3° glide):** Half of the Groundspeed multiplied by 10 (e.g., 100 kts GS / 2 = 50 x 10 = 500 fpm).

### 5.2 The Descent Briefing
This must be completed before reaching the TOD:
1. **STAR/Routing:** Review the STAR (aerodrome, plate date, identifier, routing, and altitude restrictions) or radial/MSA to the IAF.
2. **Expected Approach:** Identify the planned approach.
3. **Transition Level:** Brief the transition level to ensure timely QNH setting.
4. **MSA/TAA:** Review the Minimum Sector Altitude or Terminal Arrival Altitude.
5. **Weather:** Confirm ceiling/visibility are above minima for straight-in or circling. // add what exactly to check and where to find minimums or what are the regulatory EASA minimums
6. **TOD Check:** Specify the TOD distance relative to the relevant navaid.
7. **Fuel & Alternates:** Verify remaining fuel is sufficient for a diversion. // need more information how to exactly find out and calculate this 

## 6. Approach Procedures

### 6.1 Understanding Approach Types
- **2D Approaches (Non-Precision):** Provide lateral guidance only (e.g., LNAV, LP, VOR, NDB). Often flown using a Continuous Descent Final Approach (CDFA) technique, converting Minimum Descent Altitude (MDA) into a Decision Altitude (DA). // why MDA and not DA? 
- **3D Approaches (APV/Precision):** Provide both lateral and vertical guidance (e.g., ILS, LNAV/VNAV, LPV).

//make a table of the approaches and their guidance as well as which are the most accurate in each category etc..

### 6.2 The Approach Briefing
Must be completed before reaching the IAF: // IAF not explained 
1. **Chart Identification:** Confirm plate and date.
2. **Airport Elevation:** Establishes the altitude for stabilized approach criteria. // Airport Elevation is the elevation of the airport or not? 
3. **Navaid Selection:** Set active and standby frequencies on NAV 1/2 to anticipate changes and reduce workload.
4. **Procedure Review:**
  - *Horizontal:* Holding radial/entry, IAF, IF, FAF distances, and inbound courses.
  - *Vertical:* Minimum altitudes for all fixes, glide slope check altitudes, and continuous Rate of Descent calculation.
5. **Minima:** State the DA or MDA for straight-in or circling. // When to use which the DA or the MDA..
6. **Missed Approach:** Review the exact missed approach procedure. // stress again on the procedure of how to preform a go around in an emergency or the philosophy how to deal step by step with an emergency here 

### 6.3 Flying the Approach Segments
- **Arrival Segment:** Reduce to approach speed approximately 2 minutes before the IAF. // Times are difficult to maintain in the cockpit - distances would be better. Maybe we can add a quick calculation or estimate how many miles before and to what speed we should reduce. No specific speed but a guide how to know what is a good reference speed etc.. 
- **Initial/Intermediate Segment:**
  - Verify the procedure is correctly loaded and activated in the GNSS receiver. // clarify what a GNSS receiver is and where to find it or search for one in an aircraft.. 
  - Configure aircraft (e.g., approach flaps) 1.5 NM prior to the FAF. // FAF needs to be explained and shown how to find it on the plate.. 
  - Extend landing gear and perform pre-landing checks 1.0 NM prior to the FAF (or at 1 dot below glideslope for 3D approaches).
- **Final Approach Segment:**
  - Monitor CDI/HSI scaling (automatically increases sensitivity on GNSS approaches). // how exactly to do this? What to look for at the instrument? 
  - For 2D approaches, adhere strictly to step-down fixes before reaching MDA. // what are step down fixes? 
  - For 3D approaches, maintain within half-scale deviation of lateral and vertical paths.

### 6.4 Stabilized Approach Criteria
An approach is stabilized, and may continue, if the following are met by 1,000 ft AAL (IMC) or 300 ft AAL (VMC): // AAL needs to be explained 
- Landing gear down and locked.
- Flaps selected for landing.
- Landing checklists complete.
- Power setting appropriate (above idle).
- Bank angle not exceeding 10°.
- Speed between VREF and VREF + 10 kts (corrected for wind).
- Rate of descent not exceeding 1,000 fpm.
- Lateral/Vertical deviation within 1 dot (Precision) or +/- 5° (Non-Precision).
- If unstabilized below these altitudes, go-around is mandatory.

### 6.5 Holding and Course Reversals
- **Holding Entries:** Based on a 70°/110°/180° sector model (Parallel, Offset/Teardrop, Direct) with a 5° flexibility margin.
- **Holding Timing & Wind Correction:**
  - Adjust the outbound leg time so the inbound leg takes exactly 1 minute (or 1.5 min above 14,000 ft).
  - Wind drift: Apply three times the inbound drift correction to the outbound leg.
- **DME Arcs:** Turn 90° to the radial to enter. Turn 10° periodically to maintain the arc. Anticipate joining/leaving the arc using turn radius calculations based on groundspeed. // put the calculation here how to anticipate the leaving or joining of the arc. Also add an estimation of the calculation without ground speed.. as some aircraft’s have no GS indicated

## Gap Analysis & Research Plan
To complete this guide, research is required on the following topics:

1. **Clearance Structures:**
   - Standard ATC IFR clearance formatting (e.g., the CRAFT acronym: Clearance limit, Route, Altitude, Frequency, Transponder code).
2. **Detailed Take-Off Procedures & Comms:**
   - Step-by-step instrument take-off scanning and standard ATC communications during departure.
3. **En-Route Fuel Calculations:**
   - Standard formulas for calculating IFR fuel requirements (Trip, Contingency, Alternate, Final Reserve).
4. **En-Route and STAR ATC Communications:**
   - Standard phraseology for position reporting, level changes, and receiving STAR clearances.
5. **Emergency Procedures:**
   - Specific IFR communication protocols during emergencies (loss of comms / squawk 7600 procedures during SID, Cruise, and STAR).
6. **Reading Approach Plates:**
   - A deep dive into deciphering Jeppesen or FAA approach plates (header, plan view, profile view, minima section).
7. **Conventional Approach Techniques:**
   - Detailed, step-by-step guidance on flying specific conventional approaches (ILS, VOR, NDB) beyond the GNSS focus of the current documents.
  
     Also review my remarks and notes preceded by // and research as well as add the information requested. 
