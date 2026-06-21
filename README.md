# Portfolio — "Unveil" style

A minimal portfolio page. The list of work sits on mostly empty space, and
each title *unveils* its image on hover (desktop) or shows it inline (mobile).
Everything is in a single `index.html` — no build step, no dependencies.

## File structure

```
your-repo/
├── index.html        ← the whole site (edit this)
└── images/           ← put your images here
    ├── project-01.jpg
    ├── project-02.jpg
    └── ...
```

Create the `images` folder yourself and drop your photos in. Until you do,
the page shows labelled placeholders that name the exact file it expects.

## How to edit

Open `index.html` and look for the `EDIT` comments. The parts you'll touch:

1. **Title** — the `<title>` tag (browser tab text).
2. **Hero** — your name and one-line statement, near the top of `<body>`.
3. **Projects** — each project is one `<li class="project">` block. To add one,
   copy a block and change:
   - `data-image="images/your-file.jpg"` — the image path
   - the number (`01`), the title text, and the meta line (`2026 — Category`)
4. **Footer** — your email and links.

You don't need to touch the `<style>` or `<script>` sections. To recolor the
whole site, change the values under `:root` at the top of the `<style>` block.

Image tip: portrait-ish photos (4:5) fill the frame best; anything works since
they're cropped to fit.

## Put it on GitHub Pages

1. Create a new repository on GitHub.
   - For a site at `https://<username>.github.io`, name the repo exactly
     `<username>.github.io`.
   - For a project site at `https://<username>.github.io/<repo>`, use any name.
2. Upload `index.html` and your `images/` folder to the repo root
   (drag-and-drop in the GitHub web UI, or `git push`).
3. Go to **Settings → Pages**, set **Source** to *Deploy from a branch*,
   pick the `main` branch and `/ (root)` folder, then **Save**.
4. Wait ~1 minute. Your live URL appears at the top of that same Pages screen.

That's it — edit `index.html`, commit, and the live site updates automatically.
