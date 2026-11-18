# Printable geometry for FDM

Use this alongside the [FDM field guide](slant3d-fdm.md). The source links lead to Slant 3D examples.
The **Check** paragraphs describe this skill’s proposed verification. A useful drawing dimension, build angle
or demonstrated joint is a starting point. Actual bead widths, support settings, material and loads decide the result.

## Pick the build direction before sculpting

Mark the seating faces, direction of applied force, visible surfaces, and tool or cable access in the assembly.
Then rotate a copy into build coordinates. Compare flat, upright and, for a box or bracket, tipped onto an edge.
Slant demonstrates a box tilted 45° to change both the unsupported faces and the direction of the layers.
[Enclosure orientation](https://www.youtube.com/watch?v=8NKVNwVaZU0).

**Check.** For each candidate record first-layer footprint, tallest slender feature, roofs over empty space,
clearance to remove support, and which root would peel between layers under load. An edge-down body may need
a stable sacrificial foot. Include it in the comparison. Recheck any holes whose axes change build direction.

## Draw the underside in the build frame

A chamfer under a horizontal tab lets successive layers carry it outward. A chamfer around its visible top can
leave the entire underside flat. The same distinction applies to a latch, clamp, mounting ear or cable loop.
A side loop subject to pulling can use a pierced plate and a flange at the loaded edge where a wire-like hoop
would present a small root. [Horizontal mounting features](https://www.youtube.com/watch?v=FF4D_Moywgk)
and [side-loop design](https://www.youtube.com/watch?v=Neop_O2jMkk&t=9018s).

**Check.** Inspect the actual downward surface. For a plane with unit normal **n** and unit build direction **z**,
its inclination from horizontal is `acos(abs(dot(n,z)))`. Check only downward-facing surfaces for this test.
On a fillet or spline evaluate the shallowest patch, including where the surface meets each neighbor.
For a straight unsupported ramp at angle θ above horizontal, a layer of height h projects outward by
`h / tan(θ)`. Compare that distance with the actual bead width and overlap in the slice. A 45° ramp advances
one layer height per layer. A horizontal roof needs a separate bridge or support check.

## Blends, rounded housings, feet and closed roofs

- **Bed-facing rounds.** A circular round tangent to the bottom can start almost horizontally and leave little
  initial contact. Truncate the lower arc, use a chamfer, or build a custom curve with a wider flat foot and
  a controlled first outward step. The silhouette higher up can remain curved.
  [Bed-facing fillets](https://www.youtube.com/watch?v=IrvxX0MtGMM) and
  [rounded electronics housings](https://www.youtube.com/watch?v=Neop_O2jMkk&t=18077s).
- **Domes.** If the external form is fixed and the cavity has spare height, taper the interior roof towards a
  tighter crown. When a spherical inner seat is functional, Slant shows a purpose-built support under the
  crown. [Dome interiors](https://www.youtube.com/watch?v=udEeJjzEQZI&t=64s).
- **Feet.** Small permanent feet can hold a whole enclosure floor above the plate. Print with the feet upward
  when another face can serve as the base, or use separate feet. Give a long foot rounded ends and an approach
  that will clear the surface it slides over. [Foot design](https://www.youtube.com/watch?v=hSP9CkqhZSQ).
- **Warp.** Round the *plan-view* corners of a long base, or add detachable ears where corners lift. Slant also
  explores interrupting long shrinking runs and corrugating otherwise flat surfaces.
  [Warp control](https://www.youtube.com/watch?v=iPZoDltS30A).

**Check.** Overlay the first several layers of a curved foot or wall. Inspect the actual opening below a dome.
Verify that a revised profile clears the mating part through its entire stroke and leaves the required wall.

## Bridges, removable supports and thin uprights

Two anchored ends allow a bridge. A projecting shelf has only one. Fill a nonfunctional void, taper both
shoulders, or move the split line before adding support. For an unavoidable obstruction, Slant demonstrates
localized CAD-built supports and small sacrificial posts beneath isolated features. For a tall vertical plate,
a support comb provides *lateral* restraint using a broad-footed post and short breakaway ties at intervals.
[Eliminating supports](https://www.youtube.com/watch?v=FMs-VGAu_PQ),
[support alternatives](https://www.youtube.com/watch?v=3AZWuVRUh2c) and
[support combs](https://www.youtube.com/watch?v=Neop_O2jMkk&t=35375s).
A diagonal part can also use sacrificial fins with broad bases and narrow horizontal ties. The fin base resists
tipping, and the ties determine where the removed support leaves a mark.
[Seven support-fin examples](https://www.youtube.com/watch?v=vnn4XeKQobs).

**Check.** Measure the free span along the first bridge strands and inspect anchors at both ends. On a comb,
inspect each tie, its contact scar and the extraction path. Route a breakaway contact away from an electrical
connector mouth, bearing surface or clip root. Test the intended support interface and material combination.

## Bores, connector openings and guides

For a side-facing bore consider a gabled roof, a hexagonal opening, or local compensation above the functional
diameter. If layer splitting is the concern, consider turning the bore or reinforcing its neighborhood. For a
top-facing bore, inspect its concentric perimeter paths, add a lead-in as needed, and tune fit with local
relief or compliant fins. Slant also shows local rings and offsets around mounting holes subject to pull-out.
[Side holes, including roof shapes](https://www.youtube.com/watch?v=ip70-Tw6tBE&t=354s),
[top-facing holes](https://www.youtube.com/watch?v=3BIvSiuQVWQ),
[press-fit relief](https://www.youtube.com/watch?v=Bd7Yyn61XWQ) and
[reinforcing mounting holes](https://www.youtube.com/watch?v=UfJIMn4nvsA).

**Check.** A USB shell, cable overmold and PCB guide contact have different envelopes. Keep the guide bearing
face, sweep the overmold along insertion, and slope the surrounding roof only where there is room. Section
both ends of the recess. A good fit at the outer opening says little about an internal shoulder.

## Carry loads with printable walls

An exposed horizontal rib can leave each cell beneath it needing support. Thicken and incline the rib root,
or try a different build direction. Slant also demonstrates replacing exposed trusses with a continuous
skin and deliberately shaped interior features that induce additional perimeters in the loaded region.
A corrugated or locally relieved section is useful only when the resulting walls bond.
[Ribs for enclosures](https://www.youtube.com/watch?v=8vz9b0zNMVg),
[internal reinforcement](https://www.youtube.com/watch?v=OcxfQeeKn-s&t=152s) and
[wall ripples](https://www.youtube.com/watch?v=Neop_O2jMkk&t=4400s).

**Check.** Mark every tiny island, thin lip or slit as a functional contact, deliberate slicer instruction,
sacrificial feature or unexplained remnant. Compare slices with and without the suspected detail. A modeled
slit may have value if it creates bonded perimeter runs. A load-bearing tab that vanishes needs a wider,
connected root or a different design. Remove an unexplained sliver at its source and recheck the fit.
For a wire clip inherited from a molded design, re-evaluate the section available for the loaded arm in
its chosen build direction. [Thin parts and wire clips](https://www.youtube.com/watch?v=as84ZBjdmxU).

## Fins, slots and airflow

Slant compares slab-and-slot alignment, keyed pins and compliant fins where tight friction fits would
demand close control of the entire perimeter. For vents, sloping a slot through the wall or staggering two
rows of louvers changes sightlines and flow. Internal ribs can shorten long bridges and stiffen slats.
[Connector fins and slots](https://www.youtube.com/watch?v=vsHpiHhB3RU&t=1167s),
[vent openings](https://www.youtube.com/watch?v=Neop_O2jMkk&t=3743s) and
[directional vents](https://www.youtube.com/watch?v=Neop_O2jMkk&t=12210s).

**Check.** Measure the smallest clear airway after adding ribs and the least-supported slat in build
coordinates. Test airflow and drainage in the installed orientation. For locating fins, check insertion,
final movement, and withdrawal clearance with the mating shape and an actual printed pair.
