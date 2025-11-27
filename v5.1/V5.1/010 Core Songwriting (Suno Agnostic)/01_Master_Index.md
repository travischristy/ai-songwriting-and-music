# 00_10_Master_Index — Suno V5 Knowledge Hub

The Master Index curates every production-grade practice we now treat as canonical for Suno V5. It replaces the v4.5-era inventory with concise directives, negative prompting discipline, and stem-first editing so teams can navigate the migration without guesswork.[^global]

> **How to use this file:** Start with the guardrails below, then jump to the pillar that matches your task. Each pillar links to the V5 rewrite (or migration-in-progress) and highlights the workflows, examples, and QA loops you should expect to reference day-to-day.

## V4.5 → V5 Changes at a Glance
- **Prompting philosophy:** Swap chronological “story prompts” for short, high-signal briefs that front-load style, mood, vocal persona, and exclusions.[^global][^paradigm]
- **Negative control:** Rely on explicit `EXCLUDE:` or "no ___" instructions (≤2) to sculpt instrumentation; move exclusions earlier only if the model ignores them.[^exclusions][^negative]
- **Audio & editing:** Trust V5’s cleaner baseline mix, then use stem exports and partial regeneration to target problems instead of rerolling entire songs.[^editing][^troubleshoot]
- **Length & structure:** Expect better obedience to section tags and duration requests; fix drift section-by-section rather than rewriting whole tracks.[^troubleshoot]
- **Known quirks:** Watch for bass-heavy mixes and tempo normalization—mitigate with prompt exclusions and surgical EQ around 90–250 Hz.[^boomy]

## Global Guardrails for Every Document
1. **Concision wins:** If a human lead sheet communicates the same intent, trim the prompt. Paring down improves arrangement inference and take-to-keep ratios.[^global]
2. **Single production color:** Commit to one mix descriptor (e.g., *dry room*) and let instrumentation carry nuance.[^prompt]
3. **Minimal markup:** `[Section]` tags define structure; parentheses add ad-libs; anything extra risks literalism.[^markup]
4. **Exclusion budget:** Cap negations at two items and keep them conflict-free to avoid deadlocks.[^exclusions]
5. **Document everything:** Archive prompt, lyrics, seed, stems, and QC notes for reproducibility.[^editing]

## Knowledge Pillars (Suno V5)
| Pillar | Purpose | Status |
| ------ | ------- | ------ |
| **Implementation Doctrine** — `10_10_Core_Principles.md` | Distills migration rules, PRA, and energy management tuned for concise prompting. | Needs V5 rewrite (scheduled Task #3). |
| **Operational Workflows** — `10_20_Songwriting_Workflows.md` | Batch generation, selection checklists, stems/partial regen recipes. | Needs V5 rewrite (Task #4). |
| **Troubleshooting Framework** — `10_30_Troubleshooting_Framework.md` | Quick triage for mix haze, length drift, structural errors, and genre fidelity. | Needs V5 rewrite (Task #5). |
| **Prompt Syntax Guide** — `20_20_Prompt_Syntax_Guide.md` | Prompt grammar, EXCLUDE patterns, JSON/structured templates, pre-flight checklist. | Needs V5 rewrite (Task #7). |
| **AI-Assisted Artisan Appendix** — `Appendix_10_The_AI_Assisted_Artisan.md` | Evergreen craft married to V5 operational heuristics and verification loop. | Needs V5 rewrite (Task #8). |
| **System Instructions** — `../../v4.5/04_Instructions/System Instructions/*` | Legacy prompts for copilots and assistants. | Convert to V5 voice after core syntax updates (Task #13). |
| **Style Emulation Suite** — `v5.0 Migration Reference/Latest Knowledge/Style Emulation/*` | Authoritative reference for sonic analysis, fusion, and covers without artist names. | Canonical (import facts directly). |

## Prompt Playbook (V5-Ready Examples)
### 1. Narrative Brief (Concise Style Prompt)
```
indie pop, bittersweet, airy female vocal, clean electric + warm pads, subtle reverb, EXCLUDE: no acoustic guitar. 2:30. Theme: quiet resilience.
```
- **Why it works:** Front-loads intent with one production cue, a single exclusion, and explicit length, matching the recommended order.[^prompt]

### 2. Structured JSON Prompt (Custom Mode)
```json
{
  "style_prompt": "alternative rock, urgent, gritty male vocal, distorted guitars + tight kit, dry room, EXCLUDE: no synth pads. 2:45.",
  "lyrics": "[Verse]\nStreetlights hum in restless glow\nKeep my eyes on where to go\n[Chorus]\nHold the line, we're breaking through\n(yeah) we won't fade in two",
  "metadata": {
    "seed": "riff-882.wav",
    "target_length_seconds": 165,
    "notes": "Use for album opener; tighten low end in mix stage"
  }
}
```
- **Usage:** Pair lean text with a complementary audio seed and keep metadata for reproducibility.[^prompt][^multimodal]

### 3. Constraint Example (Negative Prompting)
```
nocturne-inspired ambient pop, glassy synths + soft piano, whispery female vocal, EXCLUDE: no drums, without boomy bass. 3:10.
```
- **Outcome:** Two exclusions target percussion and low-end buildup while staying within the allowed budget.[^exclusions][^boomy]

### 4. Lyric & Vocal Control Snippet
```
[Verse]
Flicker lights on the kitchen floor
We talk in whispers through the storm
(oh-oh) keep it close, don't let me go
[Chorus: soaring]
Hold me steady when the night leans in
We'll outrun the echo, breathe it in
```
- **Notes:** Sparse tags define structure and energy while parentheses add sung ad-libs.[^markup][^troubleshoot]

### 5. Troubleshooting Regeneration
> **Scenario:** Chorus lands flat and mix feels muddy on first pass.
> 
> **Fix:** Export stems, re-gen only the chorus with a single energy cue (*[Chorus: soaring]*), then apply a -2 dB shelf around 200–350 Hz to clear mud.[^troubleshoot][^stems]

## First-Run Checklist
1. Confirm prompt order (style → mood → vocal → instruments → production → exclusions → length).[^prompt]
2. Limit exclusions to two, phrased as "no ___" or `EXCLUDE:` statements.[^exclusions]
3. Keep section tags minimal and reserve parentheses for sung ad-libs.[^markup]
4. Generate three takes, pick the strongest vocal/arrangement pairing, and log prompt + lyrics.[^editing]
5. Export stems, check bass vs. kick balance, and document any EQ moves.[^stems]
6. Archive take-level notes for QA sign-off and future reuse.[^editing]

## QA + Cognitive Verifier Hooks
- **Coverage:** Inspect every migrated doc for lingering `v4.5` strings using `index-v45.txt` before sign-off.
- **Authority:** Cross-check claims against the facts ledger IDs listed below.
- **Prompts:** Ensure each example reflects the concise syntax, exclusion limits, and markup discipline captured here.[^prompt][^negative]
- **Clarity:** Attach the First-Run Checklist to derivative docs so new contributors can execute without back-channel guidance.
- **Consistency:** Use shared terminology (hype, tension, implied tension) when describing energy curves and troubleshooting steps.[^style]

## Facts Ledger References
- v5_global_migration_rules, v5_editing_best_practices, v5_troubleshooting_framework, v5_prompt_grammar, v5_preflight_checklist, v5_exclusion_guidance, v5_negative_prompting, v5_boomy_bass_fix, v5_stems_mixing, v5_style_deconstruction, v5_lyrics_markup_rules.

---

[^global]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Global Migration Rules (lines 10-16).
[^paradigm]: *An Advanced Guide to High-Quality Music Creation with Suno V5*, V5 paradigm shift bullets (lines 15-18).
[^exclusions]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Exclusions guidance (lines 163-168).
[^negative]: *An Advanced Guide to High-Quality Music Creation with Suno V5*, Negative prompting section (lines 188-200).
[^editing]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Workflow 1 + operational checklist (lines 82-88).
[^troubleshoot]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Troubleshooting Framework (lines 107-129).
[^boomy]: *An Advanced Guide to High-Quality Music Creation with Suno V5*, Troubleshooting table (lines 175-180).
[^prompt]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Prompt Grammar & Templates (lines 143-158).
[^markup]: *The Complete Guide to Sonic Emulation in Suno V5*, syntax rules (lines 104-129).
[^multimodal]: *Suno V5 — Core Knowledge (Consolidated Edition)*, Multimodal seeds guidance (lines 181-184).
[^stems]: *Suno v5 — Stems & Mixing Quick Fixes*, stems workflow + EQ (lines 9-26).
[^style]: *The Complete Guide to Sonic Emulation in Suno V5*, energy curve language (lines 17-76).
