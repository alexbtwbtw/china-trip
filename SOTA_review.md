# Review: SOTA Report — Solar-Powered Multirotor UAVs for 3D Area Mapping

Comments organised by category. Section headings and quoted text use the wording from your PDF.

---

## 1. Compliance with the Assignment Brief

The brief lists seven required components. Status check:

| Requirement | Status |
|---|---|
| Cover sheet | Present (combined with declaration — allowed) |
| Declaration | Present |
| **Contents page** | **MISSING** — the brief explicitly requires this |
| Brief introduction | Present (§1) |
| Literature review | Present (§2) |
| Conclusions and implications for SOTA for project RAO | Present, but **split awkwardly** between §3 ("Implications") and §4 ("Conclusions"). The brief asks for a single "Conclusions and implications" section — consider merging, or at least flipping the order so Conclusions come last. |
| List of references | Present (but you said you'll fix these) |

**Other formatting points from the brief to double-check:**
- 1.5 line spacing, 2.5 cm margins, 12 pt Arial or Times New Roman — verify in the source document.
- Word count: 2,000–2,500 max (excluding figures, tables, references, contents, cover). I'd estimate the body (§1 through §4 Conclusions) is comfortably inside this range, but you should confirm with a word count.
- Harvard referencing is the suggested style — your current numeric `[1]`, `[2]` style is **IEEE/Vancouver**, not Harvard. Confirm with your supervisor which style was agreed.

**Section numbering bug:** You have **two** sections labelled "4." — `4. Conclusions` and `4. References`. Renumber References to 5.

---

## 2. Grammar, Syntax, and Clarity Issues

### §1 Introduction
- *"This research topic is important because it provides first responders with fast, accurate situational awareness through these **3d** models…"* — should be **"3D"** (capitalised, consistent with the title).
- *"…examines **5** main research areas…"* — style: spell out numbers under ten in formal academic writing → **"five"**.
- *"…because **I** wanted to examine the problem in its entirety…"* — first-person "I" is used inconsistently across the report. Either commit to first person throughout or rewrite in third person/passive ("…because the problem was examined in its entirety…"). Most UK academic supervisors prefer the latter for SOTA reports.

### §2.1 Disaster-response and remote area mapping
- Mix of **American and British** spelling: *utilizes, analyzing, emphasizes, organisation* — pick one (UK English would be *utilises, analysing, emphasises*) and apply throughout.
- *"…image latency, cloud cover affecting optical data, limited labeled data for AI training…"* — long bulleted-style list embedded in prose; consider breaking into a bullet list or two shorter sentences.
- The whole subsection contains **only one in-text citation** (`[4]`). Almost every claim ("Several studies highlight…", "The literature emphasizes…", "Most articles link…") needs a citation. This is the single biggest weakness of the literature review.

### §2.2 Conventional multirotor drones for mapping
- **Sentence fragment:** *"To tackle these limitations, the literature highlights the importance of careful flight planning. **Ensuring adequate forward/side overlap, terrain-aware altitude selection, and robust checkpoints.**"* — the second "sentence" has no verb. Merge: *"…flight planning, including adequate forward/side overlap, terrain-aware altitude selection, and robust checkpoints."*
- Figure 1 caption: *"…study area in **Kingali**"* — likely a typo for **Kigali** (the capital of Rwanda); confirm against source [8].
- *"…**it's** a lesser limitation for solar drones"* and *"…as **it's** a major factor…"* — avoid contractions in academic writing → *"it is"*.
- *"global navigation satellite system quality"* — first use of GNSS; consider abbreviating: *"global navigation satellite system (GNSS) quality"*.
- *"RTK-PPK"* — neither RTK (Real-Time Kinematic) nor PPK (Post-Processed Kinematic) is defined.

### §2.3 Solar-powered UAVs and current technological limitations
- **Broken sentence (the most serious in the report):** *"This causes the mass energy storage needed to remain operational to increase rapidly **energy delivery** when the UAVs are exposed to such conditions."* — this is ungrammatical and the meaning is lost. Rewrite, e.g.: *"As a result, the mass of energy storage required to keep the UAV operational under such conditions rises rapidly."*
- *"…current solar panel technology can offer. **In-flight solar power irradiance fluctuates significantly…**"* — "in-flight solar power irradiance" is awkward. Suggest: *"In-flight solar irradiance fluctuates significantly…"*
- *"…even under optimal conditions where changing irradiance **isn't** factored in…"* — contraction (and the encoding has rendered it as `isn�t`; check the source file for stray smart quotes).
- *"…high-efficiency photovoltaic cells improve power density but are made from low-cost silicon, which can be heavier and less malleable."* — this reads as contradictory: high-efficiency cells are typically *not* low-cost silicon. Did you mean to contrast high-efficiency tandems with conventional silicon? Clarify.
- *"An emerging alternative is **perovskite**; however, **they** face the same…"* — singular/plural mismatch → *"perovskite cells; however, they face…"*.
- *"…as of **March 2026**, NREL reports top research-cell efficiencies of about 27.9% for single-junction crystalline Si and about 35.0% for 2-terminal perovskite/Si tandems."* — **no in-text citation here** even though [13] is the NREL chart. Add `[13]`.
- *"Another limiting factor is the weight penalty, which is the trade-off for everything on the SPUAV."* — vague. Rewrite to specify what trade-off you mean (added components → mass → reduced endurance).

### §2.4 Flight-path strategies
- *"…it is characterized by its parallel **'lawnmower'** strips and **'straight-down'** camera angle."* — quotation marks have rendered as `�` in the encoding; the source likely uses smart quotes. Convert to standard ASCII quotes for consistency.
- *"…between **30°** and **60°**…"* — degree symbols encode oddly in the PDF (`30�`). Verify the source uses real `°` characters.
- *"**It's** an attractive method, as despite being simple to plan, it provides systematic coverage…"* — contraction, plus comma splice. Suggest: *"It is an attractive method: despite being simple to plan, it provides systematic coverage…"*
- *"One study compared these three to the Nadir and oblique flight paths."* — **which study?** Add citation. (Presumably [23], based on Figure 2.)
- *"…**3** promising novel flight paths…"* → "three".
- *"POI had the worst performance out of the **3**."* → "three".
- Capitalisation: "Nadir" is sometimes capitalised, sometimes not ("nadir+oblique"). Be consistent.

### §2.5 Photogrammetry and 3D model evaluation
- *"…a typical workflow is **image capture, feature matching, and Structure from Motion, sparse cloud generation, dense multi-view stereo, meshing, texturing, and validation.**"* — the comma after "Structure from Motion" should be a semicolon or the list should be reformatted; as written it reads as if "Structure from Motion" and "sparse cloud generation" are siblings of "image capture", which loses the logical grouping.
- This subsection is **the shortest** and has **zero in-text citations** — needs strengthening (see §3 below).
- "Earth Mover's Distance" — encoding has rendered the apostrophe as `�`.

### §3 Implications for Project RAO
- *"…**they're** made from a high-altitude perspective."* — contraction.
- *"…the level of detail in these maps **isn't** high enough to really help in disaster response…"* — contraction; *"really"* is informal → "sufficient".
- *"My project aims to address this research gap…"* — strong claim. Earlier (§2.1) you wrote *"the present project will not address the identified research gap"*. **These two statements contradict each other.** Reconcile.
- *"…fixed-wing UAVs **tilt horizontally** during maneuvers such as turning."* — fixed-wing aircraft *bank* (roll about the longitudinal axis); "tilt horizontally" is ambiguous. Use *"bank"* or *"roll"*.

### §4 Conclusions
- *"…autonomous, purely solar-powered flight is already feasible with current technology, but has been demonstrated only by large-scale fixed-wing UAVs."* — needs a citation (e.g., reference to a Zephyr-class aircraft or [14]/[18]).
- The conclusion is quite short relative to the implications section. Consider expanding by one short paragraph that explicitly answers: *"What does the SOTA review tell you that you didn't know before, and what is the single most important course-correction for project RAO?"*

---

## 3. Key Issues Missing from the Report

### A. Citation density is too low
The biggest content weakness. Across roughly 2,000+ words of literature review, I count only a handful of in-text citations: `[4]`, `[8]`, `[23]`. The reference list contains **29 sources** — almost none are cited in the body. A SOTA marker will deduct heavily for this. Every paragraph that begins *"The literature shows…", "Several studies…", "Recent work…"* needs `[n]`-style attribution to the specific paper.

### B. No critical comparison between sources
The current style summarises what "the literature" says collectively. A stronger SOTA contrasts authors: *"Whereas Koeva et al. [8] report sub-10 cm accuracy, Boon et al. [12] argue that fixed-wing platforms achieve comparable accuracy over much larger areas."* This demonstrates analysis rather than reporting.

### C. Quantitative figures are largely absent
Solar UAV feasibility hinges on numbers: payload mass, panel power density (W/m²), hover power (W/kg), battery energy density (Wh/kg), typical endurance (minutes/hours). You mention NREL cell efficiencies but no comparable figures appear elsewhere. Adding even a small comparison table (e.g., reported endurance / wing area / mass for the SPUAVs in [14], [15], [18]) would substantially strengthen §2.3.

### D. The "micro" qualifier from the title is never defined
The title says **"Micro Aerial Vehicles"** but nowhere in the body do you define the MAV size class (typically <50 cm, <2 kg per common definitions). This matters because most cited solar UAV work is on much larger aircraft — you should explicitly acknowledge that there is a size-scaling gap between the cited literature and your project's MAV scope.

### E. No discussion of regulation / airspace
You mention *"regulatory…constraints for UAVs"* once in §2.1 but never expand. For a UK-based MSc, CAA rules (open/specific/certified categories, BVLOS limits) are highly relevant to a disaster-response use case and worth at least a paragraph.

### F. No discussion of payload (the camera/sensor itself)
Photogrammetric quality (§2.5) depends heavily on the sensor: global vs rolling shutter, RGB vs multispectral, gimbal stabilisation. Given solar MAVs have very tight mass budgets, the sensor choice deserves explicit treatment as a design constraint.

### G. The "AI/ML" thread is dropped
§2.1 introduces AI/ML for flood delineation, and the conclusion of §2.1 hints at AI annotation as future work — but §2.5 doesn't pick up on neural radiance fields (NeRF), Gaussian splatting, or learning-based MVS, which are all active SOTA in 3D reconstruction circa 2025–2026 and directly relevant. Consider at least one paragraph acknowledging these.

### H. No "research gap → project response" mapping table
You'd score well by adding a short table at the end of §3 that explicitly maps each subsection's identified gap/insight to a concrete project decision. Right now the reader has to extract this themselves.

### I. Figures are under-leveraged
- **Figure 1** (Kigali orthophoto) — caption is one line; no explanation in the body of *why* this figure is shown or what it demonstrates.
- **Figure 2** (flight paths) — referenced as 2.A–2.D but never has a list of figures, and the caption has only the citation `[23]`, no description.
- Both figures need a sentence in the body that says *"as shown in Figure X…"* with the analytical point being made.

---

## 4. Other Items Worth Raising

1. **Inconsistent terminology.** You use *UAV*, *drone*, *quadcopter*, *multirotor*, and *MAV* somewhat interchangeably. Define each on first use and stick to one preferred term per concept.

2. **The introduction promises a structure that the report doesn't quite follow.** It says the report becomes "increasingly project-specific with each subsection". This is broadly true, but §2.5 (Photogrammetry) is arguably *less* project-specific than §2.4. Worth re-reading to check the framing matches the content.

3. **Declaration of AI use.** You disclose Elicit and ChatGPT use, which is good. Consider being slightly more specific (e.g., *"ChatGPT was used to suggest section ordering and to draft a single paragraph in §2.X, which was then rewritten by the author"*). Vague declarations sometimes attract more scrutiny than specific ones.

4. **Encoding artefacts.** The PDF contains `�` characters in place of curly apostrophes/quotes/diacritics (e.g., `isn�t`, `Mower�s`, `K�rner`, `fa�ade`, `30�`). Either the source document has font/encoding issues or the PDF export mangled them. Open the source `.docx` and search/replace.

5. **Tense inconsistency.** Some paragraphs in §2.x use past tense ("the article demonstrated"), others present ("the literature shows"). Convention for SOTA reviews: present tense for established findings, past tense when describing what a specific study did.

6. **"5." Photogrammetry was numbered "6." in reference [27.4] / [28.4] / [29.4].** Another hint that an earlier draft had six subsections; reconcile.

7. **The phrase "I" appears around 10 times.** If your supervisor prefers a depersonalised academic register, this needs a sweep.

8. **NREL date claim:** body says "as of March 2026", reference [13.2] says "2026-03-19" — fine, just make sure you're confident the NREL chart was actually updated on that date (today's date is 2026-04-19, so this is plausible).

---

## Priority order for fixes

If you have limited time, address in this order:

1. **Add in-text citations everywhere** (single biggest mark loss).
2. **Fix the broken sentence in §2.3** ("…increase rapidly energy delivery…").
3. **Add a Contents page** and **renumber References to §5**.
4. **Resolve the §2.1 vs §3 contradiction** about whether the project addresses the research gap.
5. **Decide on Harvard vs IEEE referencing** with your supervisor and apply consistently.
6. **Sweep contractions, encoding artefacts, and US/UK spelling.**
7. **Add at least one quantitative comparison** (table or paragraph) in §2.3.
8. **Define MAV scope and acknowledge the size-scaling gap** vs the cited solar UAV literature.
