# Song Blueprint Generator (Suno V5 Edition)

The Song Blueprint Generator is a web application that pairs structured songwriting craft with Suno V5’s prompt vocabulary. Users supply titles, lyrics, and contextual notes, then the tool assembles V5-aligned style prompts, lyric scaffolds, and production checklists so every generation starts with a clear intent and minimal rework.

> **V4.5 → V5 Changes**
> - Blueprint prompts now prioritize concise directives, two-or-fewer exclusions, and minimal metatag clutter to match V5’s migration guardrails.
> - Negative prompting (`EXCLUDE:`/`without`) is promoted to a first-class control because V5 reliably honors functional negations.
> - Default mix guidance assumes V5’s cleaner baseline while adding stem-level fixes for the model’s occasional low-end bias.

## Platform Overview

- **Account & Provider Support**
  - Email/password login with encrypted storage for multiple OpenAI-compatible base URLs and per-provider API keys.
  - Built-in integrations: OpenRouter smart routing, Google Gemini via AI-SDK, and bring-your-own Suno-compatible endpoints.
- **Project Dashboard**
  - Health indicator tracks credential completeness and reports API errors before generation requests fire.
  - Users can save global defaults or blueprint-specific overrides for model, temperature, max tokens, top-p, top-k, and banned phrase lists.
- **Blueprint Workspace**
  - Multi-pane editor accepts title, optional style nucleus, raw lyrics, and additional context notes.
  - Output can be downloaded as Markdown, stored as JSON for library reuse, or exported as stems-ready checklists.

## V5 Blueprint Workflow

1. **Ingest Source Material** – Collect draft lyrics, target genre, and reference energy arcs. Tag any mandatory exclusions (e.g., no drums) upfront.
2. **Intent Audit** – Summarize the style nucleus, mood, vocal persona, and key instruments in ≤2 words each. Reserve only one production feel adjective and plan ≤2 exclusions.
3. **Lyric Structure Planning** – Use section headers (`[Verse]`, `[Chorus]`, `[Bridge]`) sparingly. Reserve parentheses for sung ad-libs. Ensure syllable counts support the intended groove.
4. **Generation Settings** – Select a V5-capable provider, keep temperature moderate (0.6–0.8) for controllability, and set target duration explicitly (e.g., `2:45`).
5. **Review & Stem Prep** – After generation, capture prompts, lyrics, and health metadata, then export stems to balance low end or re-gen sections without discarding strong material.

### Recommended Defaults

| Setting | Default | Why |
| --- | --- | --- |
| Title inclusion | Enabled | Reinforces hook focus when V5 obeys concise directives. |
| Style/metatag guidance | Enabled with brevity | Maintains high-signal intent while avoiding v4.5-style scripting. |
| Output specificity | Normal | Section-level guardrails prevent over-programming. |
| Original lyric reuse | Avoid | Encourages derivative-free rewrites while retaining thematic continuity. |
| Duration | 2:30 | Aligns with V5’s reliable length obedience; adjust per project. |

## V5 Prompt Design Guardrails

- Follow the grammar: **style nucleus → mood/energy → vocal persona → key instruments → production feel → exclusions → length → optional theme**.
- Cap exclusions at two. Move them to the front only when the model ignores them, and remove any conflicting descriptors.
- Use one decisive production adjective (`dry room`, `wide stereo`) instead of stacking processors.
- Encode dynamic contrast with simple energy cues (e.g., `tense verse`, `soaring chorus`) rather than procedural staging.

## Example Blueprints

### 1. Narrative Prompt (Indie Pop)
```
Title: Midnight Frequency
Style Prompt: indie pop, bittersweet, airy female vocal, clean electric + warm pads, subtle reverb, EXCLUDE: no acoustic guitar. 2:45. Theme: quiet resilience.
Section Outline:
- [Verse 1] Focus on city-after-rain imagery, medium energy.
- [Chorus] Hook: "Keep the midnight frequency alive." Lift energy with layered harmonies.
- [Bridge] Strip back to pads, rebuild with rising drums into final chorus.
Notes: Export stems to double-check low end after first take.
```

### 2. Structured JSON Prompt (Alt Rock Blueprint)
```json
{
  "title": "Static Proof",
  "style_prompt": "alternative rock, urgent, gritty male vocal, distorted guitars + tight kit, dry room, EXCLUDE: no synth pads. 2:30. Theme: standing your ground.",
  "lyric_scaffold": {
    "verse_1": "Map scenes of city grit, 7-7-7 syllable pattern",
    "pre_chorus": "Add rising tension cues, single-word power verbs",
    "chorus": "Repeat line-plus-three hook, all caps on core phrase",
    "bridge": "Introduce spoken aside (focus) using parentheses"
  },
  "mix_notes": [
    "High-pass non-bass parts at 90 Hz",
    "Check LUFS target (-10 integrated) before export"
  ]
}
```

### 3. Constraint Blueprint (Acoustic Ballad with Negative Prompting)
```
Title: Paper Lantern Vows
Style Prompt: acoustic folk, intimate, tender male vocal, fingerpicked guitar + light room, EXCLUDE: no drums, without electric bass. 3:00. Theme: vows by candlelight.
Lyric Directions:
- [Verse 1] Specific sensory images of warm light, 8-8-6 syllables.
- [Chorus] Universal promise language, reuse "lantern" as anchor.
- [Outro] Whispered refrain in parentheses for soft fade.
Troubleshooting Cue: If accompaniment adds percussion, move "EXCLUDE" to prompt front and regenerate chorus only.
```

### 4. Lyric & Vocal Control Blueprint (Electro Ballad)
```
Title: Signal Bloom
Style Prompt: downtempo electro pop, dreamy, breathy female vocal, glassy synths + pulsing bass, lush stereo, EXCLUDE: harsh lead guitar. 2:50.
Lyrics Draft:
[Verse 1]
Neon veins in the midnight glow,
Breathing slow as the currents flow,
(ahh)
[Chorus]
Hold this signal bloom tonight,
Let the quiet feel like light,
(yeah, yeah)
[Bridge: whispered]
Tracing pulses down the wire,
[Outro]
Fade the echo, keep the fire.
Execution Notes: Keep bracket modifiers minimal and ensure ad-libs remain in parentheses.
```

### 5. Troubleshooting Blueprint (Boomy Mix Recovery)
```
Scenario: First take comes back with heavy low end and a shorter runtime than requested.
Response Plan:
1. Export vocal and instrumental stems.
2. Apply -3 dB shelf between 90-200 Hz on instrumental stem; re-balance kick vs bass.
3. Restate length as "3:15" and remove redundant adjectives before regenerating the bridge.
4. Archive both prompts, noting the exclusion placement that produced the cleaner mix.
```

## Troubleshooting Recipes

| Issue | Mitigation |
| --- | --- |
| Boomy or muddy mix | Export stems, cut 90–250 Hz by 2–3 dB, and keep limiter at -1.0 dBTP before re-export. |
| Structure drift | Simplify the style prompt, keep section tags minimal, and regenerate only the offending section. |
| Tempo ignored | Swap explicit BPM for energy adjectives; if tempo is critical, make it the sole numeric directive. |
| Negative prompt ignored | Move the `EXCLUDE:` clause ahead of production cues and remove conflicting descriptors. |

## First-Run Checklist

- Style nucleus, mood, and vocal persona captured in ≤12 words.
- Production feel limited to one descriptor; exclusions ≤2 and clearly worded.
- All sections tagged once; parentheses only for sung asides or ad-libs.
- Target duration stated; prompt, lyrics, and settings saved for reproducibility.
- Stems exported or queued for export after first acceptable take.
- Troubleshooting plan logged (e.g., low-end EQ, section re-gen) before committing the blueprint.

## Cognitive Verifier Prep

- **Coverage:** Ensure no lingering v4.5 terminology (e.g., chronological scripting) remains in saved templates.
- **Authority:** Tie every prompt template back to the canonical V5 grammar and exclusion rules.
- **Prompts:** Verify each example demonstrates concise directives, energy control, and safe use of `EXCLUDE:`.
- **Clarity:** Blueprint steps should be actionable for first-time users, reinforced by the checklist.
- **Consistency:** Glossary terms (style nucleus, exclusions, stems) match the V5 Latest Knowledge language.
