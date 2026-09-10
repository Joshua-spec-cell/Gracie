# For Gracie

A small, mobile-first appreciation site. Single HTML file, no backend, no build step.

## 1. Add Gracie's photos
Drop 4 photos into the `images/` folder, named exactly:

```
images/gracie-1.jpg
images/gracie-2.jpg
images/gracie-3.jpg
images/gracie-4.jpg
```

Until you add them, each photo slot shows a soft placeholder — the page still works and the captions still show, so you can preview the layout right away.

Want a 5th photo, or different order? Open `index.html`, find the `<section id="gallery">` block, and copy one `<figure class="polaroid">...</figure>` to add another, or edit the `src` / caption text on any of the four.

Tips for best results:
- Portrait-ish or square photos work best (they crop to a 4:5 frame).
- Keep each file under ~500KB for fast loading — export at around 1200px on the long edge.

## 2. Add music (optional)
The soft music button in the bottom-right corner looks for a file at:

```
music/ambient.mp3
```

If it's not there, the button just sits there quietly and does nothing when tapped — nothing breaks. Add any gentle instrumental track (keep it soft and low) and it'll work automatically. No autoplay — she has to tap it herself.

## 3. Preview it locally
Just open `index.html` in a browser. No server needed.

## 4. Deploy on GitHub Pages
1. Create a new GitHub repo (can be private or public).
2. Upload `index.html`, the `images/` folder, and (optionally) the `music/` folder.
3. Go to **Settings → Pages**, set the source branch to `main` (root folder), and save.
4. GitHub gives you a link like `https://yourusername.github.io/repo-name/` — that's the link to send her.

That's it — no build tools, no dependencies beyond two Google Fonts loaded from a CDN.
