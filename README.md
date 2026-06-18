# TeamUpdraft — "The Updraft" concept refresh

A radical visual reskin of the [teamupdraft.com](https://teamupdraft.com/) homepage. **Same copy, same messaging** — a cutting-edge, motion-led design in the spirit of Midjourney / SpaceX / Paperclip.

It is a **single, self-contained `index.html`** — no framework, no build step, no CMS, no dependencies. Open it anywhere.

## Design concept — "The Updraft"
One ownable idea: a warm light source *rising* through a dark cinematic canvas. *Updraft* = rising warm air, so all motion travels upward and the rising embers represent the 5M+ sites being lifted and protected.

**Principles:** one rising light source · dark canvas so motion + product pop · oversized confident type · restraint in colour, richness in motion · every section earns its entrance.

## View it locally
Just double-click `index.html`, or serve the folder:
```bash
cd teamupdraft-refresh
python3 -m http.server 4321
# open http://localhost:4321
```

## Get a link you can send round
Because it's one static file, any of these gives you a shareable URL:

- **Fastest, no account:** drag the `teamupdraft-refresh` folder onto **[Netlify Drop](https://app.netlify.com/drop)** → instant public link.
- **GitHub Pages:** push this folder to a repo, enable Pages on the branch.
- **Any static host / S3 / Cloudflare Pages:** upload `index.html`.

## Notes
- Fully responsive (desktop → mobile) and respects `prefers-reduced-motion`.
- Accessibility pass done: skip link, keyboard focus rings, `<main>` landmark, ARIA on controls, decorative motion hidden from screen readers.
- The only network request is Google Fonts (Space Grotesk / Inter); it degrades gracefully to system fonts offline.
- The hero motion is a live `<canvas>` (not a video file), so it's resolution-independent and weightless, and it pauses when scrolled off-screen.
