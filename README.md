# BandgapReference--BGR-Layout-Design- Cadence Virtuoso Flow
### Technology: UMC 180nm 
### Tool: Cadence Virtuoso
Designed and implemented the physical layout of a Bandgap Reference (BGR) circuit with a strong focus on precision, matching, and noise performance. The layout ensures stable and temperature-independent reference voltage generation through careful symmetry techniques.

### Schematic Design (From the designer) 
o Designed a Bandgap Reference (BGR) circuit in the Schematic Editor to generate a stable, temperature-independent reference voltage.
o Incorporated key building blocks including matched BJTs, current mirrors, start-up circuit, and proportional-to-absolute-temperature (PTAT) and complementary-to-absolute-temperature (CTAT) components.
o Proper device sizing and biasing were implemented to ensure accurate current distribution and thermal compensation.
o Verified schematic connectivity, node biasing, and operating point to ensure correct functionality.
o Prepared and saved the schematic for simulation and subsequent layout implementation.


![BandgapReference schematic](https://github.com/Deepthi-S-G/Bandgap-Reference-BGR-Layout-Design-/blob/main/Band%20Gap%20Reference%20schrematic.png)


# Implementation Steps of Layout
### 1. Floor planning
o Created a structured floorplan by dividing the layout into functional blocks (BJT core, current mirrors, resistor network, and biasing circuitry).
o Ensured symmetrical arrangement of BJTs to maintain matching and temperature stability.
o Allocated dedicated regions for power rails (VDD, VSS) and sensitive analog nodes.
o Reserved spacing for routing and shielding to minimize interference.

![BandgapReference Floorplan](https://github.com/Deepthi-S-G/Bandgap-Reference-BGR-Layout-Design-/blob/main/Band%20Gap%20Reference%20floorplan.png) 


### 	2. Device Placement 
o Placed BJTs in common-centroid configuration to reduce mismatch due to process variations.
o Arranged resistors using interdigitated structures for accurate ratio matching.
o Positioned current mirrors and bias circuits close to reduce routing complexity.
o Maintained symmetry and proximity for all matched devices to improve precision.
![BandgapReference Placement](https://github.com/Deepthi-S-G/Bandgap-Reference-BGR-Layout-Design-/blob/main/Band%20Gap%20Reference%20%20PLACEMENT.png) 


### 3. Routing
o Performed manual routing using metal layers (M1–M5) ensuring minimal parasitic effects.
o Used wide metal paths for power lines to reduce IR drop.
o Applied shielding (ground lines) around sensitive nodes like Vref to reduce noise coupling.
o Inserted vias and contacts carefully while maintaining DRC-compliant spacing.
![BandgapReference Routing](https://github.com/Deepthi-S-G/Bandgap-Reference-BGR-Layout-Design-/blob/main/Band%20Gap%20Reference%20Routing.png) 



### 4. DRC (Design Rule Check)
o Performed DRC verification using Cadence Assura.
o Ensured all layout geometries follow foundry design rules.
o Achieved zero DRC errors, confirming manufacturability.

![BandgapReferencer DRC ](https://github.com/Deepthi-S-G/Bandgap-Reference-BGR-Layout-Design-/blob/main/Band%20Gap%20Reference%20DRC.png) 

### 5.LVS (Layout Versus Schematic) 
o Ran LVS to verify equivalence between schematic and layout.
o Confirmed no mismatches in nets, pins, or devices.
o Ensured layout accurately represents the designed BGR circuit.
![BandgapReference LVS ]() 

### 6.Parasitic Extraction (PEX) 
o Extracted parasitic resistances and capacitances from the layout.
o Generated extracted netlist for post-layout simulations.
o Evaluated the impact of parasitics on reference voltage stability and performance

## Outcome
o Successfully implemented a Bandgap Reference (BGR) layout with high precision and proper matching techniques.
o Ensured zero DRC errors and LVS clean results, confirming layout correctness and manufacturability.
o Minimized noise and mismatch using common-centroid layout, interdigitation, and shielding techniques.
o Generated an extracted netlist (PEX) for reliable post-layout simulation and performance validation.
o The layout is optimized for low variation, high stability, and robust analog performance.



