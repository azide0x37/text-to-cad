# FDM joints, board mounts and serviceable enclosures

Use this reference when a printed feature locates, retains, flexes, seals or carries a load.
The linked Slant 3D demonstrations supply the design patterns. The verification steps at the end
are this fork's engineering practice. Actual load, travel, clearance and life depend on the assembly.

## Put contact where it has a job

- **Locating a part.** Give the entering edge a lead-in and round the corners that would otherwise
  snag. Locate on a few defined surfaces. Long, closely spaced mating faces accumulate friction
  and are sensitive to corner bulges and first-layer spread. Use a sprung contact or a set of
  yielding fins when fit must absorb variation. [Fitting demonstration](https://www.youtube.com/watch?v=XKrDUnZCmQQ)
- **Selecting a joint.** A diamond-profile key can locate a side-facing joint with a printable roof.
  A wide tongue in a slot distributes alignment over length. A keyed T-slot can capture a slide
  against pullout across its axis. Select by assembly direction and identify how the joint resists
  withdrawal along that axis. [Keys, fins and locking slides](https://www.youtube.com/watch?v=vsHpiHhB3RU)
- **Lids.** A tapered plug gets progressively tighter as it seats. Discrete grip fins or compliant
  lands can take up clearance without making the entire lid rim a press fit. Where more travel is
  needed, a spring-loaded catch can engage after the lid seats. [Lid forms](https://www.youtube.com/watch?v=7YAylxQFe3k) · [Compliant lids](https://www.youtube.com/watch?v=IZKh6lo9SP4)
- **Snap arms.** Lay an elongated spring so bending uses continuous in-plane paths through its
  root. A vertical tongue bent across the layer stack is vulnerable to separation. Chamfer the
  insertion face, leave room behind the arm, and consider a button or multi-sided catch where
  a leaf cannot fit. [Snap orientations and geometries](https://www.youtube.com/watch?v=rsfZgT3ZEI8&t=154s)
- **Round clips and ring clamps.** Decide whether the clip or the ring will supply the deflection.
  When several tabs project from a ring, inspect each root in the proposed print orientation.
  Tilting the ring and sloping the undersides can support several tabs while improving how their
  roots cross the layers. [Ring clamp example](https://www.youtube.com/watch?v=Neop_O2jMkk&t=8395s)

## Make motion printable

- **Springs and buttons.** For a push button or return mechanism, sketch the travel and consider a
  leaf, planar serpentine or spiral. These profiles can keep a bead continuous along the spring.
  Size the active length and thickness for the desired motion. A wound helix standing upright
  loads a different set of bonds. [Spring mechanisms](https://www.youtube.com/watch?v=wpriGP45Unw)
- **Living hinges.** A thin fold concentrates strain. A broader curved flexure or several articulated
  flexures can distribute a limited rotation across a longer length and supply a restoring force.
  Account for the swept space, required opening angle and filament. Slant demonstrates compliant
  materials for thin folds. [Living hinge variants](https://www.youtube.com/watch?v=TiEyFle6lTM)
- **Print-in-place pivots.** Where free rotation or little spring return is required, consider
  captured conical pivots. Opposed sloped bearing surfaces can locate adjacent links axially while
  growing without a flat internal roof. Inspect radial and axial gaps separately in print orientation.
  [Hinge demonstration](https://www.youtube.com/watch?v=BWsUk1xSSn4) · [Conical pivots](https://www.youtube.com/watch?v=Neop_O2jMkk&t=13006s)
- **Captive sliders.** Shape the roof above the tongue and its mating top together. A sloped roof
  keeps a sagging bridge out of the sliding clearance. Provide access to remove any sacrificial
  piece at the handle opening. The spring path, handle and guide must all fit in the chosen build
  orientation. [Print-in-place latch](https://www.youtube.com/watch?v=4wRKmcWXEkw)

## Carry loads into the enclosure

For a comparison of lid-captured panels, floor-mounted boards and tie-through cable anchors, see the [Heart Labs enclosure examples](heart-labs-enclosures.md).

- **PCB seats.** Widen a boss base with a chamfered web or connect it to the wall with a rib. Where
  the PCB underside permits, recess its projecting leads into a broad seat that supports the board
  at its intended bearing surfaces. Model the tallest solder joints before sizing the recess.
  [Electrical enclosure and PCB mounting examples](https://www.youtube.com/watch?v=9ERY20MRJPo)
- **Mounts and fastener access.** A strap can pass through a slot whose loaded perimeter is traced
  by continuous layers. Rail mounts can be integrated into the wall. For an externally accessible
  screw, grow the lug out of the wall and slope its underside. Clear space for the driving tool.
  [Enclosure mounts](https://www.youtube.com/watch?v=lGnpz8q4STw) · [Horizontal mounting features](https://www.youtube.com/watch?v=FF4D_Moywgk)
- **Wire clips and side loops.** Replace a narrow right-angle junction with a broad chamfer or loft
  between the clip and its foot. For a conduit saddle, starting with the allowable volume and cutting
  the cable passage and fastener holes can leave a much stronger root. [Wire bracket](https://www.youtube.com/watch?v=Neop_O2jMkk&t=39070s)
- **Mating a lid to a rounded housing.** Use internal ribs to register a lid without crowding the
  entire perimeter with a thick rim. Choose the parting line and bed face for each half, and ease
  the lip where a first-layer bulge could jam it. [Rounded enclosure](https://www.youtube.com/watch?v=m20UPm0TOto)

## Choose a fastening method

- **Screws and nuts.** For low-duty plastic threads, compare a pilot or relief-cut hole. Where
  repeated disassembly calls for metal threads, compare a heat-set insert with a hex nut captured
  from the rear or slid in from an accessible side after printing. Orient the pocket so a shoulder
  reacts the working pull. [Captive hardware alternatives](https://www.youtube.com/watch?v=WMbmDfGEygk)
- **Printed threads.** Check pitch and tooth sections in the actual toolpath. Fine modeled teeth
  can disappear. For a horizontal screw, consider relieving the crown and floor of the hole and
  retaining printable thread arcs on the sides. Check the remaining engagement on the real screw.
  [Threaded-hole examples](https://www.youtube.com/watch?v=Neop_O2jMkk&t=14170s) · [Directional hole design](https://www.youtube.com/watch?v=ip70-Tw6tBE)
- **Bonded joints.** Give adhesive a reservoir so squeeze-out does not separate the seating faces.
  For a joint bonded after assembly, provide a delivery hole and a path to a visible exit. Keep the
  flow path clear of bearings and hardware. [Glue slots](https://www.youtube.com/watch?v=fpabmEmcztI) · [Adhesive delivery channels](https://www.youtube.com/watch?v=Nsv3YSTDYmA)
- **Magnetic closures.** A side-loaded slot or over-center catch can mechanically retain a magnet
  as a tight printed pocket relaxes. Decide how to establish polarity, which surfaces need contact,
  and which feature prevents the magnet escaping. [Magnet retention variants](https://www.youtube.com/watch?v=BwUzOJ8B_H0&t=144s)

## Verify the chosen mechanism

These are checks added by this fork. Set pass criteria from the actual application.

1. Identify the locating surfaces, service load, insertion direction and extraction direction.
   Mark the rigid stop, flexing member and release access separately. A board mount can react
   connector insertion against a fixed board edge and reserve the flexible latch for retention.
2. Sweep the entering board, mating plug, fastener, wire and release tool through their full travel.
   Include the plug overmold and the component height on both faces of the PCB. A section through
   the final seated position alone can miss a collision during insertion.
3. Inspect the slice at the root, under the ledge, through the working gap and at the first free
   layer. Verify that each load-bearing pad has deposited material connected to its base, every
   moving pair stays separate, and support has an extraction path.
4. Print the joint with its real surroundings, layer direction, material and profile. Measure
   insertion and release force, movement at the hard stop and play after repeated cycles. Where a
   spring or grip stays deflected in service, repeat the fit check after a representative dwell.
   Record the tested conditions alongside the result.
