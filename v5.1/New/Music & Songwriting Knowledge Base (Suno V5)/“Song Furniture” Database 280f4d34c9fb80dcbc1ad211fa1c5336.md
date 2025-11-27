# “Song Furniture” Database

The concept of **Song Furniture** is a meticulous and foundational principle within lyrical craft, serving as a powerful analogy for implementing the core directive to "Show, Don't Tell" in songwriting.

# DEEP RESEARCH PROMPT:

## YOUR MISSION

You are a lyrical detail specialist tasked with cataloging 1000+ "song furniture" elements—the specific, concrete, sensory details that transform generic lyrics into vivid storytelling. Your goal is to create a comprehensive resource that helps songwriters implement "show, don't tell" principles in AI-generated lyrics.

## WHAT YOU NEED TO DELIVER

A JSON database where each entry contains:

- The specific furniture element (concrete detail)
- Category and subcategory classification
- Sensory type(s) engaged (visual, auditory, tactile, olfactory, gustatory)
- Specificity level rating (1-5 scale)
- Emotional associations with intensity ratings
- Genre associations with frequency
- Section suitability (verse/chorus/pre-chorus/bridge)
- Show-don't-tell effectiveness rating (1-10)
- Famous song examples with lyric context
- Usage guidance (dos and don'ts)
- Typical pairings with other furniture
- Abstract concepts this detail replaces
- Power word potential
- Rhyme compatibility
- Era associations and cultural context
- Suno AI prompting integration

## WHERE TO FIND YOUR DATA

### Primary Sources

1. **Hit Song Lyrics** - Analyze 1,000+ songs across genres
2. **Genre-Specific Canons:**
    - Country: 200 classic/modern songs
    - Folk: 100 Americana songs
    - Rock: 100 narrative rock songs
    - Hip-Hop: 100 storytelling tracks
    - Pop: 100 detail-rich songs
3. **Creative Writing Resources** - Sensory detail lists
4. **Cultural Databases** - Regional details, touchstones

### Research Process

For each furniture element you identify:

**STEP 1: EXTRACT FROM SONGS**

- Read lyrics of hit songs
- Identify every specific, concrete detail
- Note: song, artist, year, section
- Quote the lyric context
- Describe what effect it creates

**STEP 2: CLASSIFY & CATEGORIZE**
Assign to primary category:

1. LOCATIONS (cities, venues, natural places, buildings)
2. PEOPLE & NAMES (names, nicknames, occupations, relationships)
3. TIME MARKERS (times of day, dates, seasons, historical refs)
4. COLORS & VISUALS (specific colors, light, textures)
5. WEATHER & ATMOSPHERE (conditions, phenomena, moods)
6. OBJECTS - PERSONAL (clothing, accessories, tech, keepsakes)
7. OBJECTS - HOUSEHOLD (furniture, kitchenware, décor, appliances)
8. OBJECTS - TRANSPORTATION (vehicles, parts, infrastructure)
9. BODY PARTS & PHYSICAL (body parts, physical actions)
10. FOOD & DRINK (meals, drinks, specific foods)
11. NATURE & OUTDOORS (flora, fauna, landscapes)
12. SOUNDS & MUSIC (natural sounds, human-made, music refs)
13. BRANDS & CULTURAL (brands, cultural touchstones)

**STEP 3: RATE SPECIFICITY (1-5) & SCREEN FOR SINGABILITY**

- 1: Generic (red car)
- 2: Slightly specific (old red car)
- 3: Specific (beat-up red pickup truck) ✅ IDEAL RANGE
- 4: Very specific ('67 red Chevy pickup) ✅ IDEAL RANGE
- 5: Extremely specific ('67 red Chevy C10 with rust on tailgate) ⚠️ CHECK SYLLABLES

**CRITICAL SINGABILITY FILTERS:**
Apply these checks to REJECT or FLAG furniture that creates lyrical problems:

**A. SYLLABLE COUNT CHECK**

- ✅ IDEAL: 1-4 syllables per furniture element
- ⚠️ CAUTION: 5-6 syllables (only if highly euphonious)
- ❌ REJECT: 7+ syllables (too cumbersome for singing)
- Examples:
    - ✅ "pickup truck" (3 syllables)
    - ✅ "neon sign" (3 syllables)
    - ⚠️ "refrigerator" (5 syllables - acceptable if needed)
    - ❌ "air conditioning unit" (7 syllables - too long)

**B. PHONETIC COMPLEXITY CHECK**
Reject furniture with difficult consonant clusters or cacophonous sounds:

- ❌ Multiple plosives in sequence: /kt/, /pt/, /bd/
    - Bad: "cracked plastic dashboard" (too many hard stops)
    - Good: "worn leather dashboard" (smoother)
- ❌ Harsh sibilant clusters: /sl-/, /skr-/, /spr-/
    - Bad: "slithering snake" (unpleasant /sl-/)
    - Good: "coiled snake" (smoother)
- ❌ Difficult consonant combinations that interrupt flow
    - Bad: "clenched fists" (/ncht/ cluster is awkward)
    - Good: "tight fists" (simpler)

**C. CLICHÉ & OVERUSE CHECK**
Flag furniture that appears too frequently in AI-generated lyrics:

- ❌ OVERUSED IN AI: "weathered hands," "faded photograph," "dusty road," "broken dreams"
- ✅ FRESH ALTERNATIVES: "calloused palms," "creased photo," "gravel path," "shattered plans"
- Check against hit song database: If furniture appears in 20+ songs, mark as "HIGH FREQUENCY - USE WITH CAUTION"

**D. PRETENTIOUS/ARCHAIC LANGUAGE CHECK**
Reject furniture that sounds unnatural or overly literary:

- ❌ "crimson automobile" (pretentious) → ✅ "red car"
- ❌ "dwelling place" (archaic) → ✅ "home" or "house"
- ❌ "celestial orb" (pretentious) → ✅ "moon" or "sun"
- ❌ "precipitation" (clinical) → ✅ "rain"

**E. NATURAL SPEECH PATTERN CHECK**
Would a real person say this in conversation?

- ✅ "beat-up truck" (conversational)
- ❌ "dilapidated vehicular conveyance" (unnatural)
- ✅ "cold beer" (natural)
- ❌ "refrigerated malt beverage" (clinical)

**STEP 4: IDENTIFY SENSORY TYPES**
Which senses does this engage?

- Visual (most common)
- Auditory (sounds)
- Tactile (touch/texture)
- Olfactory (smell)
- Gustatory (taste)
- Multi-sensory (best!)

**STEP 5: MAP EMOTIONAL ASSOCIATIONS**

- What emotions does this detail evoke?
- Intensity rating (1-10)
- Context-dependent variations
- Example: "rusty swing set"
    - Nostalgia (8) - childhood memories
    - Comfort (7) - home and safety
    - Sadness (5) - abandoned or broken

**STEP 6: ASSESS SHOW-DON'T-TELL POWER**

- Rating (1-10): How effectively does it show vs tell?
- What abstract concepts does it replace?
    - Abstract: "childhood" → Concrete: "rusty swing set"
    - Abstract: "lonely" → Concrete: "neon bar sign flickering"
    - Abstract: "home" → Concrete: "screen door slamming"

**STEP 7: DETERMINE SECTION SUITABILITY**

- Verse: Usually very high (narrative detail)
- Chorus: Usually low (too specific for universal themes)
- Pre-Chorus: Variable (transitional imagery)
- Bridge: Medium (contrast or callback)

**STEP 8: GENRE & CULTURAL CONTEXT**

- Which genres use this frequently?
- Regional specificity (American South, urban, etc.)
- Socioeconomic associations
- Universal recognition level
- Era associations (timeless vs. dated)

**STEP 9: USAGE GUIDANCEDos:**

- Use in verses to establish setting
- Pair with other sensory details
- Let detail imply emotion
- Choose details that resonate with audience

**Don'ts:**

- Don't use in chorus (too specific)
- Avoid mixing with abstractions
- Don't over-explain
- Avoid anachronisms unless intentional

**STEP 10: FIND PAIRINGS**
What other furniture works well with this?

- "Rusty swing set" + "gravel driveway" = complete scene
- "Neon bar sign" + "whiskey glass" + "barstool" = dive bar

**STEP 11: VALIDATE**

- Category accurately assigned
- Sensory types identified
- Specificity rated and justified
- Emotional associations researched (not assumed)
- At least 2 famous examples OR cultural validation
- Section suitability logical
- Related furniture linked (min 2)
- Usage guidance actionable

## PRIORITIZATION STRATEGY

### START HERE (Tier 1 - 400 elements)

**Essential Details (200):**

- Top 50 most common furniture in hit songs
- Genre-defining details (20 per major genre = 100)
- Universal sensory details (50):
    - Rain, sunset, moonlight
    - Coffee, whiskey, cigarettes
    - Highway, river, mountain
    - Etc.

**High-Impact Specifics (200):**

- Locations that resonate broadly (50)
    - Nashville, Brooklyn, small town, dive bar
- Objects with strong emotion (50)
    - Wedding ring, photograph, old guitar
- Time markers that set era/mood (40)
    - Friday night, 3 AM, summer, '65
- Body language/physical (30)
    - Tear-stained face, calloused hands
- Food/drink that evokes culture (30)
    - Black coffee, whiskey neat, mama's cooking

### THEN BUILD (Tier 2 - 400 elements)

- Genre-specific vocabulary (50 per genre = 300)
- Regional/cultural details (50)
- Era-specific references (50)

### FINALLY ADD (Tier 3 - 200+ elements)

- Niche but effective details
- Contemporary/modern references
- International/global details
- Experimental/unusual details

## QUALITY STANDARDS

Every entry MUST pass these checks:

- ✅ Category accurately assigned
- ✅ Sensory type(s) identified
- ✅ Specificity rated and justified
- ✅ Emotional associations researched
- ✅ At least 2 famous examples OR cultural validation
- ✅ Section suitability ratings logical
- ✅ Related furniture linked (minimum 2)
- ✅ Usage guidance specific and actionable

### MANDATORY SINGABILITY FILTERS (MUST PASS ALL)

- ✅ **Syllable count: 1-6 syllables maximum** (reject 7+)
- ✅ **No harsh consonant clusters** (no /kt/, /pt/, /bd/, /sl-/, /skr-/)
- ✅ **Not AI-cliché** (check against overused AI patterns)
- ✅ **Natural speech pattern** (conversational, not pretentious)
- ✅ **Euphonious or neutral phonetics** (avoid cacophony unless intentional)

### REJECTION CRITERIA (AUTO-REJECT IF ANY APPLY)

❌ **7+ syllables** - "air conditioning unit" (too long)
❌ **Pretentious language** - "crimson automobile" (use "red car")
❌ **Clinical/technical terms** - "precipitation" (use "rain")
❌ **Archaic phrasing** - "dwelling place" (use "home")
❌ **Difficult consonant clusters** - "clenched fists" (use "tight fists")
❌ **AI-overused phrases** - "weathered hands," "faded photograph," "dusty road"
❌ **Unnatural speech** - "dilapidated vehicular conveyance"

## EXAMPLE OF EXCELLENCE

```json
{
  "furniture_id": "furniture_001",
  "element": "neon bar sign flickering",
  "category": "OBJECTS - COMMERCIAL",
  "subcategory": "signage",
  "sensory_type": ["visual", "auditory"],
  "specificity_level": {"rating": 4, "description": "Very specific - vivid with implied sound"},
  "singability_metrics": {
    "syllable_count": 5,
    "phonetic_complexity": "low",
    "consonant_clusters": ["none_problematic"],
    "euphony_rating": 8,
    "natural_speech": true,
    "ai_cliche_status": "SAFE - uncommon in AI lyrics"
  },
  "emotional_associations": [
    {"emotion": "loneliness", "intensity": 8, "context": "late night solitude"},
    {"emotion": "melancholy", "intensity": 7, "context": "heartbreak setting"}
  ],
  "show_dont_tell_effectiveness": {
    "rating": 9,
    "description": "Immediately evokes dive bar atmosphere without stating it"
  },
  "abstract_concepts_replaced": [
    {"abstract": "lonely", "concrete": "neon bar sign flickering"},
    {"abstract": "dive bar", "concrete": "neon sign flickering"},
    {"abstract": "late at night", "concrete": "neon sign flickering"}
  ],
  "famous_examples": [
    {"song": "Whiskey River", "artist": "Willie Nelson", "year": 1973}
  ]
}

```

## EXAMPLE OF REJECTION

```json
{
  "furniture_id": "REJECTED_001",
  "element": "dilapidated vehicular conveyance",
  "rejection_reason": "MULTIPLE FAILURES",
  "failures": [
    "Pretentious language (use 'beat-up car' or 'old truck')",
    "Unnatural speech pattern (no one talks like this)",
    "9 syllables (exceeds 6-syllable maximum)",
    "Clinical/technical terminology"
  ],
  "better_alternatives": ["beat-up truck", "old car", "rusty Chevy"]
}

```

## SUCCESS METRICS

- Minimum 1,000 unique furniture elements
- All 13 categories populated with target counts
- 100% have sensory type(s) identified
- 80%+ have famous song examples
- All have emotional associations researched
- Section suitability rated for 100%
- Show-don't-tell effectiveness rated for 100%
- Related furniture linked (min 2 per entry)
- Usage guidance for 100%
- Scene kits created (min 20 common settings)
- **100% pass singability filters (syllables, phonetics, natural speech)**
- **AI-cliché status marked for all entries**

## SPECIAL INSTRUCTIONS

**Specificity is Key:**
Always prefer MORE specific over less:

- ❌ "car" → ✅ "pickup truck" → ✅ "'67 Chevy"
- ❌ "drink" → ✅ "whiskey" → ✅ "whiskey neat"
- ❌ "time" → ✅ "night" → ✅ "3 AM"

**Show, Don't Tell Focus:**
Every entry must answer: "What abstract concept does this concrete detail replace?"

- This is the core value of the database
- Helps writers avoid generic statements
- Teaches "showing" through examples

**Scene Kits:**
Group related furniture into complete settings:

- **Dive Bar Scene:** neon sign, barstool, whiskey glass, jukebox, cigarette smoke
- **Small Town:** gravel road, pickup truck, church steeple, Friday night lights
- **Heartbreak Apartment:** unmade bed, empty wine bottle, rain on window, 3 AM

**Cultural Sensitivity:**

- Note regional specificity (American South, urban Northeast, etc.)
- Flag dated references (rotary phone, cassette tape)
- Indicate universal recognition level
- Respect cultural origins

**AI-Cliché Detection Protocol:REFERENCE**: `/deep-research/musical-resources/CLICHE-GUARD-DATABASE.md`

This is CRITICAL to prevent the database from perpetuating AI-generated clichés:

1. **Use ClichéGuard Database as Single Source of Truth**
    - Check EVERY furniture element against Category 7 (AI-Specific Overused Phrases, C061-C075)
    - Check against Category 2 (Overused Imagery, C011-C020)
    - Check against Category 13 (Abstract Concepts, C136-C145)
    - Reference database IDs in your metadata
2. **AI-Cliché Examples from Database:**
    - C061: "weathered hands" = EXTREME (AI's go-to for "working person")
    - C062: "calloused hands" = EXTREME (overused in country/folk AI)
    - C063: "faded photograph" = EXTREME (AI's default "memory" image)
    - C065: "dusty road" = EXTREME (AI's default "journey" image)
    - C067: "broken dreams" = EXTREME (#1 AI emotional cliché)
3. **For each furniture element, check:**
    - Is it in the ClichéGuard Database? (Note ID and severity)
    - If EXTREME or HIGH severity → REJECT or provide alternatives
    - If MEDIUM severity → FLAG for user awareness
    - If not in database → Mark as SAFE
4. **Use database alternatives (Column 5):**
    - C061: "weathered hands" → "paint-stained fingers," "rope-burned palms," "ink-stained knuckles"
    - C063: "faded photograph" → "creased photo," "dog-eared snapshot," "water-stained picture"
    - C065: "dusty road" → "gravel path," "cracked asphalt," "mud-rutted lane"

**Singability Over Specificity:**
When there's a trade-off between extreme specificity and singability, ALWAYS choose singability:

- ❌ "'67 red Chevy C10 with rust on the tailgate" (11 syllables, too long)
- ✅ "'67 Chevy pickup" (5 syllables, singable)
- ✅ "rusty red Chevy" (5 syllables, singable)

Focus on furniture that is both evocative AND practical. The goal is to give songwriters a palette of vivid details they can immediately use to replace generic abstractions—details that are SINGABLE, NATURAL, and FRESH (not AI-clichéd).

As an expert in music production and technical writing, I can detail this concept, its purpose, and the specific elements—the metaphorical "database"—that constitute this technique, drawing directly from the sources.

### Definition and Core Principle

Song Furniture refers to the tangible, evocative, and specific sensory details that infuse lyrics with "texture and spice," effectively furnishing the narrative environment of the song.

- **Show, Don't Tell:** The principle mandates that songwriters convey emotions, actions, or events through observable details rather than abstract statements. Instead of *telling* the audience what a character feels (e.g., "I miss you"), the writer *shows* them through specific actions or objects (e.g., "I still make coffee for two. I’m not used to you not being around").
- **The Analogy:** Just as an empty room feels bare, a vague song lacks the immersive environment necessary for a listener to connect. Song furniture fills this "room," allowing listeners to engage their imagination and draw their own conclusions.

### The Song Furniture Database: Essential Elements

To effectively "show" rather than "tell," songwriters are encouraged to shift from broad concepts to concrete sensory details, imagining the song as a visual experience. The sources identify a comprehensive list of elements that can be integrated into the lyric, forming the "database" of descriptive details:

| Category | Description and Function | Examples |
| --- | --- | --- |
| **Specific Place & Time** | Grounds the song in reality and creates atmosphere. | Locations (cities, states, establishments), Time (dates, days, seasons, parts of the day), Weather. |
| **Characters & People** | Enhances specificity and characterization. | Personal or animal names, Dialogue, Age. |
| **Sensory Details** | Appeals to the five senses, bringing moments to life (sight, smell, taste, touch, sound, and movement). | Colors, Objects, Body Parts, Noun Modifiers, Brand Names. |
| **Action & Intensity** | Uses specific verbs and phrases to make the language dynamic and engaging. | Specific Actions/Descriptive Verbs (e.g., "tangled" instead of "involved"), Phrases Turned into Nouns, Numbers. |

Crucially, the effectiveness of this database relies on balance; too much furniture can clutter the song, while too little leaves it sparse and undeveloped.

### Strategic Application in Songwriting

The strategic use of Song Furniture is intrinsically linked to a song’s structure and its energy curve, which governs the listener's experience.

### 1. Energy and Structure (Hype and Tension)

The required density of specific detail varies by section:

- **Verses (Low Hype/Anticipation):** Verses are the primary stage for setting the scene, introducing characters, and establishing context. To draw the listener in with a conversational tone, the lyrics must aim for **specificity** and detailed descriptions (low hype).
- **Choruses (High Hype/Gratification):** Choruses function as the "big picture" moments, offering the main theme or universal message. They aim for **generality** and are typically broader in scope. However, the specific details (furniture) established in the verses "recolor" the recurring chorus, imbuing it with new interpretation and deeper emotional impact each time it appears.
- **Building Tension:** Lyrical details can generate **contentual tension**—a form of anticipation created through storytelling or using "cliffhangers" (lines that abruptly cut off an event) to force the listener to follow the plot progression.

### 2. Enhancing Lyrical Impact

Placing these strong, specific details—especially **power words**—in melodic "hotspots" (moments that naturally draw listener attention, like the end of a phrase or a high note) maximizes their impact. Furthermore, Word Painting directly enhances the "showing" aspect by having the music and melody *mirror* the action or emotion described by the lyrical details (e.g., a melody dipping low on the word "low").

### Relevance to AI Music Generation

For music producers and AI developers leveraging tools like Suno AI, mastering the use of Song Furniture is critically important because AI-generated lyrics often default to vagueness, predictable phrasing, and clichés.

1. **Humanization:** Human intervention is essential to refine AI output, ensuring the lyrics convey genuine emotional depth and an authentic "voice".
2. **Prompt Engineering:** To guide the AI away from generic clichés, prompts must explicitly instruct the model to "include sensory details or specific scenes" and "strive for fresh metaphors and unique expressions".
3. **Contextual Cues:** When inputting custom lyrics in Suno, ensuring the poetic structure uses sufficient detail and specific imagery helps the AI interpret the emotional direction correctly and enhances the overall musical result.