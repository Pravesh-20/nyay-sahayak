# न्याय सहायक (Nyay Sahayak)

A single-page, phone-first writing companion for the daily **न्याय** newspaper column.
Speak (🎤 Hindi voice input) or type a topic → get a polished Hindi article in the author's
own voice (trained on his real published articles, signed *@ रुक्मा पुत्र ऋषि*), 3 headline
options, a matching AI image, and a social caption — with one-tap share to WhatsApp.

- **Runs entirely on Google Gemini's free tier** — one free API key, ₹0/month
  - Articles: `gemini-2.5-pro` (auto-falls back to `gemini-2.5-flash` if quota is hit)
  - Images: `gemini-2.5-flash-image`
- **Voice:** Web Speech API (`hi-IN`), continuous dictation with live transcript
- **Optional:** paste a Claude API key in Settings to write articles with Claude instead (pay-per-use)
- **No server:** one static `index.html`; the key is entered once in ⚙️ Settings and lives
  only in the phone's `localStorage` (never committed, never sent anywhere except Google/Anthropic directly)

## Setup

1. Open the deployed page → ⚙️ Settings
2. Paste a free Gemini API key ([aistudio.google.com/apikey](https://aistudio.google.com/apikey))
3. Save, tap 🎤 once to grant microphone permission, add the page to the home screen

## Notes

- Writing style is steered by sample articles stored in Settings — paste more past articles there to sharpen the voice
- Unverifiable claims are flagged with ⚠️[जाँच लें] — always fact-check before publishing
- History of the last 30 articles is kept on-device
