# roverbot.v1 Shopping List

Maximum size LX-16A rover - 500mm × 350mm chassis, ~4.5kg target weight.

**Last updated:** January 2026

---

## YOUR BUILD: ~$272

### Drivetrain - $69

| Qty | Item | Price | Best Source | URL |
|-----|------|-------|-------------|-----|
| 4 | Hiwonder LX-16A Serial Servo | $64 | Amazon | https://www.amazon.com/dp/B073WR3SK9 |
| 1 | 8mm Aluminum Rod 500mm | $5 | McMaster-Carr | https://www.mcmaster.com/4634t34 |

**Alternative servo sources:**
- [Hiwonder Direct](https://www.hiwonder.com/products/lx-16a): $16.99 each ($68 for 4)
- [RobotShop](https://www.robotshop.com/products/hiwonder-hiwonder-lx-16a-full-metal-gear-serial-bus-servo-with-real-time-feedback-function-rc-robot-control-angle-240): check current price

**Wheels:** Sawppy-style 3D printed (see 3D Printed Parts below)

**Drive Train:**
```
LX-16A Servo → 3D Printed Coupler (25T-to-8mm) → 8mm Shaft → Wheel Hub → Wheel
```

**Shaft cuts:** 4× 50mm drive shafts from 500mm rod

### Frame - $56 (Aluminum + Printed)

| Qty | Item | Price | Source |
|-----|------|-------|--------|
| 1 | 6ft 1" Al square tube | $17 | Home Depot |
| 1 | M3/M4/M5 hardware kit | $15 | https://www.amazon.com/dp/B08JCKH31Q |
| - | 3D printed parts (~600g PETG) | $24 | Print at home |

**Frame cuts:** 2× 500mm + 2× 350mm = 1.7m total

### Sensors - $100

| Qty | Item | Price | Best Source | URL |
|-----|------|-------|-------------|-----|
| 1 | RPLidar A1 | $100 | Adafruit | https://www.adafruit.com/product/4010 |

**Alternative sources:**
- [Amazon](https://www.amazon.com/dp/B07TJW5SXF): ~$99
- [AliExpress](https://www.aliexpress.com/item/32962956404.html): ~$103 (longer shipping)
- [Seeed Studio](https://www.seeedstudio.com/RPLiDAR-A1M8-360-Degree-Laser-Scanner-Kit-12M-Range.html): check price

### Control - $20

| Qty | Item | Price | Source | URL |
|-----|------|-------|--------|-----|
| 1 | Hiwonder Servo Controller | $20 | Amazon | https://www.amazon.com/dp/B09ZL6ZBBN |

**Alternative:** [Hiwonder Direct](https://www.hiwonder.com/products/serial-bus-servo-controller): $39.99

### Power - $10

| Qty | Item | Price | Source | URL |
|-----|------|-------|--------|-----|
| 1 | 5V 5A Buck Converter | $10 | Amazon | https://www.amazon.com/dp/B09VY3WQ61 |

*Battery, wiring, connectors - already owned*

---

## TOTAL: ~$272

| Vendor | Items | Cost |
|--------|-------|------|
| **Amazon** | Servos, hardware, controller, buck | ~$109 |
| **McMaster-Carr** | 8mm aluminum rod | ~$5 |
| **Adafruit** | RPLidar A1 | ~$100 |
| **Home Depot** | Aluminum tube | ~$17 |
| **3D Print** | Frame + wheels (~600g PETG) | ~$24 |
| | **TOTAL** | **~$272** |

---

## QUICK ORDER LINKS

### Amazon Cart (~$109)
```
https://www.amazon.com/dp/B073WR3SK9 - LX-16A Servos (4) = $64
https://www.amazon.com/dp/B09ZL6ZBBN - Servo Controller = $20
https://www.amazon.com/dp/B08JCKH31Q - Hardware Kit = $15
https://www.amazon.com/dp/B09VY3WQ61 - 5V Buck Converter = $10
```

### McMaster-Carr (~$5)
```
https://www.mcmaster.com/4634t34
- 1x 8mm Aluminum Rod 500mm = $5
```

### Adafruit (~$100)
```
https://www.adafruit.com/product/4010
- 1x RPLidar A1 = $99.95
```

---

## ALREADY OWNED

| Item | Value | Notes |
|------|-------|-------|
| Raspberry Pi 5 16GB | $90 | Main compute |
| Pi 5 Aluminum Case | $20 | Passive cooling |
| Transcend USB SSD | $30 | ROS2 storage |
| BNO055 IMU | $25 | Orientation sensing |
| 2S LiPo batteries | ~$45 | Power |
| Wiring & connectors | ~$25 | XT60, JST, wire |
| Fuse & power dist | ~$15 | Safety |

---

## OPTIONAL UPGRADES

| Item | Price | Source | Notes |
|------|-------|--------|-------|
| Intel RealSense D435 | $180 | [Intel](https://www.intelrealsense.com/depth-camera-d435/) | Depth camera |
| Powered USB 3.0 Hub | $20 | Amazon | For multiple USB devices |
| 3-DOF Robot Arm | $80 | Amazon | Pick and place |
| Pan-Tilt Camera Mount | $25 | Amazon | Surveillance |

---

## 3D PRINTED PARTS

Sawppy-style wheels from [upstream STL files](https://github.com/Roger-random/Sawppy_Rover/tree/master/STL).

| Part | Qty | Weight Each | Total | Print Time |
|------|-----|-------------|-------|------------|
| Wheel (120mm) | 4 | 75g | 300g | 8 hrs each |
| Wheel Hub | 4 | 20g | 80g | 30 min each |
| LX-16A Coupler | 4 | 10g | 40g | 15 min each |
| Corner bracket | 4 | 25g | 100g | 1 hr each |
| Servo mount | 4 | 20g | 80g | 45 min each |
| Electronics tray | 1 | 60g | 60g | 2 hrs |
| Lidar mount | 1 | 20g | 20g | 30 min |
| **Total** | - | - | **~680g** | **~42 hrs** |

**STL Sources:**
- Wheels, hubs, couplers: [Sawppy STL](https://github.com/Roger-random/Sawppy_Rover/tree/master/STL)
- Frame brackets: Custom design for 1" aluminum tube

---

## WEIGHT & POWER

| Component | Weight |
|-----------|--------|
| 4× LX-16A servos | 216g |
| 4× 120mm printed wheels | 300g |
| 4× wheel hubs + couplers | 120g |
| 8mm drive shafts | 20g |
| Aluminum frame | 550g |
| 3D printed brackets | 260g |
| 2S LiPo | 450g |
| Pi 5 + case + SSD | 200g |
| RPLidar A1 | 170g |
| IMU + electronics | 100g |
| Wiring, hardware | 200g |
| **Base weight** | **~2.6 kg** |
| **Payload capacity** | **~1.9 kg** |

**Power:** ~1.7A cruise, ~6A peak @ 7.4V
**Runtime:** ~4 hours mixed use

---

*roverbot.v1 - LX-16A platform with Sawppy-style wheels*
