# Nandhitha ♥ Aravindh — Wedding Invitation Website

A single-page animated wedding invitation site, ready to host for free on **GitHub Pages**.

## 📁 Files in this repo

- `index.html` — the full invitation page (self-contained: HTML + CSS + JS in one file)
- `.nojekyll` — tells GitHub Pages to skip Jekyll processing (not needed here, but avoids any build quirks)
- `README.md` — this file

## 🚀 How to publish it on GitHub Pages

1. **Create a new GitHub repository**
   - Go to https://github.com/new
   - Name it anything, e.g. `wedding-invitation` (the name becomes part of your URL)
   - Keep it **Public** (GitHub Pages free tier requires public repos, unless you have GitHub Pro/Team/Enterprise)
   - Don't initialize with a README (we already have one)

2. **Upload these files**
   - On the new repo's page, click **"uploading an existing file"**
   - Drag in `index.html`, `.nojekyll`, and `README.md`
   - Commit the changes (commit directly to the `main` branch)

   *(Or, if you use git locally:)*
   ```bash
   git init
   git add .
   git commit -m "Add wedding invitation site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

3. **Turn on GitHub Pages**
   - In your repo, go to **Settings → Pages** (left sidebar)
   - Under "Build and deployment" → **Source**, select **Deploy from a branch**
   - Under **Branch**, select `main` and folder `/ (root)`, then **Save**

4. **Get your live link**
   - Wait 1-2 minutes, then refresh the Pages settings screen
   - Your site will be live at:
     ```
     https://<your-username>.github.io/<your-repo>/
     ```
   - Share that link with your guests!

## ✏️ Editing later

Everything (styling, countdown date, venue, wording) lives inside `index.html`. To change something:
- Edit the file directly on GitHub (click the pencil ✏️ icon on the file page), or edit locally and re-push
- The countdown timer target date is set in the `<script>` section: `new Date("2026-10-24T19:00:00+05:30")`
- Venue/date text is in the `<footer>` section near the bottom
- The temple ceremony section (25 October 2026, 5:00-6:00 AM, Sri Pon Azhagu Nachiamman Kovil) is in the `<!-- TEMPLE CEREMONY -->` block just above the footer

## 📝 Notes

- The page uses Google Fonts (Bilbo, Arvo) loaded over the internet — guests need an internet connection to see the styled fonts (falls back to a generic serif otherwise).
- No backend, database, or build step required — it's a fully static site.
- Works great on mobile; the layout is responsive.
