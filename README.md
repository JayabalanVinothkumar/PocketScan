# PocketScan

Offline document scanner for iPhone (PWA) — turns photos into crisp, high-quality PDFs. Inspired by CamScanner. No server, no uploads: everything runs and is stored on the phone.

**Live app:** https://jayabalanvinothkumar.github.io/PocketScan/

## Install on iPhone
1. Open the live link above in **Safari**.
2. Tap **Share → Add to Home Screen**.
3. Open PocketScan from the home-screen icon once while online — after that it works fully offline.

## Features
- Camera scan with automatic page-edge detection and perspective correction
- Manual corner/edge adjustment with magnifier
- Batch import from Photos (auto-cropped)
- Filters: Original, Magic Color, No Shadow, Grayscale, B&W, Lighten
- Brightness, contrast, sharpness, rotate, re-crop, apply to all pages
- Multi-page documents: reorder, delete, add, rename
- Export PDF (A4 / Letter / fit image; High / Medium / Small) or JPGs, via the iOS share sheet

## Files
| File | Purpose |
|---|---|
| `index.html` | The whole app (UI, image processing, PDF writer) |
| `sw.js` | Service worker — caches the app for offline use |
| `manifest.webmanifest` | Home-screen app metadata |
| `icon-180.png`, `icon-512.png` | App icons |

Scans live only on the device; deleting the home-screen app deletes them, so export anything important.
