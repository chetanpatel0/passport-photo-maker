# Passport Photo Maker

**Free, private passport and visa photos, made in your browser.**

🔗 **Live app:** https://YOUR-USERNAME.github.io/YOUR-REPO/

Upload a selfie and the app finds your face, removes the background, sizes your
head to the selected document rules and prepares a print-ready sheet. All
processing happens on your device; your photo is never uploaded.

## Features

- AI face detection and automatic alignment
- On-device background removal, with a manual restore/erase brush
- Presets for India, US, UK, Schengen, Canada, Australia, China, stamp size
  and custom sizes
- 14 jacket/suit overlays with drag, resize, tilt and fit controls
- Lighting, colour and edge-softness controls
- Print sheets for 4 × 6 in, A4 and 5 × 7 in paper, with optional cut lines
- JPG at 300 DPI, PNG, exact pixel sizes and KB-limited JPG
- Sheet JPG and single-page PDF
- No watermark, no sign-up, no credits, no footer in exports

## Privacy

Your photos never leave your device. Face detection, background removal and
export run locally in the browser. GitHub Pages only serves the single HTML
file; it never receives your photos.

## How to use

1. Open the live app.
2. Upload a photo or take a selfie.
3. Choose the document size and adjust the crop.
4. Pick a background colour and, if you want, a jacket.
5. Download the photo or a print-ready sheet.

For print shops, choose **Actual size / 100%**, not “Fit to page”.

## Offline use

The page embeds its fonts, suit images, AI models and WebAssembly runtime.
After it has loaded, it makes no network requests. You can also download
`index.html` and open it directly on your computer.

## Browser support

Chrome or Edge is recommended. The app needs `DecompressionStream` support
(Chrome/Edge 80+, Safari 16.4+, Firefox 113+). The first load is about 22 MB,
so allow a few seconds on mobile.

## Built with

- MediaPipe Face Landmarker
- ONNX Runtime Web
- MODNet portrait matting
- Canvas 2D and vanilla JavaScript

## Notes

- AI is optional. If a model cannot load, you can still crop, fit and download
  manually.
- Photo rules change. Always check the latest official guidelines before
  submitting.
- This repository contains the self-contained build, not the development source.

## License

Add a `LICENSE` file if you want to grant others permission to reuse the code.
Third-party libraries and models retain their own licenses.
