# The Visual Uncomplex — Widgets

Self-contained interactive widgets for "The Visual Uncomplex" blog series, hosted via GitHub Pages and embedded into WordPress via `<iframe>`.

## Setup (one-time)

1. Create a new GitHub repo, e.g. `vu-widgets`
2. Push this folder structure to it
3. In repo Settings → Pages → enable GitHub Pages from the `main` branch, root folder
4. Your widgets will be live at:
   `https://<your-username>.github.io/vu-widgets/<folder-name>/`

## Folder structure

```
vu-widgets/
  cluster-01/
    index.html      <- Episode 1: scale-out cluster widget (this one)
  <episode-name>/
    index.html      <- next widget, same pattern
```

Each widget is a **single self-contained `index.html`** — HTML, CSS, and JS all inline, no external dependencies. This makes it trivial to embed and avoids any WordPress sanitization issues entirely (the script runs inside the iframe's own document, not WordPress's).

## Embedding in WordPress

In the post, add an **HTML block** (or Custom HTML block — iframes are allowed even where `<script>` is stripped) and paste:

```html
<iframe
  src="https://<your-username>.github.io/vu-widgets/cluster-01/"
  width="100%"
  height="500"
  style="border: none; border-radius: 12px;"
  loading="lazy">
</iframe>
```

Adjust `height` per widget if content is taller/shorter.

## Adding a new episode's widget

1. Create a new folder, e.g. `cluster-02/`
2. Add a self-contained `index.html` (same pattern as `cluster-01`)
3. Push to GitHub — it's live within ~1 minute at the same URL pattern
4. Paste one `<iframe>` block into the new WordPress post, pointing at the new folder

No CodePen, no copy-pasting into multiple panels, no per-post setup beyond one iframe tag.- 👋 Hi, I’m @anuragschandra911
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
anuragschandra911/anuragschandra911 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
