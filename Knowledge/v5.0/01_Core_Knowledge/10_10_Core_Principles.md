# 10_10_Core_Principles

> This module summarises the foundational philosophies and frameworks for AI‑assisted songwriting in the Suno
> ecosystem.  It modernises the v4.5 core principles to align with Suno V5’s concise prompting paradigm, reliable
> exclusions, improved audio fidelity and stems‑based workflows【333682324514163†L29-L33】【714812518803694†L8-L28】.  The goal is to
> empower the **AI‑Assisted Artisan** with systems that blend human creativity and machine precision.

## 1. Mindset: The AI‑Assisted Artisan

Suno AI is a collaborator, not a substitute.  Treat songwriting as a deliberate craft rather than a mystical
process.  Adopt a **“dare to suck”** mindset—create boldly and iterate.  Think of yourself as a songwriter‑corporation:
assign roles (composer, lyricist, producer, mix engineer) and manage them efficiently.  Maintain authenticity by
drawing from personal experiences and focusing on the listener’s emotional journey.  The user remains the auteur;
Suno is the architect that provides systems and blueprints.

## 2. Foundational Frameworks

### 2.1 Addiction Formula

The **Addiction Formula** models a song’s energy curve using three components—**Hype**, **Tension** and
**Implied Tension**—which should rise and fall across sections to keep listeners engaged.  Structure your
arrangement so that choruses deliver the maximum release after a controlled build‑up, verses introduce new details
to reset tension and bridges provide contrast and set up the final chorus.

### 2.2 PRA Method (Pattern, Repetition, Arc)

Memorable melodies follow a balance of repetition and variation.  Build a core pattern (a melodic motif), repeat it
to establish familiarity, and then introduce variation to create an arc.  Use PRA at both the micro level (within a
phrase) and the macro level (across sections) to keep listeners hooked.

### 2.3 The Six Elements of Holistic Songwriting

1. **Arrangement:** Orchestration choices and overall track structure.
2. **Harmony:** Chord progressions and harmonic devices (modal interchange, secondary dominants, tritone substitutions).
3. **Rhythm:** Groove and rhythmic patterns; advanced techniques include syncopation, polyrhythms and odd time signatures.
4. **Part‑writing:** Interaction between lead lines and supporting voices.
5. **Lyrics:** Narrative content, imagery, rhyme, meter and prosody.
6. **Production:** Timbre, mixing, effects and dynamics.

These elements are interdependent; a small change in one influences the others.  Use them intentionally to
support your energy curve and lyrical story.

## 3. Suno V5 Creative Frameworks

### 3.1 Three‑Layer Prompting【629117737649120†L73-L113】

Effective prompts have three layers:

- **Style nucleus & mood/energy:** Define the core genre (e.g., *indie rock*, *cinematic electronic*) and
  mood/energy adjectives (*dreamy*, *melancholic*).  Add the vocal persona (e.g., *female tenor*, *gritty male*) and
  one or two key instruments (e.g., *acoustic guitar*, *synth pads*).  Conclude with a production feel (e.g.,
  *lo‑fi*, *polished*).
- **Structural syntax & tags:** Use square brackets `[ ]` to mark sections like `[Verse]`, `[Chorus]`, and optional
  modifiers such as `[Chorus: soaring]`.  Use parentheses `( )` for performance cues or ad‑libs.  Keep tags minimal
  and avoid excessive FX micro‑management.  If needed, provide a succinct duration (e.g., *3:00*) and include
  exclusions at the end (e.g., `EXCLUDE: no saxophone, no EDM`).
- **Poetic structure:** Provide optional lyrical snippets as short, concrete stanzas.  Focus on vivid imagery,
  monosyllabic hooks and consistent syllable counts.  Punctuation and line breaks implicitly shape the melody and
  pacing.

### 3.2 Concise Directives & Exclusions【333682324514163†L29-L33】【333682324514163†L34-L37】

V5 rewards prompts that are short and descriptive.  Replace v4.5’s chronological story instructions with concise
style directives.  Use one or two words per descriptor and avoid synonym stacking or contradictory genre cues【333682324514163†L52-L61】.
Functional exclusions are reliable: limit to two and place them at the end of the prompt using `EXCLUDE:` or “no X”
phrases.  If the model ignores them, move the exclusions earlier and remove conflicting descriptions【333682324514163†L34-L37】.

### 3.3 Pre‑Flight & Iterative Workflow【333682324514163†L29-L33】【714812518803694†L8-L28】

Before generating:

1. **Intent audit:** Define your style nucleus, mood/energy, vocal persona, instrumentation, production feel, exclusions
   and target length.  Document your prompt and any lyrics for reproducibility.
2. **Harmony & rhythm planning:** Sketch your chord progression and rhythmic groove to ensure energy control through
   Hype, Tension and Implied Tension (Addiction Formula) and to support melodic arcs (PRA Method).

After generation:

1. **Select the best take:** Listen to multiple takes and choose the one with the most compelling energy curve and
   production.
2. **Export stems and mix:** Export stems (drums, bass, guitars/synths, vocals, FX) and perform a quick mix audit.
   Apply targeted EQ—high‑pass non‑bass instruments at 80–120 Hz, cut 200–350 Hz to reduce mud and add air at
   8–10 kHz—and glue compression on the master bus to hit streaming‑safe loudness (−14 to −9 LUFS, ≤ −1.0 dBTP)【714812518803694†L8-L28】.
3. **Partial regeneration:** Use stems and seeds to regenerate only problematic sections or layers rather than rerolling
   the entire track.  Iterate until arrangement and mix are balanced.

### 3.4 Troubleshooting & Pitfalls【333682324514163†L52-L61】【333682324514163†L63-L65】

Common pitfalls inherited from v4.5 include:

- **Over‑scripting & metatag overload:** Long sequences of tags confuse the model and break structural coherence.  Use
  minimal tags and let the model infer arrangements within the defined structure.
- **Contradictory genre cues:** Mixing incompatible descriptors (e.g., *“punk EDM jazz fusion”*) will confuse the model.
  Limit yourself to a single genre family and a few complementary adjectives.
- **Extreme BPM demands:** V5 may normalise unrealistic tempo instructions.  Instead of specifying BPM, describe the
  desired energy (e.g., *fast‑paced*, *slow and hypnotic*)【333682324514163†L63-L65】.
- **Redundant synonyms:** Stacking multiple synonyms (e.g., *“happy, joyful, cheerful”*) wastes tokens; choose the most
  precise word and move on.

If you encounter issues, consult the troubleshooting framework for targeted solutions【714812518803694†L8-L28】.

## 4. v4.5 → V5 Changes

- **Concise vs narrative prompts:** V5 interprets short, descriptive directives; narrative story prompts are obsolete【333682324514163†L29-L33】.
- **Reliable exclusions:** Explicit negations are honoured when limited and well‑placed【333682324514163†L34-L37】.
- **Cleaner mixes & stems:** V5 outputs cleaner mixes by default and enables stems export and partial regeneration【714812518803694†L8-L28】.
- **Enhanced adherence:** The model adheres more closely to structural tags and length instructions【333682324514163†L44-L48】.
- **New pitfalls:** Over‑scripting, metatag overload and unrealistic tempo demands degrade output【333682324514163†L52-L61】【333682324514163†L63-L65】.

## 5. Examples

1. **Directive vs narrative prompt**

   - Bad (v4.5 style): “Write a detailed story about two lovers who meet at a coffee shop, describe their dialogue,
     their feelings, their actions in each verse, and build to a chorus where they confess their love.”
   - Good (V5 style): “Indie pop duet, bittersweet, male and female vocals, acoustic guitar and soft synth pad,
     no drums, 3:30, lyrics about meeting at a coffee shop and falling in love.”

2. **Three‑layer prompt with exclusions**

   ```
   Pop rock, triumphant, gritty male vocals, electric guitar, wide drums, polished
   [Verse]
   Our hearts beat louder than the city lights
   We run until the dawn breaks free
   [Chorus: soaring]
   We are the fire in the night
   Burn it up, can’t you see?
   EXCLUDE: no saxophone, no EDM
   ```

3. **Pre‑flight & iterative workflow**

   - Define intent: “Cinematic electronic ballad, dreamy, female vocals, lush synth pads, no drums, 3:00, lyrics about
     cosmic isolation.”
   - Generate multiple takes; choose the one with the best balance of atmosphere and clarity.
   - Export stems; if the bass is boomy, high‑pass non‑bass instruments at 80–120 Hz and cut 200–350 Hz.
   - Regenerate only the chorus using the same prompt and seeds if it feels weak.

4. **Avoiding pitfalls**

   - Instead of “fast BPM 180, high‑energy, adrenaline, intense, furious,” write “hard‑hitting metal, aggressive,
     intense” and let the model determine tempo.
   - Avoid listing synonyms like “bright, cheerful, happy”; choose the one that best captures your intent.

## 6. First‑Run Checklist

- [ ] Identify your role: composer, lyricist, producer, or overall arranger.
- [ ] Familiarize yourself with the Addiction Formula and PRA Method to manage energy and melodic arcs.
- [ ] Define the six elements of your song (arrangement, harmony, rhythm, part‑writing, lyrics, production).
- [ ] Perform an intent audit and craft a concise three‑layer prompt.
- [ ] Include at most two exclusions; avoid over‑tagging and unrealistic BPM.
- [ ] Generate and select the best take; export stems and apply quick EQ fixes【714812518803694†L8-L28】.
- [ ] Use partial regeneration to fix problem sections; iterate until satisfied.
- [ ] Consult the troubleshooting framework if issues persist.
