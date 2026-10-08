# Base, fork arms and gussets — concept assembly

Open `Fork_Base_Subassembly.step` as a STEP assembly in Solid Edge. It contains
15 individually named, already positioned parts: the 11-part base/azimuth
assembly plus separate left and right fork arms and separate left and right
gussets. Save the imported assembly as a native Solid Edge `.asm` if needed.
`Fork_Base_Subassembly.FCStd` is a FreeCAD review copy.

## Alignment datums (millimetres)

- Fixed base underside: Z = 0. Rotating deck top: Z = 110.
- Fork feet sit on the deck top. Fork centre planes: X = −154 and +154.
- Two foot holes per fork are centred at Y = −55 and +55. Their centres align
  with the four Ø9 deck holes at X = ±154, Y = ±55.
- Both Ø82 altitude bearing bores are coaxial along X, centred at Y = 0,
  Z = 352. The bore centre separation between the arms is 308 mm.
- Each gusset starts on the deck at Z = 110 and is trimmed to the sloping
  inner face of its fork arm. The prior 1 mm gap below the gussets is removed.

## Suggested virtual assembly order

1. Keep the existing 11-part base and azimuth assembly fixed.
2. Seat the left and right fork feet on the rotating deck and align each pair
   of foot holes with the matching deck holes.
3. Check that the altitude bores share one horizontal X axis.
4. Seat each gusset on the deck and against its corresponding fork's inner
   tapered face. The gussets are separate bodies; no weld or bolted joint has
   been specified.

All 15 imported solids are valid, and pairwise solid interference is zero in
the saved position. This verifies virtual placement, not strength or safety.
Dimensions were estimated from one reference image. Choose material, load,
joining method, fasteners, bearings and motor hardware before fabrication.
