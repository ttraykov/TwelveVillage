# Deploy The Village on GitHub Pages

This is a static forum **prototype**. It does not have real accounts, posting, uploads, or video playback. Do not enter real passwords. All sample posts, member names and sponsorships are fictional.

## 1. Create a repository

Open https://github.com/new and set:

- Owner: `ttraykov`
- Repository name: `TwelveVillage` (matching capitalization)
- Visibility: **Public** (required for GitHub Pages on a GitHub Free account)
- **Do not** initialize with a README, `.gitignore`, or license. These files are included here.

## 2. Unzip locally

From your Mac terminal, first back up an existing folder **if present**. In `~/PersonalCode`, extract `TwelveVillage-v2-GitHub-Ready.zip` and enter its `TwelveVillage` folder.

```bash
cd ~/PersonalCode
unzip ~/Downloads/TwelveVillage-v2-GitHub-Ready.zip
cd TwelveVillage
open index.html
```

If `TwelveVillage` already exists and contains a Git repository, do NOT run `git init` again without checking your existing setup. This guide assumes a fresh folder without `.git`.

## 3. Push to GitHub

```bash
git init -b main
git add .
git commit -m "Initial The Village forum preview"
git remote add origin https://github.com/ttraykov/TwelveVillage.git
git push -u origin main
```

Use the exact remote URL above. It should not contain a placeholder username or duplicate `https://github.com/`.

## 4. Publish with Pages

At https://github.com/ttraykov/TwelveVillage/settings/pages select:

- Source: **Deploy from a branch**
- Branch: **main**
- Folder: **/(root)**

Save, and check the repository **Actions** tab for a green deployment check. When it has deployed, open:

https://ttraykov.github.io/TwelveVillage/

If Pages shows 404 right away, check whether the first deployment finished. The public URL is not live until GitHub Pages publishes successfully.

## 5. Later updates

```bash
cd ~/PersonalCode/TwelveVillage
git add .
git commit -m "Update forum preview"
git push
```

## Notes

- No build or installation step is needed: GitHub serves `index.html`, `styles.css`, `script.js` and `assets/` directly.
- Keep `.nojekyll` in the repository root.
- This static GitHub Pages preview has no backend or private user data. Anyone can view the source of a public repository.
- Use a proper host/backend and enforce upload moderation, user safety and security before enabling real accounts, attachments, payments or video uploads.
