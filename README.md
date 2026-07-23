# न्याय सहायक (Nyay Sahayak)

A single-page, phone-first writing companion for the daily **न्याय** newspaper column.
Type or speak a topic → get a polished Hindi article (in the author's own voice), 3 headline
options, a matching AI image, and a social caption — with one-tap share to WhatsApp.

- **Article writing:** Claude API (`claude-opus-4-8`) with structured JSON output
- **Image generation:** Gemini API (`gemini-2.5-flash-image`, free tier)
- **No server:** one static `index.html`; API keys are entered once in ⚙️ Settings and live
  only in the phone's `localStorage` (never committed, never sent anywhere except
  Anthropic/Google directly)

## Setup

1. Open the deployed page → ⚙️ Settings
2. Paste a Claude API key ([console.anthropic.com](https://console.anthropic.com/settings/keys) — set a small monthly spend limit)
3. Paste a Gemini API key ([aistudio.google.com/apikey](https://aistudio.google.com/apikey))
4. Optionally paste more past articles into the style box (better voice matching)
5. Save, then add the page to the phone's home screen

## Notes

- Writing style is steered by sample articles stored in Settings
- Unverifiable claims are flagged with ⚠️[जाँच लें] — always fact-check before publishing
- History of the last 30 articles is kept on-device
