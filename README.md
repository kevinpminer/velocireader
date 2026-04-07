# Velocireader — RSVP Paper Reader

A fast, minimal tool for speed-reading academic papers using **Rapid Serial Visual Presentation (RSVP)**.

Upload a PDF or text file and read it word-by-word at your own pace.

🔗 **[Try it live on GitHub Pages →](https://yourusername.github.io/velocireader/)**

![Screenshot](screenshot.png)

## Features

- **PDF & TXT upload** — drag-and-drop or click to upload
- **RSVP display** with Optimal Recognition Point (ORP) highlighting
- **Adjustable speed** — 100 to 1,000 WPM via slider or keyboard
- **Multi-word chunks** — display 1, 2, or 3 words at a time
- **Click-to-jump** — click any word in the full text panel to start reading from there
- **Smart pacing** — pauses slightly longer on punctuation and long words
- **Reading time estimate** — shows total time and remaining time
- **Progress tracking** — visual progress bar and percentage
- **Keyboard shortcuts**:
  - `Space` — Play / Pause
  - `←` / `→` — Skip back / forward 5 words
  - `↑` / `↓` — Speed up / slow down
- **Fully client-side** — no server, no data collection, your papers stay on your device

## Deploy to GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to **Deploy from a branch**, select `main` and `/ (root)`
4. Your site will be live at `https://yourusername.github.io/velocireader/`

That's it — it's a single `index.html` file with no build step.

## Local Development

Just open `index.html` in a browser. No dependencies to install, no bundler required.

```bash
# Or use any local server:
python3 -m http.server 8000
# then visit http://localhost:8000
```

## How RSVP Works

Rapid Serial Visual Presentation displays text one word (or chunk) at a time at a fixed position, eliminating the need for eye movement across lines. The **Optimal Recognition Point** (the red-highlighted letter) is positioned at approximately 30% into each word, which is where the eye naturally focuses for fastest recognition.

Research suggests trained RSVP readers can comfortably read at 300–500 WPM, compared to ~250 WPM for traditional reading.

## Tech

- Vanilla HTML/CSS/JS — no frameworks
- [PDF.js](https://mozilla.github.io/pdf.js/) for PDF text extraction (loaded from CDN)
- JetBrains Mono + Literata fonts

## License

MIT
