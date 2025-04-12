# Peugeot 508 window wiper motor - water damage repair

> [!CAUTION]
> The content in this document only serves as a repair guide and in no event shall the author be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with this document or the use or other dealings in this document.

## What's the fuzz all about?

If you read this you might have experienced on a rainy day out driving that your front left window wiper all of a sudden just wipes half of your windshield and the right window wiper seems dead. You drive to your local mechanic and get told they will have to replace both window wipers. It will cost you quite a bit more than you are comfortable paying for to fix something seemingly simple as a defective window wiper motor (£2000 or similar). You might get the idea to find a used wiper motor from a scrapped car which is when you will get the next shock. The price for a dirty old used window wiper motor for this specific car model is more than the price of a new wiper motor for any other car. The reason for this is that it's a highly common problem that these fail on the Peugeot 508 and used parts are short in supply. It's simply a design flaw by Peugeot and boils down to the lack of protection above the wiper motor which make the motor openly exposed to **rain** (go figure). Especially the left wiper motor which seems to **almost always** be the culprit. A side effect of this can also be other errors showing up like airbag and passenger seat detection, this is because the indicator lamps for these functions are connected to the same communication line (LIN bus) as the wipers, and when this line is shorted that will be the result. But don't worry, these errors will also disappear once the wiper motor is fixed.

Over time the aluminum block part of the Bosch WDA motor corrodes and pushes the plastic cover away from the aluminum block, breaching the rubber gasket between the two parts and water gets into the motor, quickly corroding electronics when they are powered. Also, from my experience, it seems the rubber seal around the axle of the motor itself dries/rots over time and water will also find its way through there.

The reason for why your local dealer/workshop says you need to replace both wiper motors is that the parts they sell are always a newer version (different MCU and firmware and the old version is discontinued). Since these two wiper motors need to communicate with each other and there are slight differences in the communication protocol, the old wiper motors are incompatible with the new versions. Hence both needs replacement to the new version, unless you fix it yourself.

If you buy a dirty old second hand wiper motor, it's likely that it has already started to corrode and the problem might surface yet again in the near future. You may consider to open it up and clean the edges for corrosion and clean/refresh/replace the rubber gasket. The most difficult part of the disassembly is to get the plastic cover separated from the motor housing, do not use force and be really careful when removing the electrical motor brush assembly, this is connected to the circuit board and you will break the wires connecting the brush assembly to the circuit board if you're not careful enough. 

<div class="grid cards" markdown>

- Remove left side motor from car ([PDF of removal instructions](assets/508_wipers_remove_refit.pdf))

	![](assets/397_021_550_in_car.jpg)

	---

- Back side of the left side motor with part numbers.

	![](assets/1_397_220_614_case_back.jpg)

	---

- Remove the clamps using a flat screwdriver and carefully separate the plastic housing from the motor housing ([YouTube video made by someone else to get an idea on how to do this right](https://www.youtube.com/watch?v=EBXXZTmN6M8)), it's usually corroded and can be a bit stuck, be patient and careful.

	![](assets/1_397_220_614_case_disassembly.jpg)

	---

-  Oh boy does this look corroded, any hope?

	![](assets/1_397_220_614_pcb_lqdmg_2_opened.jpg)

	---

- First example, corroded 1 397 220 614 PCB top view.

	![](assets/1_397_220_614_pcb_lqdmg_2_in_case.jpg)

	---

- First example, corroded 1 397 220 614 PCB bottom view, corrosion is always worse here as this is where the water usually ends up.

	![](assets/1_397_220_614_pcb_lqdmg_2_bottom.jpg)

	---

- First example, repaired 1 397 220 614 PCB top view, replaced shorted components and added wires fixing corroded tracks.

	![](assets/1_397_220_614_pcb_lqdmg_2_after_top.jpg)

	---

- First example, repaired 1 397 220 614 PCB bottom view, replaced shorted components and added wires fixing corroded tracks.

	![](assets/1_397_220_614_pcb_lqdmg_2_after_bottom.jpg)

	---

- Second example, corroded 1 397 220 614 PCB top view.

	![](assets/1_397_220_614_pcb_lqdmg_1_in_case.jpg)

	---

- Second example, corroded 1 397 220 614 PCB bottom view, this is a corrosive disaster, can this at all be repaired?

	![](assets/1_397_220_614_pcb_lqdmg_1_bottom.jpg)

	---

- Second example, microscope view of extremely corroded BOSCH D0865FD microcontroller.

	![](assets/1_397_220_614_pcb_lqdmg_1_chip.jpg)

	---

- Second example, microscope view of BOSCH D0865FD microcontroller after cleanup, on this one I had to drill using a small diamond ball tip to expose the track for a broken pin under the chip's protective epoxy resin in order to get a clean point to solder a new wire to.

	![](assets/1_397_220_614_pcb_lqdmg_1_chip_drill.jpg)

	---

- Second example, cleaned up 1 397 220 614 PCB and chip. Flux and heat is your friend.

	![](assets/1_397_220_614_pcb_lqdmg_1_clean.jpg)

	---

- Second example, repaired 1 397 220 614 PCB top view, replaced shorted components and added wires fixing corroded tracks.

	![](assets/1_397_220_614_pcb_lqdmg_1_after_top.jpg)

	---

- Second example, repaired 1 397 220 614 PCB bottom view, replaced shorted components and added wires fixing corroded tracks. Also using some epoxy here to hold a wire bridge properly in place over a corroded track.

	![](assets/1_397_220_614_pcb_lqdmg_1_after_bottom.jpg)

	---


- Third example, corroded 1 397 220 614 PCB top view.

	![](assets/1_397_220_614_pcb_lqdmg_3_in_case.jpg)

	---

- Third example, repaired 1 397 220 614 PCB top view, replaced shorted components and added wires fixing corroded tracks.

	![](assets/1_397_220_614_pcb_lqdmg_3_after_top.jpg)

	---

- Third example, repaired 1 397 220 614 PCB bottom view, replaced shorted components and added wires fixing corroded tracks. Using more epoxy to protect components better from future corrosion. Hindsight this actually might not be a good idea, because the if a new leak occurs, water will just keep filling the case and reach other components, like the microcontroller and even cause more damage before noticing it.

	![](assets/1_397_220_614_pcb_lqdmg_3_after_bottom.jpg)

	---

- Third example, corroded motor housing before cleanup.

	![](assets/1_397_220_614_pcb_lqdmg_3_housing.jpg)

	---

- Third example, corroded motor housing after cleanup using a steel wire wheel brush on a drill, this should be done to get a proper seal when re-assembling it. You might also try using additional sealant like liquid rubber waterproof sealant, silicon or similar to get it completely sealed up.

	![](assets/1_397_220_614_pcb_lqdmg_3_housing_after.jpg)

	---

- Sometimes the pins connecting the plastic case connector to the PCB will also be severely corroded and might need some fix-up. Here I have removed plastic around the pin and cleaned the area in order to get a good and clean soldering point to repair the pin.

	![](assets/1_397_220_614_case_pin_fix_1.jpg)

	---

- In this example just cut and shaped a part of a U-type cable shoe to extend and repair the pin. Be creative.

	![](assets/1_397_220_614_case_pin_fix_2.jpg)

	---

- The result looks clean and solid enough.

	![](assets/1_397_220_614_case_pin_fix_3.jpg)

	---

- Sometimes you might also want to replace the motor housing, if eg. the motor is burnt/rusted/stuck or you may suspect the axle seal to also be an issue where water may leak in.

	![](assets/397_021_550_screws_and_angle.jpg)

	---

- You may use the motor housing from Bosch WDA wipers used in other car models/brands, se a more detailed list further below. In this example I used motor housing from a Skoda Octavia (much cheaper to get). Keep in mind this applies only to the motor housing and brush assembly, not the PCB and plastic casing.

	![](assets/Peugeot_508_Skoda_side-by-side.jpg)
	![](assets/Peugeot_508_Skoda_side-by-side2.jpg)

- This is a simple schematic I sketched up for the LIN bus protection circuit, which is the first thing that usually shorts and causes errors on everything else connected to the same bus like the airbag lamps and passenger seat detection lamps shown in the middle mirror unit. This is also why you will see airbag failure warnings amongst other things when turning on the ignition when you have a water damaged window wiper motor.

	![](assets/datasheet_lin.png)

	---

- There's no publicly available schematic for this PCB, so I've measured and figured out the types and values for the most critical components that usually get corroded and shorted, thus need replacement.

	![](assets/1_397_220_614_pcb_comp_bottom.png)
	![](assets/1_397_220_614_pcb_comp_top.png)

</div>

## Component identification

Below is a list of relevant components on the 1 397 220 613 / 1 397 220 614 Bosch WDA motor PCB that are critical for its function and that is most likely to be damaged when water leaks into the motor assembly. Components on the LIN Bus lines are most likely to suffer first due to how the motor is mounted to the car chassis (slightly tilted, making all the water collect in one place once water leaks to the inside).

First listed are two ICs, pins on the main MCU (D0865FD) is susceptible to some corrosion damage if the leakage has been severe. Alternatives to the components are listed under each component.

D0865FD - BOSCH microcontroller for WDA motion control, LIN Bus communication (pin 5, 40, 41, 42, 44 are LIN Bus related) `[TQFP44]`
- no datasheet available to the public
- these have custom firmware and can't just be replaced with a new chip, if replacement is needed it needs to be from a donor board of the same type motor (wipe angles and if it's a single or dual master/slave setup are all parts of firmware configuration)
- Peugeot 508 2014-2018 (Type I, Fase 2) uses wiper motors with part number 1 397 220 694 / 1 397 220 695, MCU on these are the [Infinion TLE9868QXB20](https://www.infineon.com/cms/de/product/microcontroller/embedded-power-ics-system-on-chip-/h-bridge-driver-integrated-arm-cortex-m3/tle9868qxb20/) `[VQFN-48-79]` [link to datasheet here](assets/datasheets/Infineon-TLE9868QXB20-DataSheet-v02_00-EN.pdf), which is why Peugeot will replace both wiper motors on older cars (<2014) even if just one fails, possibly differences in LIN Bus communication between them (not to be considered as a chip replacement alternative, PCB is completely different and different chip package)

[KMZ43T](assets/datasheets/KMZ43T.pdf) - NXP, Magnetic field sensor

> [!NOTE]
> Possible alternative: [AA747](assets/datasheets/SENSITEC_AA747_DSE_08.pdf) - Sensitec, MagnetoResistive Angle Sensor

QN0406 - [IPD80N04S3-06](assets/datasheets/Infineon-IPD80N04S3_06-DS-v01_00-en.pdf) 40V N-Channel Enhancement mode MOSFET `[automotive]`

> [!NOTE]
> Possible alternative: [DMTH4005SK3Q-13](assets/datasheets/DMTH4005SK3Q.pdf) `[automotive]`

27E - Dual Line CAN Bus Protector [NUP2105LT1](assets/datasheets/nup2105l-d.pdf)

> [!NOTE]
> Possible alternative is one with marking 6X that I've seen used on another board at the same spot where 27E should be (on a right side motor).

> [!TIP]
> Other CAN/LIN Bus ESD protectors may also work, like [PESD2IVN24T-Q](assets/datasheets/PESD2IVN24T-Q.pdf) (LIN bus specifically mentioned in datasheet)

No datasheets are available for the Wxx components listed below, but they are identified and alternatives are listed under. I suspect they are made by Philips/Nexperia and W prefix = made in China, but they might be "rare" markings from around 2008-2012ish and only available for the automotive industry (just a guess since it's impossible to find documentation on them).

WZR - High-speed switching double diode (series) (100V, 125mA) `[SOT-23]`

**Possible alternatives:**

| Marking | Type + Link to datasheet                   | Grade      | Comment                                                                                                                                                                  |
|---------|--------------------------------------------|------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| A7*     | [BAV99-Q](assets/datasheets/BAV99-Q.pdf)   | automotive | used as replacement by the manufacturer for WZR on a [Volvo alarm PCB](https://elektronikforumet.com/forum/viewtopic.php?t=72490) (difference from an earlier/later PCB) |
| *V1     | [BAS31](assets/datasheets/BAS29_31_35.pdf) |            |                                                                                                                                                                          |
| *5C     | [PMBD7000](assets/datasheets/PMBD7000.pdf) | automotive |                                                                                                                                                                          |
| KJE     | [BAV99-Q](assets/datasheets/BAV99.pdf)     |            |                                                                                                                                                                          |

WZE - High-voltage switching diode (single) (250V, 200mA) `[SOT-23]`

**Possible alternatives:**

| Marking | Type + Link to datasheet                   | Grade      | Comment                                                                                                      |
|---------|--------------------------------------------|------------|--------------------------------------------------------------------------------------------------------------|
| %HQ     | [BAS101-Q](assets/datasheets/BAS101-Q.pdf) | automotive |                                                                                                              |
| JS%     | [BAS21-Q](assets/datasheets/BAS21-Q.pdf)   | automotive | this is used on a newer version of the board (Infinion MCU), has several JSt, also in close proximity to WYA |

WYA - NPN general-purpose transistor (45 V, 500 mA) `[SOT-23]`

**Possible alternatives:**

| Marking | Type + Link to datasheet                        | Grade      | Comment                                                                                                      |
|---------|-------------------------------------------------|------------|--------------------------------------------------------------------------------------------------------------|
| 6C*     | [BC817-40-Q](assets/datasheets/BC817-Q_SER.pdf) | automotive | 6Cs̱ (lowercase s with underline, Siemens?) is used as a replacement for WYA on another PCB of the same type |
|         | [BC817-40](assets/datasheets/BC817_SER.pdf)     |            |                                                                                                              |

Below are some other components in same era that have similar markings, not used for the Bosch WDA but on other automotive related PCBs (this might be useful for someone as the Wxx components are almost impossible to find).

WZJ - Dual Schottky diode (common cathode) `[SOT-23]`

**Possible alternative:**

| Marking | Type + Link to datasheet                       | Grade      |
|---------|------------------------------------------------|------------|
| 45%     | [BAS40-05-Q](assets/datasheets/BAS40-05-Q.pdf) | automotive |

WZP - High-speed switching double diode (common cathode) `[SOT-23]`

**Possible alternative:**

| Marking | Type + Link to datasheet                 | Grade      |
|---------|------------------------------------------|------------|
| A4s     | [BAV70-Q](assets/datasheets/BAV70-Q.pdf) | automotive |

WYB - NPN general-purpose transistor (65V, 100 mA) `[SOT-23]`

**Possible alternative:**

| Marking | Type + Link to datasheet                       | Grade      |
|---------|------------------------------------------------|------------|
| 1Bp     | [BC846B-Q](assets/datasheets/BC846X-Q_SER.pdf) | automotive |

**Possible alternative:**

WYG - PNP general-purpose transistor (65V, 100 mA) `[SOT-23]`
- 3Bp  `[automotive]`

| Marking | Type + Link to datasheet                                  | Grade      |
|---------|-----------------------------------------------------------|------------|
| 3Bp     | [BC856B-Q](assets/datasheets/BC856-Q_BC857-Q_BC858-Q.pdf) | automotive |


```
NXP manufacturing site code

* = -: made in Hong Kong
* = p: made in Hong Kong 
* = t: made in Malaysia
* = W: made in China

Note that NXP manufacturing site code can be either prefix or suffix.

Example: A7W and W5C

Any numbers written behind this 3-character code is production year/month.
```

```
Diodes Incorporated

Product Type Marking Code: K**

Example: KJE

Any numbers written behind this 3-character code is production year/month.
```

Some of the Wxx SOT-23 components are identified using a simple component tester, cross referencing the values and using educated guesswork to find equivalent components.

![](assets/component_tester.jpg)

# DigiKey order list for the most likely components to be damaged

This is a selection of components that are most likely to be damaged and needed to fix your corroded PCB. Most parts here are of automotive grade which usually are a bit more expensive, but they at least fall within spec of the original design. I have used all these parts myself on some of the repairs shown above and every repair has been successful and 100% working.

| #  | PRODUCT DETAILS                                                                                                                                                            |
|----|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1  | [SZNUP2105LT1GOSCT-ND](https://www.digikey.no/en/products/detail/onsemi/SZNUP2105LT1G/3063422) SZNUP2105LT1G TVS DIODE 24VWM 44VC SOT233                                   |
| 2  | [31-BAS21Q-13-FCT-ND](https://www.digikey.no/en/products/detail/diodes-incorporated/BAS21Q-13-F/16548952) BAS21Q-13-F DIODE STANDARD 250V 200MA SOT233                     |
| 3  | [1727-2919-1-ND](https://www.digikey.no/en/products/detail/nexperia-usa-inc/BC817-40-215/763235) BC817-40,215 TRANS NPN 45V 0.5A TO-236AB                                  |
| 4  | [1727-BAV99-QRCT-ND](https://www.digikey.no/en/products/detail/nexperia-usa-inc/BAV99-QR/15196157) BAV99-QR DIODE ARR GP 100V 215MA TO-236AB NCNR                          |
| 5  | [846-ESR03EZPF3301CT-ND](https://www.digikey.no/en/products/detail/rohm-semiconductor/ESR03EZPF3301/4007218) ESR03EZPF3301 RES 3.3K OHM 1% 1/4W 0603                       |
| 6  | [846-ESR03EZPF46R4CT-ND](https://www.digikey.no/en/products/detail/rohm-semiconductor/ESR03EZPF46R4/21731249) ESR03EZPF46R4 RES 46.4 OHM 1% 1/4W 0603                      |
| 7  | [541-RCS060338K3FKEACT-ND](https://www.digikey.no/en/products/detail/vishay-dale/RCS060338K3FKEA/5868654) RCS060338K3FKEA RES SMD 38.3K OHM 1% 1/4W 0603                   |
| 8  | [P2.87KBCCT-ND](https://www.digikey.no/en/products/detail/panasonic-electronic-components/ERA-8AEB2871V/3070938) ERA-8AEB2871V RES SMD 2.87K OHM 0.1% 1/4W 1206            |
| 9  | [490-GCM1885G2A101FA16DCT-ND](https://www.digikey.no/en/products/detail/murata-electronics/GCM1885G2A101FA16D/13401802) GCM1885G2A101FA16D CAP CER 100PF 100V X8G 0603     |
| 10 | [490-16409-1-ND](https://www.digikey.no/en/products/detail/murata-electronics/GCM1885C2A330FA16D/7363153) GCM1885C2A330FA16D CAP CER 33PF 100V C0G/NP0 0603                |
| 11 | [490-GCM1885C2A471FA16DCT-ND](https://www.digikey.no/en/products/detail/murata-electronics/GCM1885C2A471FA16D/11618802) GCM1885C2A471FA16D CAP CER 470PF 100V C0G/NP0 0603 |
| 12 | [399-C0603C473J1RECAUTOCT-ND](https://www.digikey.no/en/products/detail/kemet/C0603C473J1RECAUTO/6825898) C0603C473J1RECAUTO CAP CER 0.047UF 100V X7R 0603                 |
| 13 | [399-C0805C512F4HACAUTOCT-ND](https://www.digikey.no/en/products/detail/kemet/C0805C512F4HACAUTO/7958369) C0805C512F4HACAUTO CAP CER 0805 5.1NF 16V ULTRA STA              |
| 14 | [445-MPZ1608D300BTD25CT-ND](https://www.digikey.no/en/products/detail/tdk-corporation/MPZ1608D300BTD25/5040309) MPZ1608D300BTD25 FERRITE BEAD 30 OHM 0603 1LN              |

# Below is a list of wiper motors and their part codes

## Peugeot 508 2011 - 2014

	1 397 220 614 - driver side (left)		[9677472580] [9816172780]
	1 397 220 613 - passenger side (right)	[9677472680] [9816172680]

## Peugeot 508 2014<

	1 397 220 694 - driver side (left)
	1 397 220 695 - passenger side (right)

> These may need calibration in Diagbox / Peugeot Planet if fitted in a Peugeot 508 < 2014

## Hardware / firmware info

The wiper motor for Peugeot 508 comes in two versions, number on motor is found on the black plastic cover on the electrical motor itself, number on mechanism is found on a white label next to one of the mounting screws. You can replace the motor with another motor with the same part number without doing anything else (no "sync" or use of diagnostic software needed). You can **not** directly replace just one motor of the old type with a motor of the new type since they are incompatible, both motors must have the same HW/SW.

| Number on motor | Number on mechanism | Side  | HW/SW           | Car model / year               |
|-----------------|---------------------|-------|-----------------|--------------------------------|
| 1 397 220 614   | 3 397 021 551       | left  | HW 1.1 - SW 1.8 | 508 2011-2014 (Type I, Fase 1) |
| 1 397 220 613   | 3 397 021 550       | right | HW 1.1 - SW 1.8 | 508 2011-2014 (Type I, Fase 1) |
| 1 397 220 694   | 3 397 021 927       | left  | HW 2.0 - SW 2.1 | 508 2014-2018 (Type I, Fase 2) |
| 1 397 220 695   | 3 397 021 928       | right | HW 2.0 - SW 2.1 | 508 2014-2018 (Type I, Fase 2) |

## Other motors of the same type

The common product number is 1 397 220 xxx and there are MANY of these motors. Most of them are used in single motor systems with mechanics linking the two wipers. These are calibrated with a completely different range of motion than what is used for dual motor systems. Dual motor systems work as a master/slave setup and need to be synchronized in order to prevent wiper overlap (wipers crashing in to each other). Older motor units with part number from about 1 397 220 5xx to 1 397 220 68x uses the BOSCH D0865FD MCU while newer motor units with part number from about 1 397 220 69x to 1 397 220 7xx uses the [Infinion TLE9868QXB20](https://www.infineon.com/cms/de/product/microcontroller/embedded-power-ics-system-on-chip-/h-bridge-driver-integrated-arm-cortex-m3/tle9868qxb20/) MCU ([datasheet](assets/datasheets/Infineon-TLE9868QXB20-DataSheet-v02_00-EN.pdf)).

This list may be useful in case you need a new motor housing or brush assembly, these may work as replacements (but NOT the PCB and probably not the plastic housing as the connectors tend to differ).

### Peugeot 3008, 2009-2016 (Type I)

	1 397 220 576 - driver side (left)
	1 397 220 577 - passenger side (right)

### Peugeot 5008, 2010-2017 (Type I)

	1 397 220 576 - driver side (left)
	1 397 220 577 - passenger side (right)

### Skoda Octavia 2017-2020 (Type III, Fase 2)

	1 397 220 712 - motor housing and brushes might fit Peugeot 508 Left

### Audi Q3, 2011-2014 (Type I, Phase 1)

	1 397 220 615 - motor housing and brushes might fit Peugeot 508 Left

One motor system with mechanics driving two wipers

### Volvo V40, 2012-2019

	1 397 220 628 - motor housing and brushes might fit Peugeot 508 Left

One motor system with mechanics driving two wipers

### VW Golf VII, 2012-2017 (Phase 1)

	1 397 220 663 - motor housing and brushes might fit Peugeot 508 Left

One motor system with mechanics driving two wipers

### Mercedes C class, 2014< (W205)

	1 397 220 696 - motor housing and brushes might fit Peugeot 508 Right

One motor system with mechanics driving two wipers

### AUDI Q7 2015< (4LB)

	1 397 220 697 - motor housing and brushes might fit Peugeot 508 Right

One motor system with mechanics driving two wipers

# [Bosch Wiper motor WDA](https://www.bosch-motorsport.com/content/downloads/Raceparts/en-GB/50954635117964683.html)

- The WDA is a wiper motor designed to execute reversing movements instead of rotating 360° like a conventional wiper.

- Its function and many operating modes are managed by integrated control electronics. The user is able to control the desired operating mode simply by switching its analog inputs to ground (Analog version) or via LIN (LIN version). The gear, the motor and the electronics are all installed in the same housing.

- The main benefit of this wiper motor is its direct rotation movement which replaces external gears and the possibility of programming the operating speed and end positions of all its function modes, upon request.

- The WDA LIN can be operated by all ECUs with LIN 2.X Master function. Further information about the LIN-Frame available upon request.

- Make sure that the wiper is in its workspace when restarting after a power failure (upper and lower limit).

- LIN ID 0x32 (Tx) is used for internal WDA diagnostic purposes. Make sure that the LIN ID 0x32 is not used in your LIN network by any other device.

[Datasheet](assets/datasheets/Data_Sheet_68715659_Wiper_Direct_Actuator_WDA.pdf)

[Calibration Sheet](assets/datasheets/Calibration_Sheet_68717323_Wiper_Direct_Actuator_WDA.pdf)

[Offer Drawing WDA LIN](assets/datasheets/Offer_Drawing_WDA_LIN_304931467_Wiper_Direct_Actuator_WDA.pdf)

[3D Data](https://www.bosch-motorsport.com/content/downloads/Raceparts/Resources/zip/3D%20Data_68718987.zip)

| WDA LIN Operating modes |
|-------------------------|
| Stop                    |
| Interval                |
| Speed 1                 |
| Speed 2                 |
| Single stroke           |

| Electrical Data                  |            |
|----------------------------------|------------|
| Power supply                     | 9 to 16 V  |
| Supply current at 40 cycles/min. | Typ. 3.4 A |
| Supply current at 60 cycles/min. | Typ. 6.3 A |

| Mechanical Data      |                         |
|----------------------|-------------------------|
| Max. wipe cycles/min | Depending on wipe angle |
| Max. wipe angle      | 160°                    |
| Max. torque          | 35 Nm                   |
| Weight               | 1,270 g                 |

| Connectors and Wires |                 |
|----------------------|-----------------|
| Connector            | CEP2M-AMP-4     |
| Mating connector     | F02U.B00.542-01 |

| Pinout LIN |               |
|------------|---------------|
| Pin 1      | LIN           |
| Pin 2      | Not connected |
| Pin 3      | Gnd           |
| Pin 4      | US            |

| LIN Protocol |            |
|--------------|------------|
| LIN Version  | 2.0        |
| LIN Speed    | 19.2 kbaud |
| Message ID   | 0x31       |

| BYTE 0 Value | 0    | 0    | Kl. X | Kl. 15 | Counter    |
|--------------|------|------|-------|--------|------------|
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |
|              |      |      |       |        |            |
| BYTE 1 Value | SPD2 | SPD1 | INT   | SST    | INT Mode   |
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |
|              |      |      |       |        |            |
| BYTE 2 Value | 0    | 0    | 0     | 0      | 0  0  0  0 |
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |
|              |      |      |       |        |            |
| BYTE 3 Value | 0    | 0    | 0     | 0      | 0  0  0  0 |
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |
|              |      |      |       |        |            |
| BYTE 4 Value | 0    | 0    | 0     | 0      | 0  0  0  0 |
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |
|              |      |      |       |        |            |
| BYTE 5 Value | 0    | 0    | 0     | 0      | 0  0  0  0 |
| Bit          | 7    | 6    | 5     | 4      | 3  2  1  0 |

| Byte | Bit    | Signal   | Explanation                                                                 | Values [dez]                                 |
|------|--------|----------|-----------------------------------------------------------------------------|----------------------------------------------|
| 0    | 0 to 3 | Counter  | The counter has to be increased with each LIN-message                       | 0 to 15                                      |
| 0    | 4      | Kl. 15   | Clamp 15 Bit has to be enabled for operation                                | ON=1<br>OFF=0                                |
| 0    | 5      | Kl. X    | Clamp X Bit has to be enabled for operation                                 | ON=1<br>OFF=0                                |
| 1    | 0 to 3 | INT Mode | Interval Mode (enabled if operation mode interval is set)                   | Interval speed:<br>1=1<br>2=5<br>3=9<br>4=13 |
| 1    | 4      | SST      | Single stroke operation mode (enabled once if Bit is set temporary)         | ON=1<br>OFF=0                                |
| 1    | 5      | INT      | Operation mode interval                                                     | ON=1<br>OFF=0                                |
| 1    | 6      | SPD1     | Operation mode speed 1                                                      | ON=1<br>OFF=0                                |
| 1    | 7      | SPD2     | Operation mode speed 2                                                      | ON=1<br>OFF=0                                |
|      |        | STOP     | Operation mode stop is enabled if SST, INT, SPD1 and SPD2 are OFF (default) |                                              |

## LIN bus

[https://github.com/iDoka/awesome-linbus](https://github.com/iDoka/awesome-linbus)

[https://github.com/skpang/Teensy32_LIN-bus_master_send_demo/issues/1](https://github.com/skpang/Teensy32_LIN-bus_master_send_demo/issues/1)

## BOSCH software links

[https://github.com/boschmotorsport](https://github.com/boschmotorsport)

[https://www.downloads.bosch-automotive.com/en/ddm/esi20](https://www.downloads.bosch-automotive.com/en/ddm/esi20)

[https://help.boschdiagnostics.com/ESItronic/#/home/Requirements/en/default](https://help.boschdiagnostics.com/ESItronic/#/home/Requirements/en/default)

[https://help.boschdiagnostics.com/ESItronic/#/home/WorkstationInstallation/en/default](https://help.boschdiagnostics.com/ESItronic/#/home/WorkstationInstallation/en/default)

[https://www.peak-system.com/PLIN-View-Pro.243.0.html?&L=1](https://www.peak-system.com/PLIN-View-Pro.243.0.html?&L=1)

[https://obrcontrolsystems.com/support/](https://obrcontrolsystems.com/support/)
