# Cliches and Overused Words Master Database:

in AI Lyrics 

---

**Sources Consolidated:**

- ✅ **clicheguarddb.csv** (220 entries - automated corpus detection)
- ✅ **cliches.json** (21 entries - AI-specific overuse)
- ✅ **banned-words-phrases-cliches.md** (21 entries - duplicate JSON)

### **Result:**

- **240 unique entries** (21 duplicates removed)
- Sorted by frequency (highest offenders first)
- Merged fields from all sources (keeping highest frequency scores)

## 🔴 **TOP 10 WORST OFFENDERS**

1. **"find way"** - 10,854 uses (CRITICAL)
2. **"feel like"** - 8,721 uses (CRITICAL)
3. **"let go"** - 8,242 uses (CRITICAL)
4. **"every step"** - 6,021 uses (CRITICAL)
5. **"can't see"** - 5,315 uses (CRITICAL)
6. **"hold tight"** - 4,089 uses (CRITICAL)
7. **"every moment"** - 3,966 uses (CRITICAL)
8. **"fade away"** - 3,711 uses (CRITICAL)
9. **"stand tall"** - 3,676 uses (CRITICAL)
10. **"every day"** - 3,519 uses (CRITICAL)

## 🤖 **AI SIGNATURE WORDS (Auto-Reject)**

These 17 words instantly flag AI authorship:

- broken, shadow/shadows, whisper/whispers, echo/echoes
- shatter/shattered, fade/fading, spark/ignite
- unsaid, unseen, fractured, static
- carve/carved, chains, paints/painting, seam/seams
- forgot/forgotten, ignite/ignited

## 📋 **DATABASE STRUCTURE**

Each entry includes:

```json
{
  "root_word_phrase": "the problematic word/phrase",
  "variants": "different forms (plural, tense, etc.)",
  "often_combined_with": "common problematic pairings",
  "severity": "CRITICAL | EXTREME | HIGH | MEDIUM",
  "context_why_avoid": "explanation of why it's problematic",
  "synonyms": "alternative words to use instead",
  "synonyms_that_rhyme": "rhyming alternatives",
  "frequency_score": "number of occurrences in corpus",
  "sources": ["which files contributed this entry"]
}

```

## 🎯 **USAGE INSTRUCTIONS**

### **For Research Agents:**

- ✅ Check ALL generated content against this database
- ✅ Auto-reject CRITICAL/EXTREME entries
- ✅ Flag HIGH entries with warnings

### **For Rhyme Dictionary:**

- ✅ Flag rhyme pairs containing these words
- ✅ Display severity level in suggestions
- ✅ Offer synonyms_that_rhyme as alternatives

### **For Furniture Database:**

- ✅ Run SCREEN 9 (frequency check) against this
- ✅ Reject furniture containing CRITICAL/EXTREME words
- ✅ Example: "broken glass" contains "broken" (EXTREME) → Reject

### **For Songwriters:**

- ✅ Avoid all CRITICAL/EXTREME phrases
- ✅ Use synonym suggestions for alternatives
- ✅ When in doubt, check frequency_score

## 💾 **DOWNLOAD & INTEGRATION**

The artifact contains the complete database structure with:

- **Metadata** (severity definitions, usage instructions)
- **Statistics** (severity distribution, top offenders)
- **Sample entries** (20 most critical examples shown)
- **Implementation notes** (API pseudo-code, integration examples)