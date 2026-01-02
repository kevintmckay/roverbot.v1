# roverbot.v1 Shopping List

Maximum size LX-16A rover - 500mm × 350mm chassis, ~4.5kg target weight.

**Last updated:** January 2026

---

## YOUR BUILD: ~$330

### Drivetrain - $145

| Qty | Item | Price | Best Source | URL |
|-----|------|-------|-------------|-----|
| 4 | Hiwonder LX-16A Serial Servo | $64 | Amazon | https://www.amazon.com/dp/B073WR3SK9 |
| 4 | goBILDA 25T-to-6mm Shaft Coupler | $40 | goBILDA | https://www.gobilda.com/4001-series-clamping-servo-to-shaft-coupler-25-tooth-spline-to-6mm-round-bore/ |
| 2 | Pololu 12mm Hex Adapter 6mm (2-pack) | $14 | Pololu | https://www.pololu.com/product/2686 |
| 1 | 1.9" RC Crawler Wheels 100mm (4-pack) | $25 | Amazon | https://www.amazon.com/dp/B0B4ZX8QC9 |

**Alternative servo sources:**
- [Hiwonder Direct](https://www.hiwonder.com/products/lx-16a): $16.99 each ($68 for 4)
- [RobotShop](https://www.robotshop.com/products/hiwonder-hiwonder-lx-16a-full-metal-gear-serial-bus-servo-with-real-time-feedback-function-rc-robot-control-angle-240): check current price

**Adapter Chain:**
```
LX-16A Servo → goBILDA 25T-to-6mm → Pololu 6mm-to-12mm Hex → RC Crawler Wheel
```

### Frame - $47 (Aluminum + Printed)

| Qty | Item | Price | Source |
|-----|------|-------|--------|
| 1 | 6ft 1" Al square tube | $17 | Home Depot |
| 1 | M3/M4/M5 hardware kit | $15 | https://www.amazon.com/dp/B08JCKH31Q |
| - | 3D printed parts (~350g PETG) | $15 | Print at home |

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

## TOTAL: ~$330

| Vendor | Items | Cost |
|--------|-------|------|
| **Amazon** | Servos, wheels, hardware, controller, buck | ~$134 |
| **goBILDA** | 4x shaft couplers | ~$40 |
| **Pololu** | 2x hex adapter 2-packs | ~$14 |
| **Adafruit** | RPLidar A1 | ~$100 |
| **Home Depot** | Aluminum tube | ~$17 |
| **3D Print** | Frame parts | ~$15 |
| | **TOTAL** | **~$330** |

---

## QUICK ORDER LINKS

### Amazon Cart (~$134)
```
https://www.amazon.com/dp/B073WR3SK9 - LX-16A Servos (4) = $64
https://www.amazon.com/dp/B0B4ZX8QC9 - Crawler Wheels (4-pack) = $25
https://www.amazon.com/dp/B09ZL6ZBBN - Servo Controller = $20
https://www.amazon.com/dp/B08JCKH31Q - Hardware Kit = $15
https://www.amazon.com/dp/B09VY3WQ61 - 5V Buck Converter = $10
```

### goBILDA (~$40)
```
https://www.gobilda.com/4001-series-clamping-servo-to-shaft-coupler-25-tooth-spline-to-6mm-round-bore/
- 4x 25T-to-6mm Coupler @ $9.99 = $39.96
```

### Pololu (~$14)
```
https://www.pololu.com/product/2686
- 2x 12mm Hex Adapter 6mm 2-pack @ $6.95 = $13.90
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

## WEIGHT & POWER

| Component | Weight |
|-----------|--------|
| 4× LX-16A servos | 216g |
| 4× 100mm crawler wheels | 400g |
| Couplers + adapters | 60g |
| Aluminum frame | 550g |
| 3D printed parts | 350g |
| 2S LiPo | 450g |
| Pi 5 + case + SSD | 200g |
| RPLidar A1 | 170g |
| IMU + electronics | 100g |
| Wiring, hardware | 200g |
| **Base weight** | **~2.7 kg** |
| **Payload capacity** | **~1.8 kg** |

**Power:** ~1.7A cruise, ~6A peak @ 7.4V
**Runtime:** ~4 hours mixed use

---

*roverbot.v1 - LX-16A platform with payload capacity*
