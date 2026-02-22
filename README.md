# Cognitive Influence Rating
### A Games of Arcadia Tool

Paste any text and get an instant manipulation score. 
Cognitive Influence Rating analyses articles, speeches, YouTube transcripts, social media posts, and news items against **20 indicators of psychological manipulation, narrative engineering, and disinformation techniques**.

**Free. Only a Google account needed. Runs entirely in your browser.**

🔗 **[Launch the app](https://gamesofarcadia.github.io/cognitive-influence-rating/)**

---

## How It Works

The tool scores any text against 20 indicators derived from open media literacy research, including the Narrative Credibility Index. 
Each indicator is scored 0–5 by an AI model, producing two outputs:

- **Psyop Score** : total out of 100, with probability range (LOW / MODERATE / HIGH)
- **Influence Signal** : based on peak indicator scores (CLEAN / CAUTION / WARNING)

The tool does not determine truth or falsehood. 
It measures whether the content uses techniques commonly associated with influence operations. 
A high score means the content is structured to persuade rather than inform.

---

## The 20 Indicators

| # | Indicator | Description |
|---|-----------|-------------|
| 1 | Emotional Manipulation | Fear, outrage, or panic used to push a reaction rather than inform |
| 2 | Designated Enemy | A group or person presented as purely evil with no nuance |
| 3 | Saviour Figure | A person or movement presented as the only solution |
| 4 | Tribal Division | Content that divides audiences into irreconcilable camps |
| 5 | False Simplicity | A complex issue reduced to one convenient cause |
| 6 | Pressure to Act | Audience pushed to act immediately with no time to verify |
| 7 | Evidence Vacuum | Key claims made with no data or verifiable sources |
| 8 | Shadow Sources | Information from unnamed or unverifiable sources |
| 9 | Narrative Instability | Story details shift or contradict each other |
| 10 | Symbolic Overload | Heavy use of emotionally charged symbols or imagery |
| 11 | Slogan Engineering | Key phrases repeat like slogans to embed a message |
| 12 | Moral Absolutism | Questioning the narrative gets you labelled an enemy |
| 13 | Hollow Authority | Experts named as proof with no supporting data |
| 14 | Herd Pressure | Viral numbers used in place of actual evidence |
| 15 | Apocalyptic Framing | Catastrophic outcomes presented as certain and imminent |
| 16 | Miracle Promise | The promised outcome is implausibly perfect |
| 17 | Dissent Suppression | Critics called shills or bots instead of being addressed |
| 18 | Suspicious Timing | Story surfaces at a moment that benefits specific interests |
| 19 | Coordinated Amplification | Same message across platforms with no clear source |
| 20 | Sealed Narrative | No alternative perspectives shown, debate discouraged |

---

## Requirements

A free **Google Gemini API key** from [aistudio.google.com](https://aistudio.google.com/apikey). 
No credit card required for the free tier. 
Your key is stored locally in your browser (no data is sent to or stored by Games of Arcadia.)

---

## Score Ranges

| Range | Verdict |
|-------|---------|
| 0–39 | LOW PROBABILITY |
| 40–69 | MODERATE PROBABILITY |
| 70–100 | HIGH PROBABILITY |

*Based on the Narrative Credibility Index.*

> **Note:** The total score is a headline. The indicator breakdown is the story. A 10/100 where one category scores 5 tells you something very different from a 10/100 spread evenly at 0–1.

---

## Models

The tool supports three Gemini models. 
Results may vary between models: different models weigh language patterns differently. 
If a result surprises you, try the other model.

- **Gemini 2.5 Flash** : default, good balance of speed and accuracy
- **Gemini 2.5 Flash Lite** : faster, can be more sensitive to subtle stylistic manipulation
- **Gemini 2.5 Pro** : untested, doesn't seem to accept free tier key

---

## Changelog

### v1.4 — Feb 2026
- Psyop Score verdict now hardcoded by range in JS; no longer subject to AI interpretation
- New **Influence Signal** indicator: CLEAN / CAUTION / WARNING based on peak indicator scores, independent of total score
- Prompt hardened to prevent malformed JSON from breaking analysis
- Conclusion no longer opens with a probability statement; focuses on what the indicators actually reveal

### v1.3 — Feb 2026
- Model selector redesigned to match panel style
- Misleading accuracy hints removed
- New **// About Results** block added explaining model variance, score reliability, and context limitations

### v1.2.1 — Feb 2026
- Increased max output tokens from 4096 to 8192 to prevent JSON truncation errors on longer texts

### v1.2 — Feb 2026
- Gemini 2.5 Flash set as default model
- Process button and model selector reorganised into a single row
- Token usage panel removed

### v1.1 — Feb 2026
- Model selector added: choose between Gemini 2.5 Flash Lite, Flash, and Pro

### v1.0 — Feb 2026
- Initial release: 20-indicator CIR scoring, Gemini API integration, copy, export, and share functions

---

## Contact

📧 [goa.contactpro@gmail.com](mailto:goa.contactpro@gmail.com)

© 2026 Games of Arcadia. All rights reserved.
