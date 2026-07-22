# PLC Gaming Website

Public landing page for the **PLC Gaming** build — one real AutomationDirect
Productivity1000 P1-622 industrial PLC driving two games and a wall of custom
control panels over Modbus TCP.

This repo is **publish-only**: it holds the website and its photos, and nothing
from the private working repo (network addresses, SSH aliases, PLC program
files, handoff docs). Keep it that way.

## Structure

```
index.html        the whole site (self-contained, no build step)
images/           drop photos here, then reference them from index.html
```

## Adding photos

1. Put your `.jpg` / `.png` files in `images/`.
2. In `index.html`, replace a placeholder
   `<div class="frame">…</div>` block with
   `<img src="images/your-photo.jpg" alt="describe it">`.
3. Leave the surrounding `<figure>` and `<figcaption>` tags in place.

## Local preview

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Deployment

Published via GitHub Pages from the default branch, root folder
(Settings → Pages).
