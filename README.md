# AnatoAR – Scan to 3D

A mobile-friendly anatomy learning page. Take or upload a picture, choose the organ, then spin a 3D model, tap each part to learn about it, earn XP and play a "find the part" game.

Educational use only. The 3D model is an original, simplified model and is **not** anatomically exact. Check details against your textbook.

## What works
- Take photo (opens the phone camera) or Upload a picture.
- 3D **heart** model: drag to rotate, pinch to zoom, tap a part for its details.
- XP, levels, parts-found progress and a find-the-part game (saved in the browser only).
- Other organs (brain, lungs, kidney, liver) are shown as "coming soon".

## What does NOT do (be honest in your demo)
- It does not recognise your picture. You choose the organ yourself after adding a picture, and the picture is only shown as a preview. It is not turned into the 3D model.
- Only the heart has a 3D model so far.

## Put it online with GitHub Pages (no coding)
1. Sign in at github.com and click **New repository**. Name it e.g. `anatoar`, set it **Public**, click **Create repository**.
2. On the new repo page click **uploading an existing file**.
3. Unzip this project. Drag **everything inside the folder** (`index.html`, `style.css`, `README.md`, and the `js` and `vendor` folders) into the upload box. Wait until all files finish uploading, then click **Commit changes**.
4. Go to **Settings > Pages**. Under "Build and deployment" choose **Deploy from a branch**, branch **main**, folder **/ (root)**, click **Save**.
5. Wait 1 to 2 minutes. Your site will be at `https://YOUR-USERNAME.github.io/anatoar/`. Open it on your phone.

## Test on your own computer first (optional)
Install Python, open a terminal inside this folder and run `python -m http.server 8000`, then open http://localhost:8000. (Double-clicking index.html may not work.)

## Files
- `index.html` page structure
- `style.css` navy/ocean glass design
- `js/app.js` 3D model, parts info, game
- `vendor/three.min.js` three.js r128 (MIT licence, see `vendor/LICENSE-three.txt`)

## Edit the learning text
Open `js/app.js`. The list called `PARTS` near the top holds every part's name, description, function, location and fact.

## Troubleshooting
- Blank page on GitHub: make sure the `js` and `vendor` folders uploaded with their files inside.
- 404 error: wait a couple of minutes after enabling Pages, then refresh.
- Camera button just opens a file picker: this depends on the phone. Use Upload instead.
- 3D not showing: try Chrome or Safari and check that WebGL is enabled.

## Credits
- three.js (MIT licence): https://threejs.org
- The 3D heart is an original model created for this project. No third-party model or image is included.
