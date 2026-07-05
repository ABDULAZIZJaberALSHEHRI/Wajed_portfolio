# Wajed Alsulaimani — Portfolio Site

A static one-page portfolio site built from the original PDF content: bio, background & expertise, competition win, Hilton journey, culinary heritage vision, menu architecture work, and the "viral creator to professional" story, ending with contact details.

## Files
```
index.html       – all page content/markup
style.css        – all styling (design tokens at the top of the file)
script.js        – nav scroll state, mobile menu, scroll-reveal animation
assets/          – all photos + logos extracted from the original PDF (optimized)
```

No build step, no dependencies — plain HTML/CSS/JS.

## Preview locally
Open `index.html` directly in a browser, or serve it:
```
cd site
python3 -m http.server 8080
```
Then visit http://localhost:8080

## Deploy on Render (free static site)

1. Push this folder to a GitHub repository (or upload directly — see below).
2. In Render: **New +** → **Static Site**.
3. Connect the repo.
4. Settings:
   - **Build Command:** (leave blank — no build needed)
   - **Publish Directory:** `.` (the root of this folder, where `index.html` lives)
5. Click **Create Static Site**. Render will give you a live `.onrender.com` URL.

### If you don't want to use GitHub
Render also supports deploying a static site by connecting to a Git repo only — so the quickest path is:
```
git init
git add .
git commit -m "Portfolio site"
git branch -M main
git remote add origin <your-empty-github-repo-url>
git push -u origin main
```
Then follow the Render steps above pointing at that repo.

## Customizing
- **Colors / fonts:** edit the `:root` variables at the top of `style.css`.
- **Copy:** edit text directly in `index.html`.
- **Photos:** swap files in `assets/` (keep the same filenames, or update the `src` paths in `index.html`).
- **Phone/email:** update the `tel:` / `mailto:` links and visible text in the `#contact` section of `index.html`.
