# Image Anonymizer

🔒 **Blur faces in images — 100% in your browser, no upload required.**

A privacy-first tool that detects and blurs faces in images entirely client-side. Your images never leave your device.

![Demo](demo.gif)

## Features

- ✅ **100% Client-side** — No server, no uploads, complete privacy
- ✅ **Face Detection** — Powered by face-api.js (TensorFlow.js)
- ✅ **Adjustable Blur** — Control blur intensity and detection confidence
- ✅ **Instant Download** — Get your anonymized image with one click
- ✅ **Drag & Drop** — Simple, intuitive interface
- ✅ **No Install** — Works in any modern browser

## Live Demo

👉 [Try it now](https://anubhav30.github.io/image-anonymizer)

## Use Cases

- Anonymize faces before sharing photos publicly
- Prepare datasets for ML without privacy concerns
- Blur faces in screenshots for documentation
- GDPR compliance for user-generated content

## How It Works

1. **Upload** — Drop an image or click to select
2. **Detect** — Face detection runs locally using face-api.js
3. **Blur** — Detected faces are pixelated/blurred
4. **Download** — Save the anonymized image

All processing happens in your browser using WebGL acceleration. Nothing is sent to any server.

## Tech Stack

- [face-api.js](https://github.com/vladmandic/face-api) — Face detection (SSD MobileNet)
- Vanilla JavaScript — Zero dependencies, no build step
- Canvas API — Image manipulation and blur effects

## Local Development

No build step required. Just serve the HTML file:

```bash
# Clone the repo
git clone https://github.com/anubhav30/image-anonymizer.git
cd image-anonymizer

# Serve locally (any method works)
python -m http.server 8000
# or
npx serve .
# or just open index.html in browser
```

## Performance

| Image Size | Detection Time | Total Time |
|------------|----------------|------------|
| 1080p | ~200ms | ~300ms |
| 4K | ~500ms | ~700ms |

*Tested on M1 MacBook Pro, Chrome 120*

## Contributing

PRs welcome! Some ideas:

- Add license plate detection
- Improve blur algorithms
- Add more export formats
- Mobile optimization

## License

MIT © [Anubhav Srivastava](https://github.com/anubhav30)

---

**Star ⭐ this repo if you find it useful!**
