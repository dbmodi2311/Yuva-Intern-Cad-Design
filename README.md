# Yuva-Intern-Cad-Design
# Adjustable Link Bracket: CAD Design Internship Project

A 4-week CAD design internship project. It starts with a single sketched part and ends with a fully documented, checked and presented assembly.

- **Author:** Modi Dhruv Bhaveshbhai
- **Programme:** B.Tech Mechanical Engineering, Government Engineering College, Patan
- **Tools:** SolidWorks Premium 2024 SP1.0, AutoCAD
- **Standards:** ISO drafting, first-angle projection, MMGS units (mm, g, s)

---

## Table of Contents

1. [Project Overview](#1-project-overview)
2. [Engineering Requirements](#2-engineering-requirements)
3. [How the Design Works](#3-how-the-design-works)
4. [Part Specifications](#4-part-specifications)
5. [Slot Geometry Analysis](#5-slot-geometry-analysis)
6. [Fit and Tolerance Analysis](#6-fit-and-tolerance-analysis)
7. [Assembly and Mates](#7-assembly-and-mates)
8. [Design Review: Findings and Limitations](#8-design-review-findings-and-limitations)
9. [Modelling Workflow](#9-modelling-workflow)
10. [Drawing and Documentation Standards](#10-drawing-and-documentation-standards)
11. [Verification Checklist](#11-verification-checklist)
12. [Repository Layout and Naming](#12-repository-layout-and-naming)
13. [Weekly Log](#13-weekly-log)
14. [Skills Demonstrated](#14-skills-demonstrated)
15. [Future Work](#15-future-work)
16. [References](#16-references)

---

## 1. Project Overview

- **What it is:** a bracket where a slotted link plate pivots on a shoulder pin in a base plate and is locked by an M10 bolt through the slot.
- **Origin:** the Slotted Link Plate (Week 2) was modelled first, then used as the core part of the assembly (Week 3) and refined into the capstone (Week 4).
- **Why this project:** one part brings together holes, a slot, tangent arcs, a concave blend, fits and fasteners, so it exercises most CAD skills in a small design.
- **Typical applications:** adjustable guards, sensor mounts, pointer arms and positioning supports.

### Parts at a glance

| Item | Part | Qty | Material / Standard |
|------|------|-----|---------------------|
| 1 | Base Plate | 1 | Plain carbon steel |
| 2 | Slotted Link Plate | 1 | Plain carbon steel |
| 3 | Shoulder Pivot Pin Ø20 | 1 | Plain carbon steel |
| 4 | Hex Bolt M10 x 40 | 1 | ISO 4017 |
| 5 | Hex Nut M10 | 1 | ISO 4032 |
| 6 | Plain Washer M10 | 2 | ISO 7089 |

---

## 2. Engineering Requirements

| ID | Requirement | How it is met |
|----|-------------|---------------|
| R1 | Link rotates freely about the pivot before locking | Ø20 H7/g6 clearance fit |
| R2 | Link can be locked firmly in position | M10 bolt, nut and washers clamp the link to the base plate |
| R3 | Bolt passes through the slot without binding | Slot is 12 wide for a Ø10 bolt (1 mm clearance each side) |
| R4 | Only standard, buyable fasteners | ISO 4017, ISO 4032 and ISO 7089 |
| R5 | Manufacturable from plain plate | Profile cutting, drilling and milling only |
| R6 | Fully documented | Drawing set, BOM, balloons, tolerances |
| R7 | All geometry is parametric and editable | Fully defined sketches |

---

## 3. How the Design Works

- The shoulder pin passes through the Ø20 hole in the base plate and the Ø20 hole in the link plate.
- The link rotates about the pin axis.
- The M10 bolt goes down through the link slot and the base plate hole.
- A washer sits under the bolt head, and a washer and nut sit under the base plate.
- Tightening the nut clamps the link face to the base plate face by friction.
- The 2 mm of pin shank that projects below the base plate allows an optional retaining clip.
- **Mounting note:** the pin end and the nut project below the base plate, so mount it with at least 10 mm free space underneath.

---

## 4. Part Specifications

### 4.1 Slotted Link Plate (Week 2)

| Feature | Value |
|---------|-------|
| Thickness | 10 mm (design choice) |
| Pivot hole | Ø20 mm |
| Slot width | 12 mm (R6 ends) |
| Slot length, centre to centre | 40 mm |
| Hole centre to slot right-end centre (horizontal) | 85 mm |
| Hole centre to slot centreline (vertical) | 40 mm |
| Top edge horizontal dimension | 90 mm |
| Corner and slot-end arcs | R15 |
| Lower boss arc around the pivot hole | R30 |
| Concave blend arc | R50 |
| Edge treatment | 1 mm chamfer on hole and slot edges |
| Sketch plane | Top Plane |
| Sketch status | Fully Defined |

### 4.2 Base Plate (design choices)

| Feature | Value |
|---------|-------|
| Outline | 160 x 100 x 10 mm |
| Pivot hole | Ø20 H7, centred 40 mm from the left edge and 40 mm from the bottom edge |
| Bolt hole | Ø10.5 mm clearance hole at 75 mm from the pivot (63.4 mm right and 40 mm up from the pivot) |
| Mounting holes | 4 x Ø9 near the corners, 15 mm from each edge |
| Corner radius | R5 |
| Edge treatment | 1 mm chamfer on hole edges |

- With the pivot at 40 mm from the left and bottom edges, the link stays inside the plate outline.
- The link reaches about 100 mm to the right of the pivot, 30 mm to the left, 55 mm up and 30 mm down.

### 4.3 Shoulder Pivot Pin (design choices)

| Feature | Value |
|---------|-------|
| Shank | Ø20 g6 |
| Shank length | 22 mm (10 base plate + 10 link + 2 projecting) |
| Head | Ø28 x 6 mm |
| Ends | 1 mm chamfer |
| Optional | Groove or hole at the projecting end for a retaining clip |

### 4.4 Fasteners

| Item | Standard | Note |
|------|----------|------|
| Hex bolt M10 x 40 | ISO 4017 | Leaves about 7.6 mm projecting below the nut; M10 x 35 is an option |
| Hex nut M10 | ISO 4032 | Height about 8.4 mm |
| Plain washer M10 (2) | ISO 7089 | 2 mm thick, larger than the 12 mm slot width |

---

## 5. Slot Geometry Analysis

The slot centreline is a straight line 40 mm above the pivot centre. Its end centres lie at:

| Point | Horizontal from pivot | Vertical from pivot | Distance from pivot |
|-------|----------------------|---------------------|---------------------|
| Left end centre | 45 mm | 40 mm | 60.2 mm |
| Right end centre | 85 mm | 40 mm | 93.9 mm |

- A bolt hole in the base plate can only line up with the slot if its distance from the pivot is between **60.2 mm and 93.9 mm**.
- The bolt hole is placed at **75 mm**, near the middle of that range, so the bolt sits at the middle of the slot at the reference position.
- The pivot-to-bolt distance is fixed by the base plate. The link therefore turns about the pivot, and the bolt moves across the slot width.
- The base plate is the controlling part: the hole position decides where the bolt sits in the slot.

---

## 6. Fit and Tolerance Analysis

### 6.1 Pivot fit: Ø20 H7 / g6 (ISO 286)

| Item | Upper deviation | Lower deviation | Limits |
|------|-----------------|-----------------|--------|
| Hole H7 | +0.021 mm | 0 | Ø20.000 to Ø20.021 |
| Pin g6 | -0.007 mm | -0.020 mm | Ø19.980 to Ø19.993 |

- Minimum clearance = 20.000 - 19.993 = **0.007 mm**
- Maximum clearance = 20.021 - 19.980 = **0.041 mm**
- Result: a close running fit that gives smooth rotation with little play.

### 6.2 Bolt fit

- M10 bolt (Ø10) in a Ø10.5 base plate hole: about 0.25 mm clearance on each side.
- M10 bolt (Ø10) in the 12 mm slot: 1 mm clearance on each side.
- M10 washer outer diameter (20 mm) is larger than the slot width, so the washer always bridges the slot.

### 6.3 General tolerances

- Linear dimensions without a tolerance follow ISO 2768-m (medium).
- Drawing notes: break sharp edges 0.5 mm, remove burrs.

---

## 7. Assembly and Mates

| Parts | Mates |
|-------|-------|
| Base Plate and Pivot Pin | Concentric (hole and shank) + Coincident (pin head face to plate face) |
| Link Plate and Pivot Pin | Concentric (hole and shank) + Coincident (link face to base plate face) |
| Bolt and Base Plate | Concentric (bolt shank and Ø10.5 hole) |
| Bolt and Link Slot | Slot mate or width mate, so the bolt stays in the slot |
| Washers, Nut and Bolt | Concentric + Coincident faces |

- Use the fewest mates that fully describe the real contact.
- Leave the link rotation free until the bolt is tightened.
- Resolve every over-defined or conflicting mate before continuing.

---

## 8. Design Review: Findings and Limitations

This section records an honest review of the design.

### 8.1 Finding: limited angular adjustment

- The slot is straight, but the link rotates in a circle about the pivot.
- With the bolt fixed in the base plate, the bolt moves **across** the slot when the link turns, not along it.
- The Ø10 bolt has only 1 mm clearance each side in the 12 mm slot.
- Estimated allowable rotation before the bolt touches the slot wall: about **±0.7° to ±1.3°**, depending on how far the bolt is from the pivot.

| Bolt distance from pivot | Approx. allowed rotation |
|--------------------------|--------------------------|
| 60.2 mm (left end) | ±1.27° |
| 75 mm (design value) | ±0.9° |
| 93.9 mm (right end) | ±0.67° |

- **What this means:** as modelled, the slot gives assembly tolerance and a small fine adjustment. It does not give a large angular range.

### 8.2 Recommended upgrades

- Change the slot to an **arc slot** concentric with the pivot, with radius equal to the bolt distance (75 mm). The bolt then slides along the slot over a wide angle.
- Or keep the straight slot and use the part as a **slotted lever**: a driver pin on a rotating crank slides in the slot and makes the link oscillate. Check the motion in a SolidWorks Motion Study.
- Or add a second base plate hole to give two fixed locking positions.

### 8.3 Other review notes

- The pin head sits on top of the link, so a thin washer or shoulder length control is needed to stop the head clamping the link.
- Clamping by friction only: for loaded use, add a serrated washer or a lock nut.
- Check clearance between the bolt head washer and the R50 blend edge.

---

## 9. Modelling Workflow

### 9.1 SolidWorks

1. Create the part file and set units to MMGS.
2. Sketch the profile on the Top Plane.
3. Add geometric relations first (tangent, horizontal, coincident, equal).
4. Add dimensions until the sketch status is **Fully Defined**.
5. Use Extruded Boss/Base for the 10 mm thickness.
6. Add chamfers and fillets.
7. Assign Plain Carbon Steel.
8. Check Mass Properties.
9. Build the other parts in the same way.
10. Create the assembly, fix the base plate and add mates.
11. Run Interference Detection and check the range of motion.
12. Create the exploded view.
13. Generate drawings from the models.

### 9.2 AutoCAD

1. Set units to millimetres.
2. Create layers: Outline, Centre, Dimension, Hidden, Text.
3. Draw with LINE, CIRCLE and ARC.
4. Refine with OFFSET, TRIM and FILLET.
5. Add dimensions with DIMLINEAR, DIMDIAMETER and DIMRADIUS.
6. Compare every dimension with the SolidWorks model.

---

## 10. Drawing and Documentation Standards

| Item | Standard |
|------|----------|
| Projection | First angle |
| Sheet size | A3 |
| Units | Millimetres |
| Title block | Part name, number, material, scale, drawn by, date, revision |
| Line types | Continuous (outline), chain (centre), dashed (hidden) |
| Dimensions | One dimension per feature, no duplicates, outside the views |
| Tolerances | H7/g6 on the pivot, ISO 2768-m for general tolerance |

### Drawing set

| Sheet | Contents |
|-------|----------|
| 1 | Assembly drawing: views, balloons, BOM, revision table |
| 2 | Base Plate detail drawing |
| 3 | Slotted Link Plate detail drawing |
| 4 | Shoulder Pivot Pin detail drawing with fit tolerance |
| 5 | Exploded view |
| 6 | AutoCAD 2D layout and plan view |

---

## 11. Verification Checklist

Tick each item when you have checked it on your own model.

- [ ] All sketches show Fully Defined
- [ ] Thickness of every plate measures 10 mm
- [ ] Material assigned to every part
- [ ] Mass properties recorded for each part and the assembly
- [ ] No mate errors or over-defined warnings
- [ ] Interference Detection shows no overlap
- [ ] Link rotates freely before the bolt is tightened
- [ ] Bolt stays inside the slot over the allowed rotation
- [ ] Drawing dimensions match the 3D model
- [ ] AutoCAD dimensions match SolidWorks
- [ ] BOM and balloons match the assembly
- [ ] Title block and revision table are complete

---

## 12. Repository Layout and Naming

```
/parts          .SLDPRT files (base plate, link plate, pin, fasteners)
/assembly       .SLDASM file
/drawings       .SLDDRW and PDF sheets
/autocad        .DWG files
/reports        Week 1-4 Word reports
/images         Screenshots and renders
README.md
```

- **File names:** `BasePlate.SLDPRT`, `SlottedLinkPlate.SLDPRT`, `PivotPin.SLDPRT`, `LinkBracket.SLDASM`.
- **Feature names:** descriptive (for example "Pivot Hole", "Slot Cut").
- **Layer names:** Outline, Centre, Dimension, Hidden, Text.
- **To open:** use SolidWorks 2024 or newer and keep all files in this folder structure so the mates resolve. Open `.DWG` files in AutoCAD or any DWG viewer.

---

## 13. Weekly Log

| Week | Focus | Output |
|------|-------|--------|
| 1 | CAD fundamentals and tool setup | Fundamentals write-up and setup screenshot |
| 2 | Hands-on practice | Slotted Link Plate: 3D model, drawing and AutoCAD redraw |
| 3 | Mini project | Adjustable Link Bracket assembly, BOM and drawing set |
| 4 | Capstone | Final design, checks, documentation and presentation summary |

---

## 14. Skills Demonstrated

- Parametric 3D modelling with fully defined sketches
- Assembly design with mates and interference checks
- Engineering drawings with tolerances, BOM and balloons
- 2D drafting in AutoCAD with layers and dimension styles
- Fit and tolerance selection (ISO 286)
- Design review and honest limitation analysis
- Technical documentation

---

## 15. Future Work

- Replace the straight slot with an arc slot for a wide adjustment range
- Add a graduated angle scale on the base plate
- Add a bushing at the pivot to reduce wear
- Run a stress study with SolidWorks Simulation
- Run a Motion Study for the slotted-lever version
- Export DXF files for laser cutting
- Create a rendered presentation image

---

## 16. References

- ISO 286: limits and fits
- ISO 2768: general tolerances
- ISO 4017: hex head bolts
- ISO 4032: hex nuts
- ISO 7089: plain washers
- ISO 273: clearance holes for bolts
- ISO 128: technical drawing conventions
- SolidWorks 2024 help and AutoCAD documentation

*Standard numbers are listed from memory. Please verify them against the official standards before final submission.*
