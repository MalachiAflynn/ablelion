# ableLion

A public, multi-year build log of designing flight technology from scratch: frames, firmware, and the sensing that ties them together. The documentation is the asset.

This folder is the first version of the ableLion website. It's a static site (plain HTML + CSS, no build step, no dependencies), so it can go live on any free static host as-is.

---

## What's in here

| File | What it is |
|------|------------|
| `index.html` | Homepage. Brand, the "building in public" intro, and a status feed. |
| `roadmap.html` | The NOW / NEXT / HORIZON roadmap. |
| `mini-drone.html` | Build page for the Mini Drone (CICS 256 group project). |
| `style.css` | Shared stylesheet for all three pages. |

All four files must stay in the **same folder**, with no subfolders. The pages link to each other by bare filename and all share `style.css`.

To preview locally, just double-click `index.html` and it opens in your browser.

---

## Next steps: get it live

Deploying on **GitHub Pages** keeps the site in a repo right next to your drone code, which fits the build-in-public idea. Free, with custom-domain support later.

### 1. Make the repo
- Create a new **public** repo.
- Name it `ablelion` and the site lives at `yourusername.github.io/ablelion`.
- Or name it `yourusername.github.io` and it lives at the root domain instead.

### 2. Add the files
- Put all four files (`index.html`, `roadmap.html`, `mini-drone.html`, `style.css`) in the **repo root**.
- No subfolders. Flat structure matters because the links are bare filenames.

### 3. Open the gate (turn on Pages)
- Repo → **Settings** → **Pages**.
- Under **Build and deployment**, set Source to **Deploy from a branch**.
- Pick the `main` branch and the `/ (root)` folder. Save.
- Wait about a minute. The live URL appears at the top of that same Pages panel.

### 4. Confirm
- Open the URL and click through the nav.
- If the page looks unstyled, it's almost always a filename case mismatch. GitHub is case-sensitive, so `style.css` must match exactly.

After this, every update is just committing the changed file(s) to the repo. The site redeploys on its own.

---

## Other free hosting options

If you'd rather not use GitHub Pages:

- **Netlify** — drag-and-drop the folder onto their site and it's live in a couple minutes. Easiest possible path.
- **Cloudflare Pages** — free and fast, connects to a GitHub repo.
- **Vercel** — free tier, Git-connected.

All four handle a plain static site like this without any configuration.

---

## What's planned next

The nav already has placeholders marked SOON:

- **Software** — write-ups of the ESP32 flight code.
- **Log** — dated build-log entries.

Two things will turn current placeholders into real pages:
- The actual contents of the MAKE 256 sensor bag (flips the Sensing card from "coming soon" to a live perception-experiments page).
- The first dated log entry.

---

ableLion · MINI DRONE → V1 → ∞
