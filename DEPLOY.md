# Publish to GitHub Pages

Repo name: **`invasion-number-vegetables`**

Upload **everything inside this `website` folder** to the **root** of that repo (not a nested `website` folder).

Your repo should look like:

```
invasion-number-vegetables/
  index.html
  styles.css
  images/
    hero.png
    screenshot-flight.jpg
    screenshot-cockpit.jpg
    (... other screenshot-*.jpg files)
  video/
    official-trailer.mp4
    veg-game-short.mp4
  DEPLOY.md
```

Upload the `video` folder too (both trailers play from the site as local MP4s).

## Step 1 — Create the repo on GitHub

1. Log in at [github.com](https://github.com).
2. Click **+** (top right) → **New repository**.
3. **Repository name:** `invasion-number-vegetables`
4. **Public**
5. Do **not** add a README, .gitignore, or license (keeps the first upload simple).
6. Click **Create repository**.

## Step 2 — Upload the files

On the empty repo page:

1. Click **uploading an existing file** (or **Add file** → **Upload files**).
2. Drag in from your PC:
   - `index.html`
   - `styles.css`
   - `DEPLOY.md` (optional)
   - the whole `images` folder (with `hero.png`)
   - the whole `video` folder (with `official-trailer.mp4` and `veg-game-short.mp4`)
3. **Commit message:** e.g. `Add coming-soon landing page`
4. Click **Commit changes**.

## Step 3 — Turn on GitHub Pages

1. Repo → **Settings** → **Pages** (left sidebar).
2. **Build and deployment** → **Source:** **Deploy from a branch**
3. **Branch:** `main` (or `master`) → folder **`/ (root)`**
4. Click **Save**.

After 1–3 minutes your site is live at:

**`https://YOUR_GITHUB_USERNAME.github.io/invasion-number-vegetables/`**

Use that URL in Steam’s **Website** field when you are ready.

## Step 4 — When Steam store page exists

1. Edit `index.html` on GitHub (pencil icon) or upload a new copy from your PC.
2. Replace the disabled button with a real link, e.g.:

   ```html
   <a class="btn btn-steam" href="https://store.steampowered.com/app/YOUR_APP_ID/" target="_blank" rel="noopener noreferrer">
     View on Steam
   </a>
   ```

3. Remove `btn-disabled`, `aria-disabled`, and `tabindex="-1"` from that link.
4. Update the “Coming soon” text in `.steam-note` if you like.

## Trailer

Embedded YouTube: `https://youtu.be/swQ1hmRX5po`  
Section `#trailer` in `index.html`. To change the video, update the iframe `src` embed ID.

## Adding screenshots later

1. Copy PNG/JPG files into `images/` (e.g. `images/screenshot-chopper.png`).
2. Add `<figure>` blocks in the `#screenshots` section of `index.html` (copy the existing title-screen example).
3. Upload the new/changed files to GitHub.

## Optional — GitHub Desktop (easier updates)

1. Install [GitHub Desktop](https://desktop.github.com/).
2. **File → Clone repository** → select `invasion-number-vegetables`.
3. Copy updated files from this `website` folder into the cloned folder.
4. **Commit to main** → **Push origin**.

## Local preview (optional)

Double-click `index.html` in File Explorer to open it in your browser. Layout should match the live site.
