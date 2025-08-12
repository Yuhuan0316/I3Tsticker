I3T WebAR Sticker — MindAR + A-Frame
====================================

This folder contains a starter WebAR experience that tracks your sticker and shows a clickable floating card that opens your website.

Files
-----
- index.html         — the WebAR page; hosts the MindAR scene with a clickable card.
- sticker.mind       — **placeholder** MindAR target file. Replace with your real compiled target file.
- sticker-sample.png — the sticker image you shared (for reference).

How to build the MindAR target (.mind)
--------------------------------------
1) Install the MindAR image target compiler (either CLI or the online tool). The official docs explain both options.
   - If using the CLI: you'll need Node.js installed.
2) Use your final print-ready sticker image (same aspect/contrast as the printed sticker).
3) Compile to a `.mind` file with **one** target (index 0). Name it `sticker.mind` and put it next to index.html.

Tips to improve tracking for this sticker
-----------------------------------------
- Your current design has large solid shapes and rotational symmetry. To make tracking more reliable:
  • Increase local detail/texture (fine patterns, edges) inside the circle.
  • Break symmetry by adding a small distinctive mark or micro-text in ONE quadrant.
  • Avoid glossy paper; use matte. Print at least 7–10 cm wide.
  • Ensure the printed sticker matches the reference image exactly (no cropping/ratio change).

Deploy
------
- Host these files on HTTPS (Netlify, Vercel, GitHub Pages).
- Put a small QR code near the sticker that links to the hosted `index.html`.
- On the page, tap "Start AR", point the camera at the sticker, then tap the blue card to open your site.

Customize
---------
- Edit `targetUrl` in index.html to change the link.
- Replace the blue card with your own 3D model, image, or animated layout.
