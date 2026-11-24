# P1-SUN — BOM (Components Specification)

**Family:** FPV Kamikaze / Interceptor (wing/quad 1–10 kg)
**Manufacturer:** SkyFall
**Status:** Fielded
**Sourcing date:** 2026-11-23 (prices/availability verified on this date)

## Key specs (from catalog)

> Base model 310 km/h; JetKiller variant 370 km/h for jet-powered drones 5,500+ Russian drones destroyed since November 2025 (company figure) About $3,000 per unit (Ukrainian MoD adviser, April 2026)
>
> SkyFall overview: SkyFall, founded in 2022, is one of Ukraine's largest drone makers. Its P1-SUN interceptor entered combat in November 2025 and, according to the company, has destroyed more than 5,500 Russian drones. In July 2026 SkyFall unveiled the P1-SUN JetKiller at Farnborough: a 370 km/h version built to catch Russia's new jet-powered drones, which shot down its first Geran-5 in late September 2026. The company says it can build up to 50,000 interceptors a month, and in June 2026 it signed a memorandum with Airbus Defence and Space on linking P1-SUN to Airbus command-and-control software. On 9 October 2026 Japan's Defense Minister Shinjiro Koizumi announced that his ministry had signed a contract to buy SkyFall interceptor drones; the model, quantity and value were not disclosed. In November 2026 SkyFall and the US avionics company Auterion announced a joint venture to build drones for Ukraine at a new German-funded factory in Germany, starting with Shrike FPV drones and later adding P1-SUN; the partners say they have already delivered more than 50,000 Shrike drones together.
>
> Sources — Defender Media, 20 Nov 2026 — Kyiv Independent, Jul 2026 — Breaking Defense, Jul 2026 — Forbes Ukraine via Euromaidan Press, 24 Apr 2026 — Defender Media, 10 Oct 2026 — Militarnyi, 10 Oct 2026
>
> Public figures as reported by the company and the press, with dates. Independent verification is part of our vetting process and is shared with counterparties under NDA.
>
> More from the ecosystem: view all 162 companies → Sting Anti-Shahed Interceptor Drone

## BOM — node level (FPV Kamikaze/Interceptor (wing/quad 1–10 kg), family reference)

| ID | Node | Component (recommended) | MPN/Model | Alternative | Qty | Weight, g | Price min, $ | Price max, $ | Suppliers | Verification |
|---|---|---|---|---|---|---|---|---|---|---|
| C-001 | Frame and housing | Custom monocoque (3D print PA12-CF) | PA12-CF (Bambu PAHT-CF16 / Ultimaker Nylon CF) | PETG-CF + carbon 5–6 mm | 1 | 500 | 40 | 60 | 3D printing service / AliExpress | estimate |
| C-002 | Powertrain | Brushless 2812 1350–1500KV | T-Motor F90 2806.5 1500KV ($29–37, AliExpress in stock) | Hobbywing Xrotor 2807 1500KV ($49/kit) | 4 | 300 | 116 | 150 | AliExpress / T-Motor Store / RC-Store (UA) | verified |
| C-003 | ESC 4-in-1 80A 4–8S BLHeli_32/AM32 | Axisflying ARGUS PRO 100A (5 900 UAH RC-Store UA) / UniFly 80A ($87) | T-Motor Cine C 80A ($370); ⚠ Tekko32 F4 80A discontinued | 1 | 45 | 87 | 140 | RC-Store (UA) / AliExpress | verified |
| C-004 | Propellers | Propeller 7x6E / 8x6E | Gemfan Vortex 7x6E ($1,2) / APC 8x6E ($2,99 genuine GetFPV) | HQProp 7.5X5 ($4) | 4 | 40 | 5 | 25 | AliExpress / GetFPV / RC-Store (UA) | verified |
| C-005 | Battery pack | Assembly 8S2P Molicel P45B (21700) | Molicel INR21700-P45B — NKON €4,55/cell (€3,92@600); IMR $5,99 | Samsung INR21700-50S — NKON €3,75/cell | 1 | 1180 | 72 | 110 | NKON (NL) / IMR Batteries (US) / RC-Store (UA) | verified |
| C-006 | Flight controller | Matek H743-SLIM V3 (⚠ being replaced with V4 — take live stock) | Matek H743-SLIM V3 — AliExpress $91 in stock | SpeedyBee F405 / H743-SLIM V4 | 1 | 15 | 55 | 91 | AliExpress (live V3 stock) / mateksys.com | verified |
| C-007 | Navigation and speed | Matek M10Q-5883 (GNSS M10 + antenna) + Pitot tube | M10Q-5883 + TE 4525DO-DS5AI001DP | BN-880 (u-blox M8N) + Pitot MS4525DO | 1 | 25 | 45 | 65 | mateksys.com / DigiKey / Newark | verified |
| C-008 | Control system (Link) | ExpressLRS 868/915 MHz 0,5–1 W | HappyModel ES900TX ($25; ⚠ ES915TX discontinued) | GEPRC LINKFLOW Dual-Band 1W (€41,58, pre-order) | 1 | 35 | 25 | 45 | AliExpress / Drone-FPV-Racer (EU) | verified |
| C-009 | FPV system | Foxeer T-Rex Micro + VTX 2,5–3 W | Foxeer T-Rex ($104–139) + Rush Tank Solo 2,5W ($43) / METELYK 3W (UA, 3 000 UAH) | Walksnail / HDZero | 1 | 60 | 43 | 139 | AliExpress / RC-Store (UA, METELYK — Ukrainian) | verified |
| C-010 | Guidance module (option) | Raspberry Pi CM4 + Global Shutter camera | RPi CM4104032 + Arducam OV9281 ($113–143, AliExpress) | Jetson Orin Nano / OV9281-compatible $20 | 1 | 120 | 102 | 250 | RAKwireless (CM4) / AliExpress (OV9281) | verified |

**BOM total (max prices, per unit): ≈ $1,600**

## Price and availability at specific sellers (2026-11-23)

| ID | Part | Seller | Price | Availability | Link |
|---|---|---|---|---|---|
| C-001 | Filament PA12-CF PAHT-CF (Bambu) | Bambu Lab US Store | $49.99 (0,5 kg) / $94.99 (1 kg) | In stock | https://us.store.bambulab.com/collections/bambu-lab-3d-printer-filament/products/paht-cf |
| C-001 | Filament Nylon CF 2,85 mm (UltiMaker) | InkMechanic (US) | $49.50 (750 g, sale) | In stock | https://www.inkmechanic.com/product/ultimaker-nylon-cf-slide-filament-2-85mm-75kg-black/ |
| C-001 | NylonX PA12-CF (MatterHackers) | MatterHackers (US) | $63.00 (0,5 kg); BASF PAHT CF15 $116 | Listing active | https://www.matterhackers.com/store/c/300mm-nylon-filament |
| C-002 | T-Motor F90 2806.5 1500KV | AliExpress | 1 199,19 UAH (~$29) | In stock (144 sold) | https://www.aliexpress.com/item/1005008694971583.html |
| C-002 | T-Motor F90 2806.5 (T-Hobby) | AliExpress | 1 240,19 UAH (~$30) | In stock | https://www.aliexpress.com/item/1005007988873860.html |
| C-002 | Hobbywing Xrotor 2807 1500KV (4 pcs) | AliExpress | 2 072,35 UAH (~$49/kit) | In stock (70 sold) | https://www.aliexpress.com/item/1005011931845755.html |
| C-003 | ⚠ Tekko32 F4 80A — DISCONTINUED | — | — | Discontinued (no verified sellers) | — |
| C-003 | Axisflying ARGUS PRO 100A ESC 4-8S | RC Store (Kyiv, UA) | 8 290 UAH (sale 5 900 UAH) | In stock | https://rc-store.com.ua/index.php?route=product/product&product_id=11710 |
| C-003 | UniFly 80A 3-8S 4-in-1 32bit | AliExpress | 3 664,39 UAH (~$87) | In stock | https://www.aliexpress.com/item/1005012798860734.html |
| C-003 | T-Motor Cine C 80A 4IN1 4-8S BLHeli32 | AliExpress | 15 533,69 UAH (~$370) | In stock | https://www.aliexpress.com/item/1005012780554522.html |
| C-004 | ⚠ APC 7x6E original — not at verified sellers | — | — | Not available (GetFPV carries 7x5E/8x6E) | — |
| C-004 | Gemfan Vortex 7x6E CCW (APC clone) | AliExpress | 51,44 UAH (~$1,2) | In stock (79 sold) | https://www.aliexpress.com/item/1005008067853738.html |
| C-004 | APC 8x6E Speed (original) | GetFPV (US) | $2.99 | In stock | https://www.getfpv.com/apc-8x6e-speed-propeller.html |
| C-004 | HQProp 7.5X5 7550 | AliExpress | 168,79 UAH (~$4) | In stock | https://www.aliexpress.com/item/1005012569179346.html |
| C-005 | Molicel INR21700-P45B 4500mAh 45A | NKON (NL) | €4.55 (€4.25@10+; €3.92@600) | In stock (page verified) | https://www.nkon.nl/en/catalogsearch/result/?q=p45b |
| C-005 | Molicel P45B | IMR Batteries (US) | $5.99 | In stock | https://imrbatteries.com/products/molicel-p45b-21700-4500mah-45a-battery |
| C-005 | FLYWOO 6S1P 4500mAh (P45B) pack | RC Store (UA) | 2 520 UAH; 6S2P 9000 mAh — 4 540 UAH | In stock | https://rc-store.com.ua/akkumulyator-flywoo-explorer-molicell-p45b-21700-6s1p-4500mah-lionpack-battery |
| C-005 | Samsung INR21700-50S 5000mAh 35A | NKON (NL) | €3.75 | In stock | https://www.nkon.nl/en/samsung-inr21700-50s-5000mah-35a.html |
| C-006 | Matek H743-SLIM V3 | AliExpress | 3 813,99 UAH (~$91) | In stock (listing active) | https://www.aliexpress.com/item/1005013116095997.html |
| C-006 | Matek H743-SLIM V3 | GetFPV (US) | $126.49 | Not in stock (V3 → V4) | https://www.getfpv.com/mateksys-h743-slim-v3-flight-controller.html |
| C-006 | Matek H743-SLIM V4 (replacement for V3) | Drone-FPV-Racer (EU) | €79.92 | Not in stock | https://www.drone-fpv-racer.com/en/matek-flight-controller-h743-slim-v4-14439.html |
| C-007 | MS4525DO (Pitot sensor) | Newark (element14) | $84.63 (1 pc); $71.39@100 | 357 pcs in stock (+280 in transit) | https://www.newark.com/te-connectivity/4525do-ds5ai001dp/pressure-sensor-differential-1psi/dp/24AJ4146 |
| C-007 | MS4525DO | DigiKey | $72.41 | 0 pcs; 10 pcs by 25.03.2027 (33 weeks) | https://www.digikey.com/en/products/detail/te-connectivity-measurement-specialties/4525DO-DS5AI001DP/3569051 |
| C-007 | MS4525DO (Holybro airspeed kit) | 3DXR (UK) | £67.65 incl. VAT | 93–134 pcs in stock | https://www.3dxr.co.uk/products/holybro-digital-airspeed-sensor-ms4525do |
| C-008 | ⚠ ES915TX discontinued — replacement ES900TX | AliExpress | 1 032,46 UAH (~$25) | In stock (102 sold) | https://www.aliexpress.com/item/1005008115926551.html |
| C-008 | GEPRC LINKFLOW Dual-Band 915M/2.4G ELRS 1000mW | Drone-FPV-Racer (EU) | €41.58 | Pre-order (end of November) | https://www.drone-fpv-racer.com/en/geprc-linkflow-dual-band-915-m-2-4g-expresslrs-1000mw-tx-module-15545.html |
| C-008 | ⚠ ELRS receiver 915 MHz — not EP1/EP2 (those are 2.4G only); iFlight ELRS Nano RX 915 | RC Store (UA) | 900 UAH | In stock | https://rc-store.com.ua/peredavach-ifligh-expresslrs-elrs-nano-receiver |
| C-008 | BetaFPV SuperD RX ELRS 2.4G/915/868 | RC Store (UA) | 950 UAH | In stock | https://rc-store.com.ua/pryimach-betafpv-superd-rx-elrs |
| C-008 | Namimno N900R ELRS 915 MHz Flash mini RX | AliExpress | 468,49 UAH (~$11) | In stock | https://www.aliexpress.com/item/1005007051063737.html |
| C-008 | Foxeer ELRS 915/868 Diversity RX | Drone-FPV-Racer (EU) | €21.58 | In stock | https://www.drone-fpv-racer.com/en/foxeer-elrs-915-868mhz-diversity-receiver-fpv-receiver-15727.html |
| C-009 | Foxeer T-Rex Micro 1500TVL | AliExpress | 4 371,90 UAH (~$104) | In stock | https://www.aliexpress.com/item/1005012142592084.html |
| C-009 | RUSH TANK SOLO 2.5W 5.8GHz 48CH | AliExpress | 1 805,19 UAH (~$43) | In stock (45 sold) | https://www.aliexpress.com/item/1005010692671172.html |
| C-009 | METELYK VTX 5.8 GHz 3 W (Ukrainian) | RC Store (UA) | 3 000 UAH | In stock | https://rc-store.com.ua/vіdeoperedavach-metelyk-vtx-58ghz-3w |
| C-010 | Raspberry Pi CM4 (CM4104032) | DigiKey | $130.00 | Not in stock (replacement CM5 SC2691 — 247 pcs) | https://www.digikey.com/en/products/detail/raspberry-pi/SC0674/13530933 |
| C-010 | Raspberry Pi CM4 | RAKwireless Store | $102.00 (2GB/16GB) | In stock (2GB/16GB); 4/8GB sold out | https://store.rakwireless.com/products/raspberry-pi-compute-module-4 |
| C-010 | Raspberry Pi Zero 2 W | Kubii (FR) | €18.00 | In stock | https://kubii.com/en/raspberry-pi-boards/3455-raspberry-pi-zero-2-w-5056561800004.html |
| C-010 | Jetson Orin Nano Dev Kit (Super 8GB) | SparkFun | $399.00 | In stock | https://www.sparkfun.com/nvidia-jetson-orin-nano-developer-kit.html |
| C-010 | Jetson Orin Nano Super Dev Kit | Arrow | €365.22 (1 pc) | 1 pc, ship from the USA | https://www.arrow.com/en/products/945-13766-0007-000/nvidia.html |
| C-010 | Arducam OV9281 mono global shutter + 850nm IR | AliExpress | 4 758,90 UAH (~$113) | In stock | https://www.aliexpress.com/item/1005012828096588.html |
| C-010 | OV9281 RPi-compatible Global Shutter (not Arducam) | AliExpress | 843,99 UAH (~$20) | In stock (29 sold) | https://www.aliexpress.com/item/1005009848925170.html |

---

For further information about the products, please contact us using the details provided:

Session: 057a9aa43e25a8fb684ce9e0d7a766ee33430e2ea5c247a3bc1a42d9bd08ec8d4f
Threema: 2MCXH9UB
