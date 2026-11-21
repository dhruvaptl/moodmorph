# MoodMorph — Adaptive AI-Inspired Moodboard Generator

**Turn your ideas into visual moods.**

MoodMorph is a zero-cost, browser-based creative moodboard generator that transforms text prompts into personalised visual directions. Describe a mood, aesthetic, or idea, and MoodMorph generates a coordinated colour palette, typography pairing, design direction, and procedural artwork.

What makes it different? The interface itself can morph to reflect the mood you're creating.

## ✨ Live Demo

**[Explore MoodMorph](https://moodmorphh.netlify.app/)**

## Features

- **Prompt-Based Generation:** Enter a mood, aesthetic, or creative idea to generate a moodboard.
- **Dynamic Colour Palettes:** Generate coordinated colour combinations with HEX values.
- **Typography Pairings:** Receive typography recommendations based on your selected mood.
- **Procedural Artwork:** Create browser-generated canvas visuals.
- **Adaptive Interface:** Toggle interface morphing to make the UI reflect the generated mood.
- **Moodboard Library:** Save and revisit up to 20 generated variations locally.
- **Export Options:** Download moodboards as PNG, export JSON specifications, and copy CSS variables.
- **Responsive Experience:** Designed to work across modern desktop and mobile browsers.

## 🛠️ How It Works

MoodMorph uses a transparent keyword-based interpretation system to map user prompts to visual parameters.

1. The user enters a creative prompt.
2. A keyword lexicon identifies recognised mood and aesthetic terms.
3. Deterministic rules generate colour, typography, and design-direction parameters.
4. A procedural canvas engine creates corresponding artwork.
5. The interface can optionally adapt its appearance to the generated mood.

## Technology & Implementation

- HTML5
- CSS3
- Vanilla JavaScript
- HTML Canvas API
- Browser LocalStorage
- Pollinations (optional external image generation)
- Google Fonts (optional typography resources)
- Netlify (deployment)

## Getting Started

MoodMorph requires no installation, backend, API key, or build process.

**Run locally:**

1. Clone or download this repository.
2. Extract the project files.
3. Open `index.html` in a modern web browser.
4. Enter a prompt or select an example.
5. Generate your moodboard and explore its customisation and export features.

Alternatively, use the [live deployment](https://moodmorphh.netlify.app/).

## AI Transparency & Technical Limitations

An important aspect of MoodMorph is transparent implementation.

The core application does **not** use a neural language model or neural image-generation model. Its prompt interpretation relies on a deterministic keyword lexicon and rule-based logic.

- Recognised keywords influence generated visual parameters.
- Unknown prompts use a deterministic hash-based hue fallback.
- Artwork is produced through procedural JavaScript canvas drawing.
- The optional Pollinations integration attempts external image generation but depends on third-party availability.

This distinction is intentional: MoodMorph demonstrates prompt-driven creative interaction without misrepresenting rule-based generation as semantic AI understanding.

## Privacy & Data Storage

- Saved moodboards are stored locally using browser `localStorage`.
- No user account or application backend is required.
- Saved content is not synchronised across devices.
- Clearing browser site data may remove saved moodboards.
- Enabling optional external image generation sends the prompt to the external image provider.

## Research & Future Exploration

MoodMorph also offers opportunities to explore the relationship between text prompts and visual design.

Potential experiments include:

1. Evaluating how changing individual prompt keywords affects generated colour palettes.
2. Comparing recognised-keyword prompts with unfamiliar vocabulary.
3. Measuring perceived visual coherence and prompt-to-design relevance through user feedback.
4. Evaluating interface readability with adaptive theming enabled and disabled.

These are proposed research directions, not completed experiments or established findings.

## Project Structure

```text
MoodMorph/
├── index.html
└── README.md
```

- `index.html` — Self-contained application containing HTML, CSS, and JavaScript.
- `README.md` — Project documentation.

## License

No third-party runtime dependency is required for the core application. Optional Google Fonts and external image generation require an internet connection.

---

**Built as a creative exploration of prompt-driven design, procedural graphics, and adaptive user interfaces.**
