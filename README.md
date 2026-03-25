# AR Memory Trail (WebAR)

This project creates a browser-based AR apology experience with A-Frame + AR.js.
No app download required.

Current mode: image-target AR (Classmate-style, no Hiro marker).

## Files

- `index.html`: Main AR scene.
- `assets/set1-01.jpg` ... `assets/set1-06.jpg`: QR 1 photos.
- `assets/set2-01.jpg` ... `assets/set2-06.jpg`: QR 2 photos.
- `assets/targets.mind`: Compiled image target for tracking.

## 1) Add Your Photos

Place your photos in the `assets` folder with these exact names:

- `set1-01.jpg`
- `set1-02.jpg`
- `set1-03.jpg`
- `set1-04.jpg`
- `set1-05.jpg`
- `set1-06.jpg`
- `set2-01.jpg`
- `set2-02.jpg`
- `set2-03.jpg`
- `set2-04.jpg`
- `set2-05.jpg`
- `set2-06.jpg`

You can use `.png` if you update the file extensions in `index.html`.

## 2) Customize Messages

Edit the `<a-text>` entries in `index.html` to change apology lines and positions.

## 3) Deploy on GitHub Pages

1. Create a GitHub repository (example: `apology`).
2. Upload all files from this folder.
3. In repository settings, open **Pages**.
4. Set source to `Deploy from a branch`, branch `main`, folder `/ (root)`.
5. Save and wait for the site URL to appear.

Example URL:

- `https://a-k-0802.github.io/apology/`

## 4) Create QR Code

Generate a high-resolution QR code for your GitHub Pages URL and print it.

## 5) Image Target Setup (Required)

This version uses image-target tracking via MindAR.

1. Pick one clear image to act as your target (for example, notebook front page).
2. Compile it into `targets.mind` using the MindAR compiler.
3. Put the compiled file at `assets/targets.mind`.
4. Open your QR URL on phone and allow camera.
5. Point camera at that target image and keep it in frame until lock.

If you want a quick workflow, use MindAR image compiler (web):

- https://hiukim.github.io/mind-ar-js-doc/tools/compile/

## Notes

- This works best over HTTPS (GitHub Pages provides HTTPS).
- On first open, camera permission is required.
- Some iPhones may need Safari and motion/camera permissions enabled.
