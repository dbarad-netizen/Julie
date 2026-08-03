# Lighter 🪶

*Everything, made smaller.* A tiny ADHD-friendly task app: brain-dump when overwhelmed, get cliff-notes back, do one thing at a time.

## How to host on GitHub Pages (about 3 minutes)

1. Create a new **public** repository on GitHub (name it `lighter` or anything you like).
2. Upload all the files in this folder to the repository root: `index.html`, `sw.js`, `manifest.json`, `icon.png`, `icon-512.png` (this README is optional).
3. In the repo, go to **Settings → Pages**. Under "Build and deployment," set Source to **Deploy from a branch**, choose branch **main** and folder **/ (root)**, and save.
4. Wait a minute or two, then visit `https://YOUR-USERNAME.github.io/lighter/`.

## Putting it on her phone

Open that URL on her phone, then:

- **iPhone (Safari):** tap Share → **Add to Home Screen**
- **Android (Chrome):** tap the menu (⋮) → **Add to Home screen** / **Install app**

It opens full-screen with the green leaf icon, like a normal app.

## How it works

- All tasks are stored **on the phone only** (browser local storage). Nothing is uploaded except the text of a task at the moment it gets AI-shrunk.
- The AI shrinking calls a small private endpoint (already live on Supabase) that turns rambly notes into a 3-line card: short title, time estimate, tiny first step. If it's ever unreachable, the app quietly falls back to a simple trim — nothing breaks.
- No accounts, no tracking, no red "overdue" anything.
