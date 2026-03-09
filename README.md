Bhagavad Gita — Wisdom for the Soul

Ancient wisdom for the modern soul.

A beautifully designed single-page web app that delivers personalized Bhagavad Gita verses based on how you're feeling — explained with warmth and depth by AI.

✨ What It Does

Choose your emotion — Select from 15 human emotions (grief, anger, fear, joy, hope, and more)
Seek wisdom — The app calls the Anthropic Claude API to find the most relevant Bhagavad Gita verse
Receive guidance — You get:

The Sanskrit transliteration of the verse
Its English translation
A compassionate, multi-paragraph explanation
A personal reflection prompt to internalize the teaching




🚀 Getting Started
Option 1 — Open directly in your browser
Just open index.html in any modern browser. No build step needed.
Option 2 — Host on GitHub Pages

Fork or clone this repo
Go to Settings → Pages
Set source to main branch, / (root) folder
Your app will be live at https://<your-username>.github.io/<repo-name>/


🔑 API Key Setup
This app uses the Anthropic Claude API. The API key is handled automatically when running via Claude.ai Artifacts.
If you're hosting this yourself, you'll need to add your API key. Open index.html and find the fetch call:
javascriptconst response = await fetch("https://api.anthropic.com/v1/messages", {
  method: "POST",
  headers: {
    "Content-Type": "application/json",
    "x-api-key": "YOUR_API_KEY_HERE",       // ← Add this line
    "anthropic-version": "2023-06-01",       // ← Add this line
  },
  ...
});

⚠️ Security note: For production apps, never expose your API key in frontend code. Use a small backend proxy (e.g. a Cloudflare Worker or Express server) to keep the key server-side.


🎨 Design

Aesthetic: Dark temple — deep blacks, gold leaf accents, saffron flame particles, rotating mandala background
Typography: Cinzel (headings) + Cormorant Garamond (body) — classical, spiritual, refined
Zero dependencies — pure HTML, CSS, and vanilla JavaScript
Fully responsive — works on mobile and desktop


🧘 Emotions Supported
Difficult EmotionsPositive EmotionsGrief, Anger, FearJoy, GratitudeAnxiety, LonelinessHope, LoveHopelessness, ConfusionPrideGuilt, Jealousy, Exhaustion

📁 File Structure
/
├── index.html    # The entire app — self-contained
└── README.md     # This file

🙏 Acknowledgements

The Bhagavad Gita — attributed to the sage Vyasa
Verse interpretations powered by Anthropic's Claude
Built with love for all souls navigating difficult days


"You have the right to perform your actions, but you are not entitled to the fruits of your actions."
— Bhagavad Gita, Chapter 2, Verse 47
