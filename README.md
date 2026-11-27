# M463J Submaster Module · Summing

Ward-Beck Systems M463J, 1972|5. Wiki page: [M463J on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M463J.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 57 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 6 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 11 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 211 |
| [PHOTOS/](PHOTOS/) | photographs of the module | 1 |
| [SOFTWARE/](SOFTWARE/) | program listings, firmware, the plugin | 1 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 16 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 34 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

## Specifications

From the technical data sheet: [1972 - M463J - P002 - 1-1.jpg](MANUALS/1972%20-%20M463J%20-%20P002%20-%201-1.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Gain** | 18 dB ±0.5 dB (with fader in 15 dB &quot;in-hand&quot; position). |
| **Frequency response** | ±0.25 dB from 20 Hz to 20 kHz |
| **Noise** | 70 dB below +8 dBm nomina 1 output level (20 Hz to 20 kHz) |
| **Harmonic distortion** | Less than 0.25% THD from 30 Hz to 20 kHz at +28 dBm or Less _ (Typically Tess than 0.05% across most of bandwidth.) Source Impedance: Summing: 30,000 ohms _ balanced. Input Impedance: Summing: Less than 5 ohms _ Output Impedance: Less than 100 ohms (at 8-109A output and DIRECT output) Less than 200 ohms at MONITOR output. Load Impedance: 600 ohms balanced (at insertion point and DIRECT output). |
| **Output level** |  |
| &nbsp;&nbsp;At insertion point | -10 dBm nomina]. At DIRECT output: +8 dBm nomina] +30 dBm maximum |
| **Phasing** | Input and output terminals designated by numbers are in phase |
| **Power requirements** | +25 volts dc, 60 MA nominal, 200 mA maximum |
| **Ambient temperature** | 0 to 60 degrees Celsius _ Dimensions: 1.6&quot; wide X 7&quot; high X 6.5 &quot; deep (41 mm X 178 mm X 165 mm). |

## Circuit description

From [1972 - M463J - Submaster Module (2).pdf](MANUALS/1972%20-%20M463J%20-%20Submaster%20Module%20(2).pdf) pages 3-6 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

The M463J is designed to accept combined or mixed feeds from previously assigned mixing channel inputs. The assigned mixing channel inputs are amplified and routed to the appropriate. points within the console system.

Input and Summing Amplifier The signal originating from the external mlxlng network is applied to the summing current nodes of the input amplifier via edge connector pins I/A.

Ql through Q8 form a summing amplifier comprising a balanced input and an unbalanced output. to correct for small system level variations, trim pot R7 is.i ncor por ate d as part of the preamplifier. The differential balance adjustment control R6 serves to minimize common mode type signals originating ahead of the amplifier. C12 couples the output of the summing amplifier to a low-pass filter consisting of R22, R23, R24, C13, C14, CIS and ZI. The 3 dB roll-off point is located at approximately 40 kHz.

The output of ZI is coupled through C18 to the output amplifier 8-109A.

8-109A Output Amplifier and INSERT The 8-109A amplifier raises the nominal signal level to 0 dBm. The output is actively balanced and fed to the &quot;insert point&quot; at pins 15/5.

Pins 15/5 are usually connected to a normalled set of insert jack~, with the output side connected to the submaster fader. The fader output is returned to the module on pins 9/K. The feed for the PREFADE outputs is normally picked up at the mixing fader input and is returned to the module via pins 14/R. 8-109F Booster Amplifier

This amplifier operates with again of 33 dB. It recovers the 15 dB &quot;in-hand&quot; loss incurred by the fader and provides

aaditional gain to produce a nominal level of +8 dBm at its

output.

DIRECT Output and MON·nOR Output · The DIRECT output appears at pins 16/T. An additional isolated output is provided at pins 17/U. The latter output maybe utilized as a metering and/or monitor takeoff. Care should betaken to restrict loading of this output to 5k ohms or higher. Master Outputs and PAN Control A left and aright MASTER output are also being fed by the 8-109F output signal. They are routed via PAN switch SWI and PAN control R29 to R32, followed by two MASTER ASSIGNMENT SWITCHES SW5 and SW6. The master outputs are connected to the appropriate module output terminals via summing network resistors to be combined with feeds from other submaster mixing channels.

Auxiliary Outputs In addition, a SOLO output is available via SW7, to allow selective monitoring of the particular submaster channel. Other feeds originating from the 8-109F amplifier are supplied to the POST FADE RS, FB and PA channels.

PRE/POST Selector Switches and Level Controls PRE/POST selection of the RS, FB and PA channels is facilitated by switches SW2, SW3 and SW4 respectively; each switch is followed by its associated level control. The outputs of the level controls are fed to the summing outputs via individual assignment ~ switches. Following the assignment switches, these outputs are fed to their appropriate mixing &quot;buses via summing resistors. Control Functions A dc control contact closure is provided through operation of either one of the MASTER ASSIGNMENT switches SW5 or SW6. A further control contact is available on the SOLO switch SW7. Power Supply Decoupling

An active power supply decoupling network consisting of Q9

through Q14 provides isolation between the module and the ±25

voJt supply rails. Transistors Q13 and Q14 monitor the supply current. In the event of excessive power supply demands, such

as from component failure or amplifier overdrive, the current flow ing through Qll and Q12 will be limited.

**PARTS LIST**

PART DESCRIPTION MFG MFG PART NUMBER

Capacitor 330 uF/6 V

delete Kemet

**.. T390E337M003AS**

C5 10 pF Philips 2222-638-10109

C7 15 pF 2222-638-10159 C8 3.3 pF 2222-638-09338

CI0 10 uF/25 V Kemet T390CI06M025AS

C12 33 uF/lO V T390D336MOI0AS C13 1500 pF Aselco CQ92-MC-152M C14 220 pF Philips 2222-630-03221 C15 33 pF.. 2222-638-58339 C16 10 pF 2222-638-10109 C17 4.7 pF 2222-638-094 78 C18 33 uF/lO V Kemet T390D336MOI0AS C19 0.022 uF Aselco CQ92 -MC-223M C20 22 uF/25 V Philips 426ETF22

Diode Motorola

**.. I N4003**

Ql Transistor National 2N4401

</details>

<!-- /module data -->

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVkNZLW8yMmotdFk/view?resourcekey=0-pGXSlJdoHwg1Ct99AZgpLA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVkNZLW8yMmotdFk&resourcekey=0-pGXSlJdoHwg1Ct99AZgpLA" width="240" alt="1972 - M463J - 463-04-010 - WHEN DEPRESSED THE POSTFADE SIGNA.jpg"></a><br><sub>1972|5 · 463-04-010 - WHEN DEPRESSED THE POSTFADE SIGNA · <a href="MECHANICAL/1972%20-%20M463J%20-%20463-04-010%20-%20WHEN%20DEPRESSED%20THE%20POSTFADE%20SIGNA%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNngyQVlrRXBRNWs/view?resourcekey=0-5IzcYrHa-0pJpj3xQIntjw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNngyQVlrRXBRNWs&resourcekey=0-5IzcYrHa-0pJpj3xQIntjw" width="240" alt="1972 - M463J - 463-01-009 - FRE TAOC INPUT PAN INSERT FADER.jpg"></a><br><sub>1972|5 · 463-01-009 - FRE TAOC INPUT PAN INSERT FADER · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-01-009%20-%20FRE%20TAOC%20INPUT%20PAN%20INSERT%20FADER%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKelJ2S25JYkF4eGs/view?resourcekey=0-mWBnj_fThwLJVpzz0OYajw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKelJ2S25JYkF4eGs&resourcekey=0-mWBnj_fThwLJVpzz0OYajw" width="240" alt="1972 - M463J - 463-01-009 - MONITOR OUTPUT DIRECT OUTPUT.jpg"></a><br><sub>1972|5 · 463-01-009 - MONITOR OUTPUT DIRECT OUTPUT · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-01-009%20-%20MONITOR%20OUTPUT%20DIRECT%20OUTPUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeEZSblo1ZVBGdDg/view?resourcekey=0-mG1_qdleO0pJG4BL5-T-Ug" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeEZSblo1ZVBGdDg&resourcekey=0-mG1_qdleO0pJG4BL5-T-Ug" width="240" alt="1972 - M463J - 463-02-009 - NLESS OTHERWISE SPECIFIED COMPONENT DESIGNATIONS.jpg"></a><br><sub>1972|5 · 463-02-009 - NLESS OTHERWISE SPECIFIED COMPONENT DESIGNATIONS · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-02-009%20-%20NLESS%20OTHERWISE%20SPECIFIED%20COMPONENT%20DESIGNATIONS%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVTVpTnBvN0VYdVE/view?resourcekey=0-PqLj0JwrOhqAYNEYDGlpJw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVTVpTnBvN0VYdVE&resourcekey=0-PqLj0JwrOhqAYNEYDGlpJw" width="240" alt="1972 - M463J - 463-02-009 - NLESS OTHERWISE SPECIFIED.jpg"></a><br><sub>1972|5 · 463-02-009 - NLESS OTHERWISE SPECIFIED · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-02-009%20-%20NLESS%20OTHERWISE%20SPECIFIED%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKM29yNVlzT0l2X0k/view?resourcekey=0-e6UjbfcCcPAhEujFKf59cA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKM29yNVlzT0l2X0k&resourcekey=0-e6UjbfcCcPAhEujFKf59cA" width="240" alt="1972 - M463J - 463-06-001 - JES COMPONENT SIDE NOIES PINS IEI.jpg"></a><br><sub>1972|5 · 463-06-001 - JES COMPONENT SIDE NOIES PINS IEI · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-06-001%20-%20JES%20COMPONENT%20SIDE%20NOIES%20PINS%20IEI%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNVBpZnlKd2xEZ0U/view?resourcekey=0-5_v-lX8QudUgmUzy9wdtgA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNVBpZnlKd2xEZ0U&resourcekey=0-5_v-lX8QudUgmUzy9wdtgA" width="240" alt="1972 - M463J - 463-06-001 - SUBMASTER MODULE UNT.jpg"></a><br><sub>1972|5 · 463-06-001 - SUBMASTER MODULE UNT · <a href="SCHEMATICS/1972%20-%20M463J%20-%20463-06-001%20-%20SUBMASTER%20MODULE%20UNT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbXFiaFZveVN5bXM/view?resourcekey=0-YQNID-9y8KD0x2AEMG7RuA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbXFiaFZveVN5bXM&resourcekey=0-YQNID-9y8KD0x2AEMG7RuA" width="240" alt="1972 - M463J - 8-109-02-002 - OUTPUT AMPLIFIER CKDEAL SCHEMATIC.jpg"></a><br><sub>1972|5 · 8-109-02-002 - OUTPUT AMPLIFIER CKDEAL SCHEMATIC · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-02-002%20-%20OUTPUT%20AMPLIFIER%20CKDEAL%20SCHEMATIC%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKR0hXNjd0OEQ1Skk/view?resourcekey=0-zsrHFUcVVVil8_2DqAMbbw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKR0hXNjd0OEQ1Skk&resourcekey=0-zsrHFUcVVVil8_2DqAMbbw" width="240" alt="1972 - M463J - 8-109-02-002 - RII RIZ.jpg"></a><br><sub>1972|5 · 8-109-02-002 - RII RIZ · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-02-002%20-%20RII%20RIZ%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSDZ5NWtaYzV3cFU/view?resourcekey=0-AQcEH8XxTiwHxqdu0TCqCQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSDZ5NWtaYzV3cFU&resourcekey=0-AQcEH8XxTiwHxqdu0TCqCQ" width="240" alt="1972 - M463J - 8-109-02-007 - NDMINAL VALUE.jpg"></a><br><sub>1972|5 · 8-109-02-007 - NDMINAL VALUE · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-02-007%20-%20NDMINAL%20VALUE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcFhPTDFvcjU5c2s/view?resourcekey=0-u5lMfI9zUOafFzORTD5joA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcFhPTDFvcjU5c2s&resourcekey=0-u5lMfI9zUOafFzORTD5joA" width="240" alt="1972 - M463J - 8-109-02-007 - RII RIZ.jpg"></a><br><sub>1972|5 · 8-109-02-007 - RII RIZ · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-02-007%20-%20RII%20RIZ%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKb1daZFlKU1RRSGM/view?resourcekey=0-08ggQSH3dVT3rM-bvaofKg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKb1daZFlKU1RRSGM&resourcekey=0-08ggQSH3dVT3rM-bvaofKg" width="240" alt="1972 - M463J - 8-109-06-002 - RAS COMPONENT LAYOUT.jpg"></a><br><sub>1972|5 · 8-109-06-002 - RAS COMPONENT LAYOUT · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-06-002%20-%20RAS%20COMPONENT%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVXlOMTNjSHNmMVk/view?resourcekey=0-2xu8AYykKJGb8wEaB41LRQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVXlOMTNjSHNmMVk&resourcekey=0-2xu8AYykKJGb8wEaB41LRQ" width="240" alt="1972 - M463J - 8-109-06-002.jpg"></a><br><sub>1972|5 · 8-109-06-002 · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-06-002%20(EXTRACTED).svg">vectors</a></sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcmFlZnFNeG4yN1E/view?resourcekey=0-Vta-_GHsSOhVtN6wyMBVSQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcmFlZnFNeG4yN1E&resourcekey=0-Vta-_GHsSOhVtN6wyMBVSQ" width="240" alt="1972 - M463J - 8-109-06-007 - BOOSTER AMPLIFIER.jpg"></a><br><sub>1972|5 · 8-109-06-007 - BOOSTER AMPLIFIER · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-06-007%20-%20BOOSTER%20AMPLIFIER%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMThKY01DNWllZTQ/view?resourcekey=0-BTOPlySjq4iBtzjxHToZsw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMThKY01DNWllZTQ&resourcekey=0-BTOPlySjq4iBtzjxHToZsw" width="240" alt="1972 - M463J - 8-109-06-007 - DRI ENG.jpg"></a><br><sub>1972|5 · 8-109-06-007 - DRI ENG · <a href="SCHEMATICS/1972%20-%20M463J%20-%208-109-06-007%20-%20DRI%20ENG%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ2pFV2toVUlIdVU/view?resourcekey=0-A0SV-aJ4YS_OqElH2kbttw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ2pFV2toVUlIdVU&resourcekey=0-A0SV-aJ4YS_OqElH2kbttw" width="240" alt="1972 - M463J - 463-04-009 - CONNECTOR REAR VIEW HALE.jpg"></a><br><sub>1972|5 · 463-04-009 - CONNECTOR REAR VIEW HALE · <a href="PINOUTS/1972%20-%20M463J%20-%20463-04-009%20-%20CONNECTOR%20REAR%20VIEW%20HALE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

Not on Google Drive yet: `M463J - RTO-144 Connections.pdf`

## RTO-144 pinout

Read from 2 pinout pictures (each its own `.pinout.json` beside it); 2 to check (`conflicts`). Every contact, with where it was read: [`RTO.json`](RTO.json). How a picture becomes this table: [the pinout decision tree](https://github.com/WardBeckSystems/WBSps.ca/blob/main/2026/Engineering/PINOUTS.md).

**To check:**

- disagree P1-W: kept M1 CONTROL (control_out); M463AC/PINOUTS/1986 - M463AC - 463-04-009 - CONNECTOR REAR VIEW.pinout.json says M1 CONTROL (control_in)
- disagree P1-X: kept M2 CONTROL (control_out); M463AC/PINOUTS/1986 - M463AC - 463-04-009 - CONNECTOR REAR VIEW.pinout.json says M2 CONTROL (control_in)
- insert guessed: Direction (in/out) of M1 CTL and M2 CTL not stated FADER OUT (K/9) and FADER IN (S/15): fader send/return. (M463J: 1972 - M463J - 463-04-009 - CONNECTOR REAR VIEW HALE.jpg)

**Inserts:** FADER INSERT: FADER OUT → FADER IN

| Pin | Signal | Kind | Port | Confidence |
|---|---|---|---|---|
| 1 | INPUT | in | INPUT | high |
| 2 | SHIELD | shield | shield | high |
| 3 | PA OUT | out | PA OUT | high |
| 4 | FB 2 OUT | out | FB 2 OUT | high |
| 5 | FB 1 OUT | out | FB 1 OUT | high |
| 6 | RS 2 OUT | out | RS 2 OUT | high |
| 7 | RS 1 OUT | out | RS 1 OUT | high |
| 8 | SOLO OUT | out | SOLO OUT | high |
| 9 | FADER OUT | insert_send | FADER OUT | high |
| 10 | SHIELD | shield | shield | high |
| 11 | M1 OUT | out | M1 OUT | high |
| 12 | M2 OUT | out | M2 OUT | high |
| 13 | SHIELD | shield | shield | high |
| 14 | PREFADE IN | in | PREFADE IN | high |
| 15 | FADER IN | insert_return | FADER IN | high |
| 16 | DIRECT OUT | out | DIRECT OUT | high |
| 17 | MONITOR OUT | out | MONITOR OUT | high |
| 18 | CONTROL COMMON | ground |  | high |
| 19 | -25 V | power |  | high |
| 20 | COMMON | ground |  | high |
| 21 | +25 V | power |  | high |
| 22 | CHASSIS GROUND | ground |  | high |
| A | INPUT | in | INPUT | high |
| B | SHIELD | shield | shield | high |
| C | PA OUT | out | PA OUT | high |
| D | FB 2 OUT | out | FB 2 OUT | high |
| E | FB 1 OUT | out | FB 1 OUT | high |
| F | RS 2 OUT | out | RS 2 OUT | high |
| H | RS 1 OUT | out | RS 1 OUT | high |
| J | SOLO OUT | out | SOLO OUT | high |
| K | FADER OUT | insert_send | FADER OUT | high |
| L | SHIELD | shield | shield | high |
| M | M1 OUT | out | M1 OUT | high |
| N | M2 OUT | out | M2 OUT | high |
| P | SHIELD | shield | shield | high |
| R | PREFADE IN | in | PREFADE IN | high |
| S | FADER IN | insert_return | FADER IN | high |
| T | DIRECT OUT | out | DIRECT OUT | high |
| U | MONITOR OUT | out | MONITOR OUT | high |
| V | SOLO CONTROL | control_in | SOLO CTL | high |
| W | M1 CONTROL | control_out | M1 CTL | high |
| X | M2 CONTROL | control_out | M2 CTL | high |
| Y | M1/M2 CONTROL IN | control_in | M1/M2 CTL IN | high |
| Z | N/C | nc |  | high |

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMXVkdnRiMG9ad28/view?resourcekey=0-s2MHUHP05BJ2lj6Jaw-P_A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMXVkdnRiMG9ad28&resourcekey=0-s2MHUHP05BJ2lj6Jaw-P_A" width="240" alt="1972 - M463J - P001 - Title Page.jpg"></a><br><sub>1972|5 · P001 - Title Page</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTHNMSzQ0LUlTMHc/view?resourcekey=0-CqcoYLjWkqE4mfnsFmJzCg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTHNMSzQ0LUlTMHc&resourcekey=0-CqcoYLjWkqE4mfnsFmJzCg" width="240" alt="1972 - M463J - P002 - 1-1.jpg"></a><br><sub>1972|5 · P002 - 1-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKekFmYU5xcGNBVUE/view?resourcekey=0-wWX1OHn7AqDzJdNNNEOBiQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKekFmYU5xcGNBVUE&resourcekey=0-wWX1OHn7AqDzJdNNNEOBiQ" width="240" alt="1972 - M463J - P003 - 2-1.jpg"></a><br><sub>1972|5 · P003 - 2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKYUpWZzFGQmZ4Nnc/view?resourcekey=0-KzwBE3GwkDP66FpU-EeEcw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKYUpWZzFGQmZ4Nnc&resourcekey=0-KzwBE3GwkDP66FpU-EeEcw" width="240" alt="1972 - M463J - P004 - 2-2.jpg"></a><br><sub>1972|5 · P004 - 2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSFRXa0JOVkk4Y00/view?resourcekey=0-iZl8MtdYZ6lclkMWXtMt0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSFRXa0JOVkk4Y00&resourcekey=0-iZl8MtdYZ6lclkMWXtMt0A" width="240" alt="1972 - M463J - P005 - 3-1.jpg"></a><br><sub>1972|5 · P005 - 3-1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcFJnVHlraXh0YXM/view?resourcekey=0-xitiRAtL3DdW_tZAXCrHKw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcFJnVHlraXh0YXM&resourcekey=0-xitiRAtL3DdW_tZAXCrHKw" width="240" alt="1972 - M463J - P006 - 3-2.jpg"></a><br><sub>1972|5 · P006 - 3-2</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbExDM1VHOHItSjg/view?resourcekey=0-weiowUgUt3Fr5fdkxELXMw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbExDM1VHOHItSjg&resourcekey=0-weiowUgUt3Fr5fdkxELXMw" width="240" alt="1972 - M463J - P007 - 3-3.jpg"></a><br><sub>1972|5 · P007 - 3-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMi1mSnVoWWN3VDg/view?resourcekey=0-7xF-np8o_gvDYMPOKiCnqg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMi1mSnVoWWN3VDg&resourcekey=0-7xF-np8o_gvDYMPOKiCnqg" width="240" alt="1972 - M463J - P008 - 3-4.jpg"></a><br><sub>1972|5 · P008 - 3-4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdHhwWUszZURraGs/view?resourcekey=0-npgvULAfjAxJUVOq-8tOhg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdHhwWUszZURraGs&resourcekey=0-npgvULAfjAxJUVOq-8tOhg" width="240" alt="1972 - M463J - P009 - 8-109-1-1.jpg"></a><br><sub>1972|5 · P009 - 8-109-1-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd0g3bUZQVmVqblk/view?resourcekey=0-mcfMquvQLgKfrFc1rJdkCA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd0g3bUZQVmVqblk&resourcekey=0-mcfMquvQLgKfrFc1rJdkCA" width="240" alt="1972 - M463J - P010 - 8-109-1-2.jpg"></a><br><sub>1972|5 · P010 - 8-109-1-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaU9RelpSM1NQXzQ/view?resourcekey=0-LopBveX_XSjopT1UWuZPcQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaU9RelpSM1NQXzQ&resourcekey=0-LopBveX_XSjopT1UWuZPcQ" width="240" alt="1972 - M463J - P011 - 8-109-1-3.jpg"></a><br><sub>1972|5 · P011 - 8-109-1-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKaHROa1JSNVduSjQ/view?resourcekey=0-YOmTWmAH3bUAL519zNz-wQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKaHROa1JSNVduSjQ&resourcekey=0-YOmTWmAH3bUAL519zNz-wQ" width="240" alt="1972 - M463J - P012 - 8-109-2-1.jpg"></a><br><sub>1972|5 · P012 - 8-109-2-1</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcks0bHNIR0oxdEU/view?resourcekey=0-padpAbvuZ4GIbrtcu8VBgg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcks0bHNIR0oxdEU&resourcekey=0-padpAbvuZ4GIbrtcu8VBgg" width="240" alt="1972 - M463J - P013 - 8-109-2-2.jpg"></a><br><sub>1972|5 · P013 - 8-109-2-2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRFU4OEl0Sk9jNGs/view?resourcekey=0-rZtNHJdCI2kn4ezeKz8HYw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRFU4OEl0Sk9jNGs&resourcekey=0-rZtNHJdCI2kn4ezeKz8HYw" width="240" alt="1972 - M463J - P014 - 8-109-2-3.jpg"></a><br><sub>1972|5 · P014 - 8-109-2-3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNHpzVDBzU3lJV0U/view?resourcekey=0-tv3HezhNT0gMmhjfLHcBQg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNHpzVDBzU3lJV0U&resourcekey=0-tv3HezhNT0gMmhjfLHcBQg" width="240" alt="1972 - M463J - P015 - 8-109-2-4.jpg"></a><br><sub>1972|5 · P015 - 8-109-2-4</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNElJTXZ3WEIweGM/view?resourcekey=0-XJaqG58Z6DsLRWZfZ_e0ZQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNElJTXZ3WEIweGM&resourcekey=0-XJaqG58Z6DsLRWZfZ_e0ZQ" width="240" alt="1972 - M463J - P016 - 8-109-2-5.jpg"></a><br><sub>1972|5 · P016 - 8-109-2-5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKWUk1SjN6UE9WSHc/view?resourcekey=0-C4fdcfec3j2fa5mShYY6Xg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKWUk1SjN6UE9WSHc&resourcekey=0-C4fdcfec3j2fa5mShYY6Xg" width="240" alt="1972 - M463J - Submaster Module (2).pdf"></a><br><sub>1972|5 · Submaster Module (2)</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQVFZNVp6RU0xSk0/view?resourcekey=0-DcytJjMeXQmJWL7R8fTJWA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQVFZNVp6RU0xSk0&resourcekey=0-DcytJjMeXQmJWL7R8fTJWA" width="240" alt="1972 - M463J - Submaster Module.pdf"></a><br><sub>1972|5 · Submaster Module</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1972 - M463J - 463-01-009 - FRE TAOC INPUT PAN INSERT FADER.kicad_sch](KICAD/1972%20-%20M463J%20-%20463-01-009%20-%20FRE%20TAOC%20INPUT%20PAN%20INSERT%20FADER.kicad_sch)
- [1972 - M463J - 463-01-009 - MONITOR OUTPUT DIRECT OUTPUT.kicad_sch](KICAD/1972%20-%20M463J%20-%20463-01-009%20-%20MONITOR%20OUTPUT%20DIRECT%20OUTPUT.kicad_sch)
- [1972 - M463J - 463-02-009 - NLESS OTHERWISE SPECIFIED COMPONENT DESIGNATIONS.kicad_sch](KICAD/1972%20-%20M463J%20-%20463-02-009%20-%20NLESS%20OTHERWISE%20SPECIFIED%20COMPONENT%20DESIGNATIONS.kicad_sch)
- [1972 - M463J - 463-02-009 - NLESS OTHERWISE SPECIFIED.kicad_sch](KICAD/1972%20-%20M463J%20-%20463-02-009%20-%20NLESS%20OTHERWISE%20SPECIFIED.kicad_sch)
- [1972 - M463J - 8-109-02-002 - OUTPUT AMPLIFIER CKDEAL SCHEMATIC.kicad_sch](KICAD/1972%20-%20M463J%20-%208-109-02-002%20-%20OUTPUT%20AMPLIFIER%20CKDEAL%20SCHEMATIC.kicad_sch)
- [1972 - M463J - 8-109-02-002 - RII RIZ.kicad_sch](KICAD/1972%20-%20M463J%20-%208-109-02-002%20-%20RII%20RIZ.kicad_sch)
- [1972 - M463J - 8-109-02-007 - NDMINAL VALUE.kicad_sch](KICAD/1972%20-%20M463J%20-%208-109-02-007%20-%20NDMINAL%20VALUE.kicad_sch)
- [1972 - M463J - 8-109-02-007 - RII RIZ.kicad_sch](KICAD/1972%20-%20M463J%20-%208-109-02-007%20-%20RII%20RIZ.kicad_sch)
- [1972 - M463J - Submaster Module (2) p26.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20(2)%20p26.kicad_sch)
- [1972 - M463J - Submaster Module p19.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20p19.kicad_sch)
- [1972 - M463J - Submaster Module p20.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20p20.kicad_sch)
- [1972 - M463J - Submaster Module p21.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20p21.kicad_sch)
- [1972 - M463J - Submaster Module p26.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20p26.kicad_sch)
- [1972 - M463J - Submaster Module p30.kicad_sch](KICAD/1972%20-%20M463J%20-%20Submaster%20Module%20p30.kicad_sch)
- [M463J.kicad_sym](KICAD/M463J.kicad_sym)
- [index.html](KICAD/index.html)

## Software

- [index.html](SOFTWARE/index.html)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
