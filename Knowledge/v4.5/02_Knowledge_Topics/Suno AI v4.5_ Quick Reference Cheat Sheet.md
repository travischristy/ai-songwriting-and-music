# Suno AI v4.5: Quick Reference Cheat Sheet

### General Philosophy for v4.5 Prompting

**Embrace Narrative and Linear Prompts:** Suno v4.5 excels when provided with detailed, conversational, and structurally linear instructions. Instead of merely listing keywords, describe the song's intended evolution chronologically, akin to "temporal programming" its dynamic changes.

### "Style of Music" Prompting for v4.5

This prompt is crucial for defining the song's overall sonic architecture.

**A. Key Components to Specify:**

- **Genre and Style:** Be specific (e.g., "indie folk," "synthwave," "trap metal") or broad (e.g., "rock," "jazz," "hip-hop").
- **Mood and Emotion:** Describe the feeling or energy (e.g., "melancholic," "uplifting," "cinematic," "intense").
- **Instrumentation and Production Style:** Mention key instruments, their desired sound qualities, and overall production elements (e.g., "strong bassline," "smooth saxophone," "warm electric guitar," "gated reverb snares," "shimmering Juno pads," "clean, professional mastering").
- **Vocal Preferences:** Define vocal tone, singer type, and structure (e.g., "female singer with soft, airy vocals," "very soulfully deep voice with a gritty and weathered dub reggae tone").

**B. Structuring Your Prompt for v4.5:**

- **Narrative/Linear Progression:** Describe the song's intended evolution chronologically. For example: "Starts with melancholic piano, gradually introduces strings in verse, explodes into a soaring orchestral chorus, bridge features a quiet, reflective acoustic guitar solo before building back up". This guides the AI through dynamic changes and builds a narrative arc directly within the music.
- **Layered Descriptors:** Blend multiple stylistic elements (genre, mood, texture, rhythm) in a single prompt for richer output. For example: "Create an organic house track with live instrumentation—warm acoustic guitar licks, jazzy Rhodes chords, and a swinging percussion groove. Keep the mood uplifting but intimate, with a loose, improvisational feel".
- **Punctuation Rules are Critical for v4.5:**
    - Use **periods** at the end of each distinct categorized instruction set (e.g., after Genre, Style, Mood sections) to help Suno distinguish them. This is essential for v4.5.
    - **Avoid commas** to separate these main category blocks in v4.5 style prompts, as this can lead to misinterpretation. Instead, use "and" or "with" to link related descriptors within a continuous thought.
- **Character Limit:** While older models had a 120-character limit, v4.5 has an increased limit, often noted as up to 1000 characters, allowing for more detailed narrative prompts.

**C. What to Avoid in Style Prompts:**

- **Direct Artist/Band Names:** **DO NOT** use specific artist, band, or song titles (e.g., "Billie Eilish style," "Smells Like Teen Spirit by Nirvana"). This is due to copyright concerns, unpredictable and inconsistent results, potential content filter issues, and the AI potentially singing the artist's name. Instead, describe the desired style descriptively (e.g., "dark, minimalist electro-pop with whispery female vocals").
- **Negative Instructions:** Avoid telling Suno what *not* to include (e.g., "no drums," "without guitar," [no synth]). Suno models generally ignore negation instructions. Phrase everything in positive terms, emphasizing the instruments or elements you *do* want.
- **Overly Vague or Overly Complex Prompts:** A single word or generic prompt will likely produce bland results. Conversely, a paragraph of convoluted or conflicting adjectives can confuse the model. Aim for clear, concise, yet descriptive instructions.

### "Custom Lyrics" Prompting for v4.5

Utilizing the "Custom Lyrics" field with v4.5's enhanced capabilities provides paramount creative control over your song's narrative and vocal delivery.

**A. Metatags for Structure and Musical Cues:**

- **Structural Tags:** Define song sections and guide the AI's song layout.
    - Examples: `[Verse]`, `[Chorus]`, `[Bridge]`, `[Intro]`, `[Outro]`, `[Pre-Chorus]`, `[Hook]`, `[Instrumental]`, `[Post-Chorus]`.
- **Vocal Tags:** Specify voice type, delivery, or effects.
    - Examples: `[Male Vocal]`, `[Female Vocal]`, `[Whispers]`, `[Shout]`, `[Rapped Verse]`, `[Harmonized Chorus]`, `[Spoken Word]`, `[Soulful Vocals]`, `[Gospel Choir]`.
- **Instrumental Tags:** Cue specific instruments or instrumental sections at precise points.
    - Examples: `[Guitar Solo]`, `[Piano Break]`, `[Synth Lead]`, `[Bass Drops]`, `[Instrumental Solo]`.
- **Dynamic and Emphasis Tags:** Influence energy and intensity of a section.
    - Examples: `[Crescendo]`, `[Building Intensity]`, `[Soft Outro]`, `[Catchy Hook]`, `[Emotional Swell]`, `[Big Finish]`.

**B. Formatting Cues for Nuance and Expressiveness (v4.5 Enhancements):**

- **ALL CAPS:** Writing words or lines in ALL CAPS cues the AI to deliver them with "greater volume, intensity, or passion". This is effective for emphasizing emotional peaks.
- **Asterisks (`*sound effect*`):** Surrounding a word or phrase with asterisks can prompt the AI to incorporate specific sound effects or ambiance (e.g., `*rain*`, `*gunshots*`, `*thunder*`, `*crowd cheering*`). Use sparingly for obvious sounds.
- **Parentheses (`()`):** Add ad-libs and spontaneous vocalizations for a more conversational flow (e.g., `(ad lib: "Yeah!")`).
- **Punctuation and Line Breaks:** Influence pacing and pauses. A comma creates a "small pause," and ellipses (`...`) create a "longer pause". Adjusting line breaks also impacts rhythmic effect and singability.
- **Contextual Prompting (v4.5 Specific):** Leverage v4.5's "better prompts in the Lyrics box" feature by embedding descriptive parentheticals or bracketed instructions more liberally within the lyric content. This guides "performance nuances line-by-line or section-by-section" (e.g., `(softly, with a hint of longing)` before a line).

**C. Best Practices for Metatags and Lyrical Craft:**

- **Keep Simple and Concise:** Metatags work best with a maximum of three words. Overloading a tag can cause it to be ignored or, worse, sung as part of the lyrics.
- **Be Specific and Descriptive:** Pair a brief style description with a noun indicating the instrument or voice (e.g., `[Syncopated Bass]`).
- **Proper Formatting:** Always enclose metatags in square brackets `[]`.
- **Avoid AI Clichés / Humanization:** AI-generated lyrics often default to generic expressions and clichés.
    - **Prompt for Originality:** Explicitly instruct the AI to "actively avoid common lyrical clichés and predictable phrasing" and to "strive for fresh metaphors and unique expressions".
    - **Inject Personal Voice & Imagery:** Infuse prompts with personal experiences, emotions, a consistent language style (conversational, poetic, narrative), and vivid sensory imagery to combat vagueness (e.g., "melancholic ballad about lost love in a rainy city"). Developing a "word bank" can assist this.

### Technical Considerations and Limitations (v4.5)

Understanding these will help set realistic expectations and adapt your approach.

- **Strengths:**
    - **End-to-end Capability:** Generates composition, arrangement, lyrics, and vocals together.
    - **Mainstream Styles:** Excels at polished choruses and hooks in popular genres.
    - **Lyric Coherence:** Produces more coherent lyrics and better enunciation, adapting well to user-provided lyrics (even non-English, with some quirks).
    - **Genre Mixing:** Capable of creative fusions, though best kept to two genres at a time.
    - **Logical Structure:** Better at maintaining logical song structure, especially with story-driven prompts.
- **Constraints & Biases:**
    - **Randomness (RNG):** Requires multiple generations to achieve desired results.
    - **Misinterpretation/Hallucination:** May misinterpret or partially ignore prompts, or jumble lyrics.
    - **Limited Musical Complexity:** Tends to default to 4/4 time and common Western pop chord progressions; struggles with unusual time signatures or complex jazz chords.
    - **No Fine Control:** Lacks direct control over mixing levels, exact note sequences, or precise melodic/bassline programming.
    - **Pop Tendency:** May lean "pop-ish" even when aiming for other genres.
    - **Unwanted Instruments:** Can occasionally add instruments like synth leads unexpectedly.
    - **Audio Quality Issues:** Some users report "muffled" audio, digital distortion, or volume increases over time, despite v4.5 improvements.