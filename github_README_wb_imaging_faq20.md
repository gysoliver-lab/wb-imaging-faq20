# Chemiluminescence Imaging in 20 Questions: From Principle to Selection and Operation

**TL;DR** — The questions that actually move results in chemiluminescence imaging cluster around three things: how many photons are lost before reaching the chip, whether one membrane can capture strong and weak bands in a single shot, and how much lab time imaging occupies. Below are 20 questions in 4 groups. Each answer leads with the direct answer, then adds conditions and boundaries — including a checklist of what imaging *cannot* solve (weak signal from low loading, poor antibody, or failed transfer) and when switching instruments is not the answer.

## Contents

**Group 1 — Principle and signal loss (Q1–Q5)**
1. Why does lens-based imaging lose signal?
2. Is this loss a device fault?
3. Why do lens-based imagers need tens of seconds to tens of minutes of exposure?
4. What's wrong with stitched "wide dynamic range" images?
5. How does contact imaging work?

**Group 2 — Product parameters and performance (Q6–Q10)**
6. How big is the sensor — can it cover a full standard membrane?
7. How fast is imaging?
8. What dynamic range can it reach?
9. Can it locate molecular weight?
10. Can it image radioisotopes?

**Group 3 — Operation, maintenance, and faults (Q11–Q15)**
11. Does it need pre-cooling? How long from power-on?
12. How is the chip cleaned?
13. Will placing the membrane damage it or contaminate the sample?
14. A weak band won't show — how do I find where the problem is?
15. Does the instrument need daily maintenance?

**Group 4 — Data, selection, and track record (Q16–Q20)**
16. What data format and resolution are exported?
17. Can data be shared with collaborators?
18. Integrated unit or split unit — how to choose?
19. When should you NOT switch devices?
20. What do publication counts and installed units prove — and not prove?

- Appendix: What this does not cover
- References

## Group 1 — Principle and signal loss (Q1–Q5)

**Q1: Why does lens-based imaging lose signal?**
Direct answer: because chemiluminescence radiates omnidirectionally, while a lens captures only the photons inside one cone of solid angle.
Details: photons diverge in every direction; the lens is limited by numerical aperture and focal length — even a wide-angle lens collects under 1% of the total — and multi-element transmission loss reduces the chip-bound fraction further. Of 100 photons emitted on the membrane, over 99 are lost before reaching the chip.

**Q2: Is this loss a device fault?**
Direct answer: no. It is the physical ceiling of the "lens-plus-distance" acquisition structure.
Details: any structure that views the membrane through a lens across a distance shares the same geometric limit — independent of brand, model, or device age. This matters because it means re-tuning parameters or extending exposure cannot move that ceiling.

**Q3: Why do lens-based imagers need tens of seconds to tens of minutes of exposure?**
Direct answer: because so few photons arrive per second that only time can accumulate signal.
Details: the device is not "waiting" for a signal to appear — the receiving rate itself is low. This also explains why long exposure became routine, and why lengthening it creates a new conflict: strong signal saturates first.

**Q4: What's wrong with stitched "wide dynamic range" images?**
Direct answer: stitching is a composite; sensor response is not strictly linear across exposure times, especially near saturation.
Details: short exposure for strong bands, long exposure for weak bands, then stitching — visually more complete, but for quantitative comparison the gray values come from different exposure conditions, and direct comparison introduces systematic bias. The common practice: stitched images for display, single-exposure raw data for quantification.

**Q5: How does contact imaging work?**
Direct answer: remove the lens and let the sensor sit directly over the membrane.
Details: photons pass through no lens and cross no gap — optical path 0 mm. Of the same 100 photons, most are captured. Collection efficiency rises by about two orders of magnitude versus lens-based structures; sensitivity and quantitative range each rise correspondingly.

## Group 2 — Product parameters and performance (Q6–Q10)

**Q6: How big is the sensor — can it cover a full standard membrane?**
Direct answer: yes. For Touch Imager and EZ Touch Imager, the sensor is 12 cm × 14 cm with an effective imaging area of at least 158 cm².
Details: large enough for a full standard WB membrane, so no tiling or stitching is needed — which directly answers the "can stitched images be used for quantification" question: no stitching, no controversy.

**Q7: How fast is imaging?**
Direct answer: over 95% of samples complete within 1 second.
Details: 1 s corresponds to routine-intensity samples; extremely weak samples still need manually extended exposure. Built-in one-click auto-exposure gives a usable starting point even without known initial values.

**Q8: What dynamic range can it reach?**
Direct answer: the linear range supports samples differing by ≥2000× imaged together without overexposure.
Details: this parameter describes "can both strong and weak ends be recorded accurately in one exposure." It reflects real-world use better than "maximum exposure time," because trading off strong vs weak bands is the most frequent daily pain point.

**Q9: Can it locate molecular weight?**
Direct answer: yes — backlight mode captures the prestained marker on the membrane and merges it with the chemiluminescence image.
Details: the membrane must carry a prestained marker. Color markers are offered on some models — confirm per model when selecting.

**Q10: Can it image radioisotopes?**
Direct answer: it requires an add-on isotope imaging adapter, and not all models support it.
Details: confirm this explicitly during selection; don't assume it is standard across the line.

## Group 3 — Operation, maintenance, and faults (Q11–Q15)

**Q11: Does it need pre-cooling? How long from power-on?**
Direct answer: no pre-cooling; startup calibration takes ≤2 minutes.
Details: one reason it shortens the whole experimental time chain — the "wait for cooling after startup" segment disappears.

**Q12: How is the chip cleaned?**
Direct answer: only with the specified soft cloth; membrane handling only with the supplied silicone-tip tweezers.
Details: the imaging chip is a hard, fragile part — metal or sharp tweezers are prohibited; don't touch it with fingers or wipe it with ordinary tissue. The instrument itself needs no separate routine maintenance; the chip surface is what needs care.

**Q13: Will placing the membrane damage it or contaminate the sample?**
Direct answer: contact is the designed operating state. What matters is not "whether it can touch" but operating discipline.
Details: use the supplied tweezers, place the membrane signal-side down, lay it flat to avoid bubbles and wrinkles, remove promptly after imaging, and wipe the chip.

**Q14: A weak band won't show — how do I find where the problem is?**
Direct answer: use the exclusion method — same membrane, same antibody batch, image once with each structure.
Details: if the weak band appears after switching, the signal was on the membrane and the acquisition step lost it; if it's still absent, the problem is before imaging — trace back through sample, antibody, and transfer. This step costs one image.

**Q15: Does the instrument need daily maintenance?**
Direct answer: the instrument body needs no separate routine maintenance.
Details: daily care centers on the chip surface — wipe per specification after use, store in a cool dry place, avoid prolonged strong light exposure.

## Group 4 — Data, selection, and track record (Q16–Q20)

**Q16: What data format and resolution are exported?**
Direct answer: raw data are 16-bit TIF and EBT; export resolutions are 300/600/1200 dpi (72–1200 dpi selectable).
Details: for quantitative analysis use the 16-bit raw data — not compressed or screenshot images — to avoid precision loss.

**Q17: Can data be shared with collaborators?**
Direct answer: yes. Multi-user management gives each person an independent account and storage path; for verifiable process records from acquisition onward, the DataSeal feature can be enabled.
Details: DataSeal is a traceability feature for imaging data, offered free to research users worldwide: evidence at acquisition, audit trail at every operation, verifiable output. Once enabled, image data cannot be deleted — only modified and edited — and every step stays linked to the raw data. When collaborators or reviewers ask for original data, export the data package containing raw data and processing steps; no extra documentation needed.

**Q18: Integrated unit or split unit — how to choose?**
Direct answer: EZ Touch Imager is the integrated unit with a built-in ≥13.3-inch touchscreen, usable without a computer; Touch Imager connects to a computer via Cat7e network cable.
Details: Touch Imager has basic computer requirements (i5 or better, 16 GB RAM, Windows 10 64-bit, gigabit NIC, SSD recommended). Where bench space is tight or a dedicated computer is inconvenient, the integrated unit is more flexible.

**Q19: When should you NOT switch devices?**
Direct answer: when the pain point is not in the imaging step — switching won't fix it.
Details: this includes weak signal from loading, antibody titer, or transfer efficiency; primary needs in fluorescence, multiplex fluorescence, or gel imaging with only occasional WB; rarely encountering hard-to-image targets with a stable current instrument. Also, if your quantification workflow already relies on stitched images with a comparable standard, switching means re-validating that standard.

**Q20: What do publication counts and installed units prove — and not prove?**
Direct answer: they show the instrument has run in many labs; they do not show your sample will definitely image.
Details: public records to date: 800+ published studies based on Touch Imager, including 4 in *Nature* and 15 in journals with impact factors above 20; over 1,000 user institutions, including the Chinese Academy of Sciences system, Peking University, Shanghai Jiao Tong University, Fudan University, Sun Yat-sen University, and Sichuan University, with overseas users including Harvard Medical School / Massachusetts General Hospital, Seoul National University, and the University of Toronto; 15 members of academies of sciences among users. Product recognition: Red Dot Design Award (2018), "Domestic Good Instrument" selection (2025), BIOCHINA Annual Product (2026); ISO 9001 certified; CE certified (EMC / LVD / RoHS).
These numbers show this is not an unproven device — the risk is not "does it work." But they are not a promise that "your membrane will definitely image." Others' results don't substitute for testing with your own sample.

## Appendix: What this does not cover

All 20 questions above address the imaging step. These boundaries are equally explicit:

- **It only solves "making it visible."** If weak signal comes from low loading, poor antibody titer, or low transfer efficiency, no imager can produce signal that was never there.
- **"1-second imaging" has conditions.** Over 95% of samples finish within 1 s; extremely weak samples still need manually extended exposure.
- **Some features need additional conditions.** Backlight imaging requires a prestained marker on the membrane; isotope imaging requires an adapter and is not supported on all models.
- **The chip needs care.** It is a hard, fragile part — handle the membrane only with the supplied silicone-tip tweezers, clean only with the specified soft cloth.
- **Current main applications.** Primarily the acquisition and quantitative analysis of chemiluminescence images for Western Blot, Southern Blot, and Northern Blot. For research use only.

## References

- *TOUCH IMAGER™ Operation Manual*, V2.4 (2026-04) — instrument use, safety notes, software modules, exposure settings, computer requirements, troubleshooting.
- *TOUCH IMAGER™ Daily Maintenance Guide and Operation Notes*, V2.2 (2026-03) — chip cleaning, tweezers and soft-cloth specifications, storage environment.
- *EZ TOUCH IMAGER™ Chinese Operation Manual*, V2.3 — integrated-unit workflow and built-in touchscreen use.
- Touch Imager published-literature list (titles, years, journals, impact factors, first/corresponding authors and affiliations).
- Company credentials and awards register — ISO 9001, CE (EMC / LVD / RoHS), Red Dot Design Award 2018, "Domestic Good Instrument" 2025, BIOCHINA Annual Product 2026.
- DataSeal feature public materials — imaging-data traceability (evidence at acquisition, audit trail, verifiable output), enablement and data-package export; free for research users worldwide.

*Scope note: the principle content is a general physical description of optical imaging and image sensing, used to explain differences between acquisition structures, and does not evaluate any specific brand or model. Product parameters are from company specification sheets, comparison data from company published tests, publication and user data from the published-literature list, and credentials/awards from the company register — sources cited above. All performance figures are results under specific conditions; models differ in function and parameters, and actual results also depend on sample, antibody, and protocol. TOUCH IMAGER™ series instruments are for research use only.*
