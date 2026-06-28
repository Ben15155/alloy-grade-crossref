# China GB ↔ Western Cast-Alloy Grade Cross-Reference (by composition)

Open reference mapping **Chinese GB cast aluminum (ZL, GB/T 1173)** and **magnesium (ZM, GB/T 1177)**
alloy grades to their **nearest ASTM/AA, EN 1706/1753 and JIS equivalents** — matched **by chemical
composition, not by name** (the mistake most online tables make).

📄 **Browsable table:** see the GitHub Pages site for this repo · 📊 **Machine-readable:** [`alloy-grade-crossref.csv`](alloy-grade-crossref.csv)

> Compiled and maintained by **[YIRUI Alloy](https://yiruialloy.com)** — a magnesium & aluminum alloy
> casting manufacturer in Jiaozuo, China (since 2006). Full guide with composition notes:
> <https://yiruialloy.com/chinese-gb-casting-alloy-western-equivalents/>

## How to read this
Equivalents are the **nearest grade by composition**, not a guaranteed 1:1 substitution. Only two pairs
are genuinely exact: **ZM1 → ZK51A** and **ZM2 → ZE41A**. The single binding document for any order is the
**GB/T material certificate**. Confirm the spec for your application.

## Cast Aluminum — GB/T 1173 (ZL)
| GB grade | Key composition (wt %) | ASTM/AA (UNS) | EN 1706 | JIS | Match |
|---|---|---|---|---|---|
| ZL101 | Si 6.5–7.5 · Mg 0.25–0.45 | 356.0 / A356.0 | AC-42000/42100 | AC4C | close |
| ZL101A | Si 6.5–7.5 · Mg 0.25–0.45 · Ti 0.08–0.20 | **A356.0** | **AC-42100** | AC4CH | near-exact |
| ZL102 | Si 10–13 | 413.0 / A413.0 | AC-44000/44100 | AC3A | close |
| ZL104 | Si 8–10.5 · Mg 0.17–0.35 · Mn 0.2–0.5 | A360.0 | **AC-43300** | AC4A | approx |
| ZL105 | Si 4.5–5.5 · Cu 1–1.5 · Mg 0.4–0.6 | 355.0 / C355 | AC-45300 | AC4D | close |
| ZL111 | Si 8–10 · Cu 1.3–1.8 · Mg 0.4–0.6 | **354.0** | — | — | close ⚠️ not AlSi8Cu3 |
| ZL114A | Si 6.5–7.5 · Mg 0.45–0.75 · Ti | A357.0 | AC-42200 | AC4CH-mod | close |
| ZL201 | Cu 4.5–5.3 · Mn 0.6–1.0 · Ti | ~204.0 / 295.0 | AC-21100 | AC1B | approx |
| ZL205A | Cu 4.6–5.3 · Cd · V · Zr · B | **none** (nearest 206/A206) | none | none | China-proprietary |
| ZL301 | Mg 9.5–11.0 | 520.0 | ~AC-51300 | AC7B | close |

## Cast Magnesium — GB/T 1177 (ZM)
| GB grade | Key composition (wt %) | ASTM (UNS) | EN/ISO | Match |
|---|---|---|---|---|
| ZM1 | Zn 3.5–5.5 · Zr ≥0.5 | **ZK51A** (M16510) | MCMgZn6Zr | **exact** |
| ZM2 | Zn 3.5–5.0 · RE(Ce) 0.75–1.75 · Zr | **ZE41A** (M16410) = Elektron RZ5 | MC35110 | **exact/near** |
| ZM3 | RE(Ce) 2.5–4.0 · Zn 0.2–0.7 · Zr | EZ33A (M12330) | MC65120 | approx |
| ZM4 | RE 2.5–4.0 · Zn 2.0–3.0 · Zr | EZ33A | MC65120 | close |
| ZM5 | Al 7.5–9.0 · Zn 0.2–0.8 · Mn | **AZ91C/E** (M11914) | MCMgAl9Zn1 | close |
| ZM6 | **Nd 2.0–3.0** · Zn 0.2–0.7 · Zr | EZ33A analog | MC65120 | approx ⚠️ not ZE41A |
| ZM7 | Zn 7.5–9.0 · Ag 0.6–1.2 · Zr | **none** (nearest ZK61A) | — | China-proprietary |
| ZM10 | Al 9.0–10.2 · Zn 0.6–1.2 · Mn | AZ91C/E; AZ92A | ~MCMgAl9Zn1 | close |

### Key corrections (common mistakes)
- **ZL111 = 354.0**, *not* AlSi8Cu3/AC-46200 (name-based tables get this wrong).
- **ZL205A** has **no** Western equivalent (Cd/V/Zr/B micro-alloyed, proprietary).
- **ZM6 ≈ EZ33A-type** (Nd, low Zn) — *not* ZE41A/RZ5 (Ce, high Zn — the opposite).
- **ZM5 = AZ91C** by convention; mean composition sits nearer AZ81A.

## License
[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) — free to reuse **with attribution to
[YIRUI Alloy (yiruialloy.com)](https://yiruialloy.com)**.

## Contributing
Found a better composition match or a GB/T 1177-2018 impurity-ceiling correction? Open an issue or PR with the
authoritative source. Sources used: GB/T 1173 / 1177, ASTM B26/B108/B80/B403, EN 1706/1753, Total Materia, MatWeb, MakeItFrom.
