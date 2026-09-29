# 8D Studio — recovered source

Public recovery snapshot of **8D Studio**, recovered from the live Vercel production deployment on 2026-09-29.

Live app: https://8d-studio.vercel.app

## What is recovered

- `index.html` — original production-served source, including HTML, CSS and JavaScript (~52.8 KB)
- Core Web Audio / HRTF / room reflection / Doppler / bass-anchor processing
- File input, tab-audio capture, demo loop and offline WAV/WebM export UI

The production page also references `manifest.json`, `sw.js`, and `icon-512.png`. Those ancillary PWA files are not included in this recovery snapshot yet because the connected Vercel interface currently exposes the live root document but not authenticated sub-path file download.

## Security check

Before publishing, the recovered main source was scanned for common API keys, GitHub tokens, AWS keys, private-key blocks and obvious secret/token/password assignments. No matches were found.

## License

This recovery branch lives in a repository licensed under MIT. A dedicated `8d-studio` repository can be created later and this snapshot moved there without changing the recovered source.
