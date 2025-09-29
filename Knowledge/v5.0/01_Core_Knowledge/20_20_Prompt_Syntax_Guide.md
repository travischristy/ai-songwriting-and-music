# 20_20_Prompt_Syntax_Guide

## Suno V5 Prompt Syntax & Grammar

This guide replaces the v4.5 “lyrical syntax” analysis with an actionable reference for crafting effective prompts in Suno V5.  It distills community wisdom and official guidance into a concise set of rules and examples.

### 1. Core Principles of V5 Prompting

V5’s architecture rewards **clarity and brevity**.  Avoid the exhaustive, chronologically scripted prompts that worked in v4.5; instead, focus on high‑level direction【333682324514163†L29-L33】.  In practice this means:

1. **Style nucleus → Mood → Persona → Instrumentation → Production feel → Exclusions → Length**.  Arrange your style prompt elements in this order and use no more than one or two descriptors per slot【333682324514163†L29-L33】.
2. **Explicit negatives**.  Remove unwanted instruments or qualities via phrases like “no drums” or with an `EXCLUDE:` clause.  Place exclusions near the end of your style prompt and limit them to two【333682324514163†L34-L37】.
3. **Minimal metatagging**.  Structural tags (e.g., `[Verse]`, `[Chorus]`) and performance notes (e.g., `[whispering]`) remain essential, but over‑tagging can confuse V5【333682324514163†L52-L61】.  Use tags sparingly and avoid nested brackets.
4. **Separate sung content from instructions**.  Use **square brackets** for non‑lyrical instructions and **parentheses** only for text you want the model to vocalise (ad‑libs, echoes).  Do not place commands inside parentheses, as they will be sung【333682324514163†L44-L48】.
5. **Three layers of control**.  Effective prompting harmonises the high‑level style prompt, explicit lyrical syntax (meta tags and performance notes) and the implicit poetic structure (rhyme, rhythm, and syllable patterns)【333682324514163†L73-L108】.

### 2. Structural & Performance Tags

- **Section tags**: `[Intro]`, `[Verse]`, `[Pre‑Chorus]`, `[Chorus]`, `[Bridge]`, `[Outro]`.  These markers tell the model how to arrange the song.  Place them on their own line or at the start of the line in the lyrics box.
- **Performance tags**: `[whispering]`, `[falsetto]`, `[shouting]`, `[rap verse]`.  These modify how subsequent lyrics are delivered.
- **Sound design tags**: `[sound of rain]`, `[vinyl scratch]`, `[crowd cheering]`.  Use these sparingly to insert environmental or sound‑effect cues.
- **Modifiers**: You can append a colon and modifiers to a section tag for more detail (e.g., `[Chorus: sparse, quiet]`) but avoid long lists【333682324514163†L52-L61】.

### 3. Negative & Constraint Prompts

V5’s improved obedience makes negative prompting a powerful tool.  To exclude an instrument or quality:

- Use simple language like “no heavy metal guitars” or `EXCLUDE: distorted guitars`.  Place this at the end of the style prompt【333682324514163†L34-L37】.
- Avoid stacking more than two exclusions.  If the model still includes the unwanted element, move the exclusion earlier in the prompt or reduce conflicting descriptors【333682324514163†L55-L61】.

### 4. Prompt Examples

The following examples illustrate the recommended syntax for common scenarios.  Adjust descriptors and exclusions to fit your creative vision.

#### 4.1 Narrative Style Prompt

```
dreamy synth‑pop anthem with intimate female vocals, bright arpeggiated synths, punchy 808‑style drums; mid‑tempo at 100 BPM. EXCLUDE: distorted guitars
```

This succinct description specifies the style nucleus, instrumentation, tempo and an exclusion.  It avoids chronological scripting and trusts V5’s arrangement capabilities【333682324514163†L29-L33】.

#### 4.2 Structured JSON Prompt

Suno V5 supports structured inputs for certain advanced workflows.  Use JSON format to define discrete properties:

```json
{
  "style": "jazzy lo‑fi hip‑hop with vinyl crackle",
  "mood": "relaxed and nostalgic",
  "vocals": "male baritone, soft delivery",
  "instruments": ["upright bass", "electric piano", "brush drums"],
  "length": "2:30",
  "exclude": ["saxophone"]
}
```

Values should be concise; arrays should contain no more than three items.  This structure mirrors the recommended prompt grammar and ensures consistent parsing.

#### 4.3 Constraint / Negative Prompt

```
alternative folk ballad with warm acoustic guitar and gentle harmonica. EXCLUDE: drums, synthesiser
```

This example demonstrates the use of two exclusions to ensure a stripped‑back arrangement.  Place exclusions at the end of the prompt for best compliance【333682324514163†L34-L37】.

#### 4.4 Lyric & Vocal Control

```
[Verse]
I wander through the city lights
alone but feeling free tonight
[Chorus: soaring, full band]
Light up the sky above my head
sing with the stars, I won't forget
(yeah!) (ooh‑woah)
```

Square brackets denote the section and performance character.  Parentheses add vocalised ad‑libs; they are sung as written【333682324514163†L44-L48】.

#### 4.5 Troubleshooting Prompt

If your song exhibits a boomy low‑end or muddy mix, you can correct it through prompting and mixing:

```
dark trap beat with clean 808 bass and crisp hi‑hats; EXCLUDE: boomy bass, overly saturated low end
```

After generation, export stems and apply a high‑pass filter to non‑bass elements at 80–120 Hz and a wide cut around 200–350 Hz【714812518803694†L8-L28】.  Aim for ‑14 LUFS integrated loudness and a ‑1 dBTP ceiling on the master【714812518803694†L19-L28】.

### 5. First‑Run Checklist

Before generating a song, ensure that you:

1. Define the style nucleus, mood and vocal persona clearly.
2. Limit instrumentation and production descriptors to a few key elements.
3. Specify one or two exclusions if necessary.【333682324514163†L34-L37】
4. Use structural tags and performance notes sparingly.
5. Save your prompt and lyrics for reproducibility and iterate via stems or section regeneration.