# roverbot.v1 Shopping List

500mm × 350mm chassis, ~4.5kg max weight, ~$295 total.

---

## Parts to Buy - $295

| Qty | Item | Price | URL |
|-----|------|-------|-----|
| 4 | LX-16A Servo | $64 | https://www.amazon.com/dp/B073WR3SK9 |
| 1 | Servo Controller | $20 | https://www.amazon.com/dp/B09ZL6ZBBN |
| 1 | RPLidar A1 | $100 | https://www.adafruit.com/product/4010 |
| 1 | M3/M4/M5 Hardware Kit | $15 | https://www.amazon.com/dp/B08MJGQCLQ |
| 1 | 5V 6A Buck Converter | $12 | https://www.amazon.com/dp/B0C4L66SZ9 |
| 1 | M3 Heat-Set Inserts (100) | $15 | https://www.amazon.com/dp/B077CJV3Z9 |
| 1 | M3x8mm Set Screws (100) | $5 | https://www.amazon.com/dp/B0BQ62254W |
| 1 | 8mm E-Clips (44) | $8 | https://www.amazon.com/dp/B015LLOD64 |
| 1 | Loctite Blue 242 | $6 | https://www.amazon.com/dp/B000I1RSNS |
| 1 | 8mm Aluminum Rod 500mm | $5 | https://www.mcmaster.com/4634t34 |
| 1 | 1" Al Square Tube 6ft | $17 | Home Depot |
| - | 3D Print (~700g PETG) | $28 | - |

**Total: ~$295** (+$15 for 8mm reamer if needed)

---

## 3D Printed Parts

STL from [Sawppy](https://github.com/Roger-random/Sawppy_Rover/tree/master/STL):

| Part | Qty | Weight | Time |
|------|-----|--------|------|
| Wheel (120mm) | 4 | 300g | 32 hrs |
| Wheel Hub | 4 | 80g | 2 hrs |
| LX-16A Coupler | 4 | 40g | 1 hr |
| Corner bracket | 4 | 100g | 4 hrs |
| Servo mount | 4 | 80g | 3 hrs |
| Electronics tray | 1 | 60g | 2 hrs |
| Lidar mount | 1 | 20g | 0.5 hr |
| **Total** | | **~680g** | **~42 hrs** |

Post-processing: Ream wheel hubs to 8mm, install heat-set inserts.

---

## Already Owned

| Item | Value |
|------|-------|
| Raspberry Pi 5 16GB | $90 |
| Pi 5 Case + SSD | $50 |
| BNO055 IMU | $25 |
| 2S LiPo + wiring | $85 |

---

## Cuts

- **Aluminum tube:** 2× 500mm + 2× 350mm
- **8mm rod:** 4× 50mm shafts

---

## Drive Train

```
LX-16A → Printed Coupler → 8mm Shaft → Wheel Hub → Wheel
```
