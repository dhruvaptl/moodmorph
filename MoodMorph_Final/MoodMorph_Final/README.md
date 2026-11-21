# MoodMorph

MoodMorph is a zero-cost, browser-based creative moodboard prototype. It interprets a prompt using a transparent keyword lexicon and deterministic rules, then adapts a colour palette, typography pairing, design direction and procedural canvas artwork.

## Run it

1. Download and extract this folder.
2. Open `index.html` in a modern browser (Chrome, Edge, Firefox or Safari).
3. Enter an idea or choose one of the example prompts.
4. Generate, then try the interface morph toggle, palette swatches, regenerate, save, PNG export and JSON export.

No installation, account, API key, backend, hosting or build step is required.

## What is genuinely implemented

- Natural-language text input with a transparent keyword-to-parameter lexicon.
- Deterministic colour palette generation with HEX values.
- Rule-based typography recommendations and design-direction copy.
- Procedural canvas artwork generated locally in the browser.
- Optional adaptive interface theme.
- Local browser storage for saved prompts and variations (up to 20).
- PNG moodboard export, JSON specification export, CSS variable copying.
- Responsive layout.

## Important AI / research honesty

The core application does **not** call a neural language model or neural image-generation model. Prompt interpretation is a deterministic keyword/rule system; artwork is procedural canvas drawing. Unknown prompts receive a deterministic hash-based hue rather than semantic understanding. This is intentionally disclosed in the interface.

The optional external image checkbox attempts to use Pollinations over the internet. It is not required for the app, may be unavailable or rate-limited, and its availability/terms are outside this project's control. Do not describe it as a guaranteed free service. The core application works without it.

## Privacy and storage

Prompts and saved boards remain in the browser's `localStorage` on that device/browser. They are not synced to an account or server. Clearing browser site data can remove saved boards. The optional external image feature sends the prompt to the external image provider when enabled.

## Project structure

- `index.html` — complete self-contained application (CSS and JavaScript included).
- `README.md` — setup, features and technical limitations.

## Research directions

Potential experiments (collect actual observations before making claims):

1. Compare the palette and typography generated for prompts with one keyword changed (e.g. `dreamy lavender` vs `dark lavender`).
2. Test known-keyword prompts against prompts with unknown vocabulary; record when the fallback hue is used.
3. Ask participants to rate palette coherence, typography fit and perceived match to their prompt on a consistent scale.
4. Compare the interface with theme morphing enabled and disabled for readability and perceived fit.

Record prompt, matched keywords, generated parameters, participant ratings, sample size and limitations. Do not claim semantic AI understanding or research findings without evidence.

## License

No third-party runtime dependency is required for the core application. The optional Google Fonts stylesheet and optional external image service require an internet connection.
