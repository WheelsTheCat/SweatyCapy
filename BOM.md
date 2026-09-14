# SweatyCapy v1.0 — Bill of Materials

Generic BOM — any equivalent part with the same footprint/pitch will work.

## PCB Components

| Ref | Qty | Part | Description | Notes |
|---|---|---|---|---|
| Therm1–Therm16 | 16 | JST-XH 3-pin header (B3B-XH-A) | Thermistor ports, 2.54 mm pitch, top entry | GND / 3V3 / Signal |
| ADXL | 1 | JST-XH 6-pin header (B6B-XH-A) | SPI / ADXL345 breakout | GND, 3V3, MOSI, MISO, SCLK, CS |
| Fan | 1 | JST-XH 2-pin header (B2B-XH-A) | 3010 fan connector | 5 V / GND |
| Power1 | 1 | Screw terminal, 2-pos, 5.08 mm pitch | 5 V power input for the Pi | e.g. Phoenix-style KF301-5.08 |
| H1 | 1 | 2×20 female stacking header (DS1023-2*20SF11) | Raspberry Pi 40-pin GPIO connector | Extra-tall / stacking style recommended for clearance |
| R1, R2 | 2 | 4.7 kΩ resistor, 1/4 W, through-hole | 1-Wire bus pull-ups (S1, S2) | 5% tolerance is fine |
| U2 | 1 | 47 µF electrolytic capacitor, ≥10 V, radial | 5 V rail bulk decoupling | Observe polarity |

## Off-Board / Assembly Hardware

| Qty | Part | Description | Notes |
|---|---|---|---|
| 1 | 3010 fan, 5 V DC | Board cooling (30 × 30 × 10 mm) | May be powered externally instead |
| up to 16 | DS18B20 temperature probe | Waterproof pre-potted probe style | Fit JST-XH 3-pin plugs to match port pinout |
| 16 | JST-XH 3-pin plug + crimp terminals | Mating connectors for probes | Pre-crimped pigtails save time |
| 4 | M2.5 × 11 mm standoff + screws | HAT mounting to the Raspberry Pi | Standard Pi HAT hardware |
| 2 | M3 screw + nut (optional) | 3010 fan mounting | Length to suit fan + board stack |
| 1 (optional) | ADXL345 accelerometer board | Input shaping via the 6-pin SPI port | Wire per the README pinout |
