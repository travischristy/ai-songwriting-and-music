# 10_20_Songwriting_Workflows

> This module provides a modern roadmap for creating songs with Suno V5.  It summarises the foundational
> philosophies of the AI‑Assisted Artisan and introduces an updated co‑writing workflow that leverages V5’s
> concise prompting, reliable exclusions, stems export and mixing features.  It replaces the v4.5 outline and
> focuses on practical application【333682324514163†L29-L33】【714812518803694†L8-L28】.

## 1. Introduction: A New Paradigm for the AI‑Assisted Artisan

Generative AI is reshaping music creation.  In V5, Suno acts as a co‑writer capable of realising high‑quality
arrangements from short, descriptive prompts.  The knowledge base serves as your manual, guiding you through the
craft of songwriting and the art of prompt engineering.  This document outlines the core workflow and offers
genre‑specific considerations.

## 2. Part I: Foundations of Craft (Overview)

The foundations of AI‑assisted songwriting are described in detail in the **Core Principles** document.  In summary:

- **Mindset:** Embrace deliberate practice, authenticity and audience awareness.  Treat AI as a collaborator and
  adopt the songwriter‑corporation mindset.
- **Methodologies:** Apply the Addiction Formula to manage energy curves and the PRA Method to shape melodic arcs.
- **Six Elements:** Orchestrate arrangement, harmony, rhythm, part‑writing, lyrics and production in concert.
- **Advanced Craft:** Explore lyrical blueprinting, song mapping, melodic hotspots and interval jumps for
  sophisticated expression.

Refer to `10_10_Core_Principles.md` for deeper explanations.

## 3. Part II: V5 Co‑Writing Workflow

### 3.1 Define the Intent (Pre‑Flight Checklist)【333682324514163†L29-L33】【629117737649120†L73-L113】

1. **Style nucleus & mood:** Choose a genre or sub‑genre (e.g., *lo‑fi hip‑hop*, *symphonic metal*) and mood/energy
   descriptors (e.g., *melancholic*, *high‑energy*).  Add the vocal persona and one or two key instruments.
2. **Production feel & exclusions:** Specify a production aesthetic (*polished*, *gritty*, *lo‑fi*) and any
   instruments or styles to exclude (`EXCLUDE: no saxophone, no EDM`)【333682324514163†L34-L37】.
3. **Length & lyrical topic:** State the desired duration succinctly and optionally provide a lyrical theme.
4. **Document:** Save your prompt and any lyrics for later reference.

### 3.2 Craft the Prompt

Compose a concise directive following the recommended grammar order: style → mood/energy → vocal persona →
instruments → production feel → exclusions → length → lyric topic【629117737649120†L73-L113】.  Use square brackets `[ ]`
for structural sections and parentheses `( )` for performance cues.  Provide optional lyrical stanzas with concrete
imagery and natural spelling.  Avoid over‑scripting or synonym stacking【333682324514163†L52-L61】.

### 3.3 Generate & Select

Run generation and listen to multiple takes.  Evaluate the energy curve (Addiction Formula), melodic arc (PRA) and
production quality.  Choose the take that best aligns with your intent.  If none satisfy, adjust the prompt by
removing nonessential tags or moving exclusions earlier【714812518803694†L8-L28】.

### 3.4 Stems Export & Partial Regeneration【714812518803694†L8-L28】

Export stems—drums, bass, guitars/synths, vocals and FX—and balance them.  If a specific section is weak (e.g.,
the chorus lacks impact or the bass is boomy), regenerate only that section using the same prompt and seeds.
Repeat until the arrangement and mix feel balanced.

### 3.5 Add Vocals, Instrumentals & Inspire

Use Suno’s **Add Vocals** and **Add Instrumentals** features to overlay new melody or instrumentation layers onto an
existing track.  Use **Inspire** to generate variations of a take based on your favourite seed.  These tools allow
you to develop a song iteratively without starting over.

### 3.6 Mix & Master【714812518803694†L8-L28】

After stems are balanced, apply quick mix fixes:

- **Low‑end management:** High‑pass non‑bass instruments at 80–120 Hz to reduce mud; cut 200–350 Hz to prevent
  congestion; add air at 8–10 kHz for clarity.
- **Dynamics & loudness:** Use glue compression on the mix bus and aim for an integrated loudness of −14 to −9 LUFS
  with peaks under −1.0 dBTP.
- **Final polish:** Resist over‑processing; V5’s raw output is already clean.  Mastering tweaks should enhance, not
  transform, the mix.

### 3.7 Iterate & Finalise

Return to your pre‑flight checklist, adjust your prompt if necessary, and repeat generation.  Archive your prompt,
lyrics and settings for reproducibility.  Use the troubleshooting framework (see `10_30_Troubleshooting_Framework.md`)
to diagnose common issues and apply targeted fixes.

## 4. Part III: Genre Modules (Overview)

While the core workflow is consistent across genres, each style has its own conventions:

- **Hip‑Hop:** Emphasise flow, cadence and narrative; focus on rhythmic variation and lyric punchlines.
- **EDM:** Build energy towards the drop; experiment with build‑ups and breakdowns; high‑energy dynamic shifts.
- **Metal:** Craft compelling riffs; balance intensity and melody; incorporate syncopated rhythms and breakdowns.
- **Jazz:** Focus on harmonic sophistication and improvisational form; allow space for solos and chord extensions.
- **Ambient:** Prioritise texture and atmosphere; use evolving soundscapes and minimal rhythmic elements.

Apply the same three‑layer prompt framework and stems workflow to each genre.  Adjust instrumentation, tempo and
production feel to suit the style.

## 5. Part IV: Practical Exercises & Case Studies

To build your craft, engage with exercises such as:

- **Prompt engineering drills:** Write five prompts with different style/mood combinations; observe how small
  changes affect the output.
- **Energy curve challenges:** Compose a song where each chorus escalates the hype and tension while the verses
  reset and introduce new details.
- **Genre emulation practice:** Use the style‑emulation guide to recreate the feel of a favourite song without
  naming the artist【757099851912435†L2-L26】.
- **Case study deconstruction:** Analyze the energy curve and arrangement of classics like “Bohemian Rhapsody” or
  “Smells Like Teen Spirit” and map them to the Addiction Formula and PRA Method.

## 6. v4.5 → V5 Changes

- **Workflow simplification:** V5 eliminates the need for exhaustive chronological prompts; concise directives suffice【333682324514163†L29-L33】.
- **Stems & partial regeneration:** V5 supports stems export and partial regeneration; v4.5 required entire rerolls【714812518803694†L8-L28】.
- **Reliable exclusions:** Use `EXCLUDE:` to control instrumentation; avoid long lists of negatives【333682324514163†L34-L37】.
- **Mixing guidance built in:** V5’s default mix quality reduces the reliance on “mastering hacks,” though targeted EQ
  fixes remain useful【714812518803694†L8-L28】.
- **New pitfalls:** Over‑scripting, metatag overload and unrealistic tempo instructions degrade output【333682324514163†L52-L61】【333682324514163†L63-L65】.

## 7. Example Workflow

**Example:** *“Lo‑fi hip‑hop, melancholic, male baritone, piano and vinyl crackle, no drums, 2:30, lyrics about rainy nights in the city.”*

1. **Define intent:** Style and mood specified; vocal persona and instrumentation noted; `no drums` sets the exclusion; length is given.
2. **Craft prompt:** “Lo‑fi hip‑hop, melancholic, male baritone, piano and vinyl crackle, no drums, 2:30, lyrics about rainy nights in the city.”
3. **Generate:** Run and select the take with the smoothest groove and clear bass.
4. **Stems:** Export drums (silence), bass, piano, vocals and FX.  If the bass overwhelms the mix, high‑pass other
   instruments at 90 Hz and cut 250 Hz.  If the piano feels too sparse, add a second take using **Add Instrumental**.
5. **Iterate:** Regenerate the chorus if it lacks emotional lift; adjust the prompt to add one energy cue such as
   “[Chorus: warm, uplifting].”
6. **Finalize:** Mix stems, apply gentle compression and limiting, and export the final track.  Archive the prompt and
   mixing notes for future reference.

## 8. First‑Run Checklist

- [ ] Read `10_10_Core_Principles.md` to understand the underlying mindsets and frameworks.
- [ ] Perform the pre‑flight intent audit and document your prompt and lyrics.
- [ ] Compose a concise three‑layer prompt with at most two exclusions.
- [ ] Generate multiple takes; select the best and export stems.
- [ ] Apply quick mixing fixes and partial regeneration as needed.
- [ ] Iterate until satisfied; archive your work for reproducibility.
- [ ] Use the troubleshooting framework for targeted problem solving.
