# Light-Theme Industrial Biorefinery Twin: Photorealistic Visualization & Inside-Workflow Engineering

## Executive Overview
Following the successful deployment of the standalone 3D digital twin and interactive click inspection, this phase upgrades the entire virtual solution into a **modern, light-theme industrial engineering SCADA suite** (inspired by Siemens TIA Portal, Rockwell Automation FactoryTalk, and clean CAD engineering dashboards), incorporating **photorealistic 3D object visualization** and **detailed inside-workflow cutaways** that display the real-world physical and biochemical phenomena occurring inside each processing unit.

---

## User Review Required

> [!IMPORTANT]
> **Light-Theme Industrial Aesthetics Baseline**:
> - We will transition the default visual theme from the dark slate palette to a crisp, high-contrast **Industrial Cleanroom / SCADA Light Theme**:
>   - Background: Clean architectural concrete / off-white canvas (`#f1f5f9` / `#f8fafc`).
>   - Dashboard panels: Crisp white surfaces (`#ffffff`) with subtle brushed steel borders (`#cbd5e1`), sharp high-contrast typography (`#0f172a`), and industrial cyan/teal/emerald telemetry accents.
>   - 3D Environment: Soft daylight ambient lighting, crisp contact shadows, epoxy factory flooring with safety yellow walkway striping and equipment boundary zones.
>   - User retains a 1-click toggle to switch back to Dark SCADA or X-Ray Piping mode at any time.

> [!NOTE]
> **Inside-Workflow Cutaway Enhancements**:
> Every unit will feature an interior inspection cutaway showing active mechanical and biochemical mechanisms:
> 1. **Whey Unloading & Pasteurizer**: Flexible tanker unloading hose with pulsing fluid, raw whey silo liquid level sight glass, and cutaway plate heat exchanger with hot/cold counter-current flow streams.
> 2. **Fermenter Vessel**: Transparent viewport showing rotating dual 6-blade Rushton turbine impellers creating a fluid vortex, internal helical cooling coil, rising fermentation gas bubbles, and automated pH base dosing droplets.
> 3. **Recovery & BMED**: Cutaway distillation column showing horizontal bubble-cap trays with liquid weirs and rising vapor, plus BMED stack with alternating bipolar membrane sheets.
> 4. **PLA Polymerization & Extruder**: Cutaway of the twin-screw extruder revealing **dual intermeshing co-rotating screws** actively conveying molten polymer forward, plus rotary pelletizer cutter dropping white PLA resin pellets into the hopper.
> 5. **Packaging Line**: Calendering steel rolls pressing molten sheet into a continuous film roll, and thermoforming mould cycling with transparent PLA cups and clamshell trays.
> 6. **Anaerobic Digester & CHP**: Granular sludge bed with rising methane bubbles into the green gas-holder dome, yellow biogas pipe with flowing gas particles feeding the CHP engine with spinning radiator fan, and biofertilizer compost conveyor.

---

## Proposed Changes

Grouping files by target components:

### 1. 3D Digital Twin Engine (`ArtifactDigitalTwin` & `BiorefineryDigitalTwin`)

#### [MODIFY] [`biorefinery_dashboard.html`](file:///C:/Users/dines/.gemini/antigravity/brain/6e3ef6b5-1976-4d5f-9cc5-5251cd169add/biorefinery_dashboard.html)
- **UI Light Theme Restyling**:
  - Update all Tailwind container classes from `bg-slate-950`, `bg-slate-900`, `border-slate-800` to clean light industrial styling: `bg-slate-100`, `bg-white`, `border-slate-200`, `shadow-sm`, and high-contrast text `text-slate-900`.
  - Update HUD telemetry panels, charts, cards, and zone buttons to high-legibility light engineering aesthetic with industrial badge highlights.
- **Realistic PBR Procedural Textures**:
  - Procedural brushed stainless steel texture generator for columns, fermenters, and vessels.
  - Procedural safety yellow/black hazard warning stripes for equipment boundary footings.
  - Procedural diamond-plate steel pattern for catwalks and stairs.
- **Inside-Workflow Cutaways & Dynamic Animations**:
  - Add twin rotating intermeshing extruder screws in Zone 4.
  - Add bubble-cap distillation trays with liquid layers and vapor arrows in Zone 3.
  - Enhance fermenter fluid vortex and pH dosing pipe in Zone 2.
  - Add tanker flexible hose and plate heat exchanger counter-current thermal channels in Zone 1.
  - Add thermoformer mould clamping cycle animation in Zone 5.
  - Add UASB sludge bed and CHP radiator fan animation in Zone 6.
- **Industrial Detailing**:
  - Add circular dial pressure/temperature gauges with needles on reactor heads.
  - Add red/yellow handwheel valves and sanitary pipe flanges on major process lines.
  - Add industrial safety railings, toe-boards, and warning signs.
- **Synchronized Self-Contained Bundle**:
  - Keep the full Three.js and OrbitControls engine directly inlined so that all new geometries and animations run offline with 100% reliability.

#### [MODIFY] [`digital_twin_3d.js`](file:///C:/Users/dines/.gemini/antigravity/scratch/whey_to_pla_biorefinery/js/digital_twin_3d.js)
- Implement matching inside-workflow cutaways, rotating extruder screws, distillation trays, dial gauges, and procedural materials for the scratch application codebase.

#### [MODIFY] [`index.html`](file:///C:/Users/dines/.gemini/antigravity/scratch/whey_to_pla_biorefinery/index.html) & [`css/styles.css`](file:///C:/Users/dines/.gemini/antigravity/scratch/whey_to_pla_biorefinery/css/styles.css)
- Restyle the main portal UI into the light industrial SCADA theme matching `biorefinery_dashboard.html`.

---

## Verification Plan

### Automated Tests
- Syntax verification via Node `vm.Script` validator on both dashboard and scratch scripts.
- Model consistency test: Run `node test_models.js` to ensure 100% pass on all 9 mass/energy balance and TEA benchmarks.

### Manual Verification
- Verify 3D rendering in daylight/light mode with soft shadows and crisp industrial materials.
- Verify inside-workflow cutaways:
  - Watch rotating twin-screw extruder screws inside the barrel.
  - Watch bubble cap trays inside the distillation column.
  - Watch dual Rushton impellers and rising bubbles inside the fermenter.
  - Watch calendering rolls and thermoformer cycle.
  - Watch biogas generation and CHP radiator fan.
- Verify button clicks on all 6 zones and verify camera transitions smoothly to each cutaway with updated SCADA telemetry.
