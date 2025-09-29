# 10_30_Troubleshooting_Framework

> This updated troubleshooting framework diagnoses common issues encountered when co‑creating music with Suno V5
> and provides actionable solutions rooted in the Addiction Formula, PRA Method and V5’s specific capabilities.
> It supersedes the v4.5 table by incorporating V5’s cleaner mixes, reliable exclusions, stems workflow and
> revised prompt syntax【714812518803694†L8-L28】【333682324514163†L29-L33】.

## Diagnosing & Solving Common Songwriting Flaws

The table below maps frequent symptoms to their probable causes in the V5 model and offers targeted remedies.  Use
this as a quick reference when your generated tracks do not meet expectations.

| **Common Symptom** | **Probable Cause (V5)** | **Actionable Solution (Framework & Suno Tactic)** |
| --- | --- | --- |
| **Mix feels muddy or boomy** | Excess low‑end or crowded midrange in the arrangement; lack of high‑pass filtering | **Export stems and balance.** High‑pass non‑bass instruments at 80–120 Hz; cut 200–350 Hz to clear mud; add air at 8–10 kHz. Remove redundant instruments or conflicting descriptors in the prompt. Re‑generate sections if necessary【714812518803694†L8-L28】. |
| **Song length is off (too long/short)** | Missing or ambiguous duration in the prompt; unrealistic tempo demands | **Specify length succinctly** (e.g., “3:00”). Use partial regeneration to fix sections that are too long/short. Avoid unrealistic BPM instructions; describe energy instead【333682324514163†L63-L65】. |
| **Ignored exclusions or unwanted instruments** | Too many exclusions; contradictory descriptors; exclusions buried in the prompt | **Limit to two exclusions** and place them at the end (e.g., `EXCLUDE: no saxophone, no EDM`). If ignored, move the exclusion earlier and remove conflicting descriptors. Regenerate only offending stems or sections【333682324514163†L34-L37】. |
| **Flat energy / sections lack dynamics** | Insufficient energy cues; repetitive patterns; neglect of PRA arcs | **Add a single energy cue** per section (e.g., `[Chorus: soaring]`, `[Bridge: quiet]`). Introduce variation via the PRA Method—repeat the motif then vary it to create an arc. Consider adjusting instrumentation to create contrast【629117737649120†L73-L113】. |
| **Genre drift or confused style** | Conflicting descriptors, synonym stacking or over‑scripting | **Simplify the style nucleus.** Choose one genre family and one or two mood descriptors. Remove redundant synonyms and conflicting tags. If drift persists, regenerate with a pared‑down prompt【333682324514163†L52-L61】. |
| **Vocal balance issues (too loud/quiet)** | Vocal stem not balanced in the mix; inadequate compression/EQ | **Export the vocal stem** and apply subtle compression and EQ. High‑pass at 80–120 Hz, cut harsh mids and add air. Reduce competing midrange instruments or use `Add Vocals` to overlay a more balanced performance【714812518803694†L8-L28】. |
| **Structural tags ignored / sections misaligned** | Over‑tagging or conflicting instructions; missing pre‑flight check | **Use minimal section markers** and follow the recommended grammar order. Ensure each section has a clear purpose. Regenerate only the offending section using the same seeds. Perform the pre‑flight checklist before next generation【629117737649120†L73-L113】. |

## v4.5 → V5 Changes

- **Mix & stems fixes:** V5’s cleaner mixes mean global “mastering hacks” are obsolete; instead, apply targeted EQ and
  stems balancing【714812518803694†L8-L28】.
- **Length adherence:** V5 respects stated durations more closely; always provide a length if it matters【333682324514163†L44-L48】.
- **Exclusions reliability:** Negations are honoured when concise and well‑placed【333682324514163†L34-L37】.
- **Pitfalls:** Over‑scripting, excessive tags and unrealistic BPM demands still degrade results【333682324514163†L52-L61】【333682324514163†L63-L65】.

## First‑Run Checklist

- [ ] Identify the symptom you are experiencing.
- [ ] Review the probable causes to verify whether your prompt or mix may be at fault.
- [ ] Apply the suggested solution: adjust the prompt (length, exclusions, descriptors), export stems for mixing, add or
  adjust energy cues or regenerate specific sections.
- [ ] Iterate and re‑evaluate until the issue is resolved.  Save each prompt and mix configuration for reproducibility.
