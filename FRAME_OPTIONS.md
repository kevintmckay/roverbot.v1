# roverbot.v1 Frame Options

Two frame options optimized for the Prusa CORE One (250×220mm bed).

---

## Quick Comparison

| Aspect | B: Hybrid Modular | E: Pivot Rocker |
|--------|-------------------|-----------------|
| Weight | 450g | 470g |
| Cost | $15 | $12 |
| Print time | 8 hrs (+32 hrs wheels) | 14 hrs (+32 hrs wheels) |
| Rigidity | Very Good | Good |
| Suspension | None | Yes (±15°) |
| Metal parts | 4× 6mm rods | 1× 8mm rod |
| Printed parts | 9 pieces | 8 pieces |

---

## Option B: Hybrid Modular

Printed corner modules connected by aluminum rods. Lightest and fastest to print.

```
    ┌────────┐══════════════════════┌────────┐
    │ CORNER │      6mm Al rod      │ CORNER │
    │ MODULE │══════════════════════│ MODULE │
    └───╫────┘                      └────╫───┘
        ║                                ║
        ║  printed sleeve                ║
        ║  with rod inside               ║
        ║                                ║
    ┌───╫────┐                      ┌────╫───┘
    │ CORNER │══════════════════════│ CORNER │
    │ MODULE │      6mm Al rod      │ MODULE │
    └────────┘══════════════════════└────────┘
```

### Printed Parts

| Part | Size | Qty | Weight | Time |
|------|------|-----|--------|------|
| Corner module | 120×100×50mm | 4 | 320g | 4 hrs |
| Tube sleeve | 200×30×30mm | 4 | 60g | 2 hrs |
| Electronics tray | 180×100×20mm | 1 | 60g | 2 hrs |
| **Total** | | **9** | **~450g** | **~8 hrs** |

### Metal Parts

| Part | Size | Qty |
|------|------|-----|
| 6mm aluminum rod | 500mm | 2 |
| 6mm aluminum rod | 350mm | 2 |

### Pros
- Lightest frame option
- Fastest print time
- Very rigid when assembled
- Easy to disassemble for transport

### Cons
- No suspension (rigid frame)
- 4 rod cuts needed
- Rod alignment can be tricky

---

## Option E: Pivot Rocker (Recommended)

Two frame halves connected by center pivot. Simple suspension keeps all 4 wheels grounded.

See [PIVOT_FRAME.md](PIVOT_FRAME.md) for full details.

```
    ┌─────────────────────────────────┐
    │         FRONT HALF              │
    │   [servo]            [servo]    │
    │      ○                  ○       │
    └───────────────┬┬────────────────┘
                    ││
                    ●● ← 8mm pivot rod
                    ││
    ┌───────────────┴┴────────────────┐
    │      ○                  ○       │
    │   [servo]            [servo]    │
    │         REAR HALF               │
    └─────────────────────────────────┘


    SIDE VIEW - ON UNEVEN TERRAIN

         ┌──────────┐
         │  FRONT   │╲
         └────○─────┘ ╲
              wheel    ●────────────┐
                      pivot  │  REAR   │
                             └────○────┘
                                  wheel
```

### Printed Parts

| Part | Size | Qty | Weight | Time |
|------|------|-----|--------|------|
| Front half | 250×200×40mm | 1 | 180g | 4 hrs |
| Rear half | 250×200×40mm | 1 | 200g | 5 hrs |
| Servo arm | 80×60×30mm | 4 | 80g | 4 hrs |
| Pivot bushing | 30×20mm | 2 | 10g | 0.5 hr |
| **Total** | | **8** | **~470g** | **~14 hrs** |

### Metal Parts

| Part | Size | Qty |
|------|------|-----|
| 8mm aluminum rod | 100mm | 1 |

### Pros
- Actual suspension for terrain
- All 4 wheels stay grounded
- Simpler metal work (1 cut vs 4)
- Servo mounts integrated
- Better outdoor performance

### Cons
- More print time than Hybrid
- Wires must cross pivot (needs slack loop)
- Pivot bushing wears over time

---

## Printer Compatibility (CORE One 250×220mm)

| Part | Option B | Option E |
|------|----------|----------|
| Largest piece | 200×30mm sleeve | 250×200mm half |
| Fits bed? | ✓ Easy | ✓ Just fits |
| Orientation | Any | 250mm along X |

---

## Which to Choose?

| Choose... | If you prioritize... |
|-----------|---------------------|
| **B: Hybrid Modular** | Lightest weight, fastest print, maximum rigidity, indoor use |
| **E: Pivot Rocker** | Terrain handling, outdoor use, simpler assembly |

**Default recommendation: Option E (Pivot Rocker)** - The suspension is worth the extra print time for real-world use.

---

## STL Files Needed

### Wheels (Both Options)

From [Sawppy STL](https://github.com/Roger-random/Sawppy_Rover/tree/master/STL):

```
Wheel.stl                 (×4)
Wheel Hub.stl             (×4)
LX-16A - Coupler.stl      (×4)
```

### Option B (Hybrid)

```
corner_module_FL.stl      (front-left)
corner_module_FR.stl      (front-right, mirrored)
corner_module_RL.stl      (rear-left)
corner_module_RR.stl      (rear-right, mirrored)
tube_sleeve_long.stl      (×2, for 500mm)
tube_sleeve_short.stl     (×2, for 350mm)
electronics_tray.stl      (×1)
```

### Option E (Pivot Rocker)

```
pivot_front_half.stl      (×1)
pivot_rear_half.stl       (×1)
servo_arm_left.stl        (×2)
servo_arm_right.stl       (×2, mirrored)
pivot_bushing.stl         (×2)
```

---

## Material Recommendations

| Material | Use Case | Settings |
|----------|----------|----------|
| PETG | All structural parts | 240°C, 80°C bed, 3 walls |
| CF-PETG | Maximum strength | 260°C, hardened nozzle |

| Part Type | Infill | Pattern |
|-----------|--------|---------|
| Frame halves/corners | 40% | Grid |
| Servo mounts/arms | 50% | Grid |
| Sleeves/bushings | 30% | Gyroid |

---

*Both options fit CORE One. Choose Hybrid for speed, Pivot for suspension.*
