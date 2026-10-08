# Complete gimbal concept assembly

`Gimbal_Assembly.step` is one named AP214 STEP assembly containing 31 separately
named, positioned components. `parts_step/` contains the corresponding
individual STEP parts. `Gimbal_Review.FCStd` is a FreeCAD review copy.

To make a native Solid Edge assembly, open `Gimbal_Assembly.step` in Solid Edge
as an assembly and save it as `.asm`. The STEP file already carries the part
positions; it does not need manual placement. A Solid Edge `.asm` cannot be
generated in this Linux workspace.

## Last-stage joint alignment (millimetres)

- Altitude rotation axis: horizontal X axis at Y = 0, Z = 352.
- Parts 12/13: nominal Ø82 outer / Ø60 inner bearing envelopes, centred in
  the fork holes at X = −154 / +154. Actual bearing type, fits and retention
  remain to be designed.
- Parts 14/15: hollow Ø60 trunnions pass through those bearing envelopes.
  Each has a four-hole inner flange on a nominal Ø80 pitch circle, seated
  against the left/right telescope side of part 18 at X = −87 / +87.
- Parts 16/17: cylindrical spacers lie between bearing inner faces
  (X = −139 / +139) and the trunnion flanges (X = −93 / +93).
- Part 18: telescope body envelope has matching blind holes on both sides.
  Its side-to-side size, loads and balance are illustrative.
- Camera side, left to right from the camera toward the telescope: part 22
  camera envelope, 21 camera interface plate, 20 derotator envelope, 19
  adapter flange, and the outer six-hole flange of part 14. Nominal hole
  patterns match at each interface, but the camera, derotator and optical
  standard are not selected.
- Motor side: part 23 altitude motor plate seats against the right fork
  and shares its four-hole pattern. Part 24 coupling meets the right
  trunnion and part 25 motor envelope. Shaft-to-coupling torque transfer,
  gearbox and motor mounting remain unengineered.
- Parts 29/30: cable clips conform to the left fork surface and align with
  its two cable mounting holes. Cable routing and bend radius are unverified.

## Checks and limits

All 31 parts and the assembly reimport as valid solids. There are no
positive-volume intersections between separate components at the saved
position. Contact and matched holes are nominal geometry, not real fits or
fastener specifications. Bearing preload, restraints, travel stops,
structural loads, clearances during motion, balance, optical path, motors,
materials and tolerances require actual component specifications before
fabrication.

The entire model remains an image-derived concept; dimensions in
`parameters.json` were assumed from the single perspective reference.
