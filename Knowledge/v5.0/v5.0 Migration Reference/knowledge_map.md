# Suno v5 Knowledge Base: Core Principles

This document outlines the foundational principles for creating high-quality music with Suno v5. It serves as the strategic "why" behind the tactical "how" detailed in other guides.

> **Note:** This guide is based on the canonical facts found in the `v5.0 Migration Reference/Latest Knowledge` directory.

---

### Principle 1: Intentionality Over Iteration

**v5 rewards clear, concise, and direct instructions.** While random exploration has its place, the most consistent path to quality is starting with a strong, well-defined creative vision.

-   **DO:** Spend time defining your desired genre, mood, instrumentation, and vocal style *before* generating.
-   **DON'T:** Use vague or contradictory terms. "Chill hype track" is less effective than "Lofi hip hop with an upbeat, confident feel."

### Principle 2: The Prompt is the Instrument

In v5, the style prompt is your primary interface for musical control. Treat it with the same care as a musician treats their instrument.

-   **Concise Language:** v5 understands natural language well. Overly complex or "narrative" prompts from v4.5 are no longer necessary. Be direct.
-   **Key Elements First:** Place the most important descriptors (e.g., genre, core feel) at the beginning of the prompt.

> **v4.5 → v5 Change:** The long, narrative, and chronologically ordered prompts that were effective in v4.5 are less optimal for v5. v5 favors brevity and directness.

### Principle 3: Control Through Exclusion

One of v5's most powerful features is the ability to specify what you *don't* want. Use negative constraints to refine your output and avoid common issues.

-   **`EXCLUDE:` Syntax:** Use the `EXCLUDE: [term]` metatag to remove unwanted elements. This is highly effective for things like "boomy bass," "muddy mix," or specific instruments.
-   **Natural Language Negation:** Simple phrases like "no electric guitar" or "without drums" are also effective.

**Example:**
```
// Style Prompt
Acoustic folk, singer-songwriter, gentle female vocals, clear acoustic guitar, sparse piano. EXCLUDE: boomy bass, muddy mix
```

### Principle 4: Structure with Metatags

Use bracketed metatags `[tag]` in the lyrics to define song structure and control performance. This is the most reliable way to guide the AI's arrangement.

-   **Standard Tags:** `[Verse]`, `[Chorus]`, `[Bridge]`, `[Intro]`, `[Outro]`, `[Guitar Solo]`
-   **Performance Tags:** `[whispered]`, `[shouted]`, `[upbeat]`

### Principle 5: The Human is the Editor

AI is a powerful collaborator, not a replacement for your artistic judgment. Use v5's editing tools to assemble the best parts of multiple generations into a cohesive whole.

-   **Stem Separation:** Download stems (vocals, bass, drums, other) to fix mix issues or replace parts in a DAW.
-   **Partial Regeneration:** Use the editor to regenerate specific lines or sections that didn't land correctly.
-   **The "Best Of" Method:** Generate several clips. Take the best chorus from one, the best verse from another, and assemble them.

---

### First-Run Checklist for v5

1.  [ ] **Start Simple:** Create a song with a clear, two-genre prompt (e.g., "Indie Pop, Synthwave").
2.  [ ] **Add Structure:** Use `[Verse]` and `[Chorus]` tags in your lyrics.
3.  [ ] **Use a Negative:** Add `EXCLUDE: muddy mix` to your style prompt.
4.  [ ] **Review Stems:** Download the stems for your generation and listen to the `bass` and `vocals` tracks individually.
5.  [ ] **Iterate on a Section:** Identify one line you dislike and use the editor to regenerate only that part.

## v5.0 Inventory Snapshot
| v5.0 Document | Initial Classification |
| ------------- | ---------------------- |
| 01_Core_Knowledge/00_10_Master_Index.md | model-specific |
| 03_Expert_Songwriter_Books/HowtoWriteOneSong.md | model-agnostic |
| 03_Expert_Songwriter_Books/Mastering Melody Writing꞉ A Songwriter’s Guide to Hookier Songs with Pattern, Repetition, and Arc [Transcript].md | model-agnostic |
| 03_Expert_Songwriter_Books/Song Building, Mastering Lyric Writing.md | model-agnostic |
| 03_Expert_Songwriter_Books/Song-Maps-A-New-System-to-Write-Your-Best-Lyrics.md | model-agnostic |
| 05_Misc/Apps_Tools_Projects/Song Blueprint Generator.md | model-agnostic |
