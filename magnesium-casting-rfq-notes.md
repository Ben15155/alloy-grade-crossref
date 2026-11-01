# Magnesium casting RFQ notes (sand / low-pressure / gravity / investment)

For buyers and design engineers specifying **magnesium castings**. Routes covered: low-pressure
resin sand (including 3D-printed sand molds), gravity permanent mold, and investment (lost-wax).

Out of scope: extrusion, sacrificial anodes, and high-pressure die casting. Gravity permanent
mold is a gravity pour into a metal mold (some buyers say "gravity die"). That is not
high-pressure die casting.

Equivalents below follow this repository: nearest grade **by composition**, not a guaranteed
substitution. The binding document on an order is the material certificate.

## Process selection

| Route | What it is | Specify it when | Poor fit |
|---|---|---|---|
| Low-pressure resin sand, including 3D sand molds | Resin-bonded sand mold and cores, not clay/green sand. Metal fills from the bottom under low pressure and is held while the casting feeds. A 3D-printed sand mold or core is the same route without a pattern. | Medium to large parts, cored passages, wall-thickness changes, prototypes through moderate quantity, geometry that may still move. | You need investment-class as-cast tolerances on most dimensions. Machine critical faces and write the grade. |
| Gravity permanent mold | Gravity pour into a reusable metal mold. | The shape releases from metal tooling and the quantity will repeat. | Complex sand cores, or a geometry that is still changing. |
| Investment (lost-wax) | Wax or printed pattern, ceramic shell, then pour. | Smaller parts, thin sections, fine detail, surfaces you want near-net. | A large part, or a few rough prototypes where sand is enough. |

"Low pressure" on this route means a controlled fill of a **sand** mold. It does not mean
high-pressure die casting.

Sand design: plan walls from about 3 mm, keep sections even, and blend thick-to-thin. Magnesium
sand is inhibited sand; molten magnesium reacts with bare silica. Investment holds thinner
walls than sand — confirm the section on the drawing instead of using a catalog minimum.

## When AZ91C is suitable for sand casting

On a sand or gravity permanent-mold RFQ, write **AZ91C**. A bare "AZ91" does not fix the route
or the purity variant. The GB/T 1177 grade is **ZM5**.

| Item | Value |
|---|---|
| GB grade | ZM5 (ZMgAl8Zn) |
| Composition (wt %, Mg balance) | Al 7.5–9.0 · Zn 0.2–0.8 · Mn 0.15–0.50 |
| Nearest ASTM | AZ91C / AZ91E (UNS M11914) |
| Match | Close. By convention ZM5 is called AZ91C; the mean composition sits nearer AZ81A. |

AZ91C is the ordinary sand and gravity grade in the AZ91 family. Use it for a general
structural casting — housing, case, bracket, cover, frame — at room temperature, where you
want that castability and machinability.

Specify **AZ91E** instead when the same sand or gravity part has a corrosion or salt-exposure
requirement. C and E are not interchangeable on salt spray. AZ91E stays on the sand/gravity
route; it is the higher-purity variant, not a different process.

Do not use AZ91C for sustained load above about 120–130 °C. The limit is creep. Send the
service temperature and look at ZE41A (ZM2) or an EZ33-type grade (ZM3, ZM4). ZM6 is a
neodymium grade, not ZE41A — see the cross-reference in this repo.

Put the temper on the drawing: **F** as-cast, **T4** solution-treated (ductility), **T6**
solution-treated and aged (strength). Where the standard is ASTM B80, heat treatment applies
to the whole casting, not a local region.

Zirconium does not refine AZ91C. Aluminum interferes. Zr grain refinement belongs on the
Zn–Zr and RE–Zr grades (ZK51A, ZE41A, EZ33-type).

## What to put on an RFQ

- **3D drawing** — STEP model and the matching 2D drawing, same revision.
- **Dimensions in mm**, with datums. Mark which faces are as-cast and which are machined.
- **Alloy** and the standard: AZ91C or ZM5, or another named casting grade. Add AZ91E only
  when that purity is required. State the temper or the mechanical requirement it must meet.
- **Quantity** for this order, and annual volume if known. Say prototype or production.
- **Heat treatment**, and whether the heat-treatment record is a deliverable.
- **NDT**: method, acceptance standard, and the regions it covers. Radiography for internal
  soundness and penetrant for surface-breaking indications are the usual pair. Say whether
  tensile bars are cast separately or attached.
- Casting tolerance grade (below), plus any feature tighter than that grade.
- Pressure-tight or sealing surfaces, if the part has them.
- Delivery: cast blank or machined part.

## Dimensional tolerance

Cite **ISO 8062-3** and **GB/T 42124.3** (formerly **GB/T 6414-2017**, withdrawn 2025-12-01).
ISO 8062-3:2023 names the linear grades **DCTG**. Older drawings and GB/T 6414 say **CT**.
Same grade numbers: CT6 and DCTG 6 are one callout.

**CT4–CT6** are the grades typically written for investment castings. That is an industry
specification band in the standard, not a YIRUI laboratory result and not a promise for a
given part. Gravity permanent mold is often specified coarser. Sand — including low-pressure
resin sand and 3D sand molds — is coarser again. Put the grade on the drawing; do not assume
CT4–CT6 for a sand route.

Figures below are the standard's **total** linear tolerance in millimetres (ISO 8062-3:2007
Table 2, grades 4–6; GB/T 6414 used the same CT table). Default disposition is symmetric
about the nominal. Wall thickness takes one grade coarser. If the order names ISO 8062-3:2023
or GB/T 42124.3, that text governs where a figure differs.

| Nominal (mm) | CT4 | CT5 | CT6 |
|---|---|---|---|
| ≤ 10 | 0.26 | 0.36 | 0.52 |
| > 10–16 | 0.28 | 0.38 | 0.54 |
| > 16–25 | 0.30 | 0.42 | 0.58 |
| > 25–40 | 0.32 | 0.46 | 0.64 |
| > 40–63 | 0.36 | 0.50 | 0.70 |
| > 63–100 | 0.40 | 0.56 | 0.78 |
| > 100–160 | 0.44 | 0.62 | 0.88 |

Larger sizes are in the standard. A general note that foundries can quote against:

`General tolerances ISO 8062-3 – DCTG x – GCTG y – RMA z`

Required machining allowance (RMA) is its own grade. Do not bury stock inside the CT number.
Tolerance only the features that must be tighter than the general grade.

## Further reading

- https://yiruialloy.com/products/magnesium-alloy-castings/
- https://yiruialloy.com/capability/magnesium-alloy-casting/
- https://yiruialloy.com/magnesium-sand-casting-guide/
- https://yiruialloy.com/az91-magnesium-casting-alloy-guide/
- https://yiruialloy.com/casting-tolerances-dimensional-accuracy-buyer-guide/
- https://yiruialloy.com/chinese-gb-casting-alloy-western-equivalents/

Compiled by YIRUI Alloy (https://yiruialloy.com), Jiaozuo, China.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to reuse **with attribution to
[YIRUI Alloy (yiruialloy.com)](https://yiruialloy.com)**.
