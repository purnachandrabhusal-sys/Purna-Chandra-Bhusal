# Setup guide (for the person deploying — one-time, ~30 minutes)

The site is plain Jekyll with zero plugins beyond the GitHub Pages defaults,
so GitHub builds it automatically on every commit. No build tools, no
Actions workflows, no dependencies to maintain. Once deployed, the only
"maintenance" is editing text files.

## 1. Create the GitHub account and repository

1. Create a GitHub account **in Purna's name** (he should own his site
   long-term). Pick a clean username, e.g. `purnasurname`.
2. Create a new **public** repository named exactly
   `<username>.github.io` (e.g. `purnasurname.github.io`).
   Using this special name means the site publishes automatically at
   `https://<username>.github.io` with no extra path — which keeps every
   link in this project working without configuration changes.
3. Upload everything in this folder to the repository:
   on the repo page → **Add file → Upload files** → drag the whole
   contents in (including the `_layouts`, `assets` folders and the
   hidden `.gitignore` if your OS shows it — it's optional) → **Commit changes**.

## 2. Verify it's live

Wait 1–2 minutes, then open `https://<username>.github.io`.
If it doesn't appear: repo **Settings → Pages** → confirm
"Deploy from a branch" / branch `main` / folder `/ (root)`.

Check on your phone too — the layout is responsive with no JavaScript.

## 3. Point purna.online at GitHub Pages

Do this **after** step 2 works, so there's no downtime.

**In GitHub:**
1. Repo → **Settings → Pages → Custom domain** → enter `purna.online` → Save.
   (GitHub adds a `CNAME` file to the repo — leave it there.)
2. Recommended: GitHub **account** Settings → Pages → **Verified domains**
   → verify `purna.online`. This prevents anyone else from ever claiming
   the domain on GitHub Pages.

**At the domain registrar (where purna.online was bought):**
1. First remove the old Google Sites records: delete any `CNAME` pointing
   to `ghs.googlehosted.com` and any Google Sites A records. Also
   disconnect the domain inside Google Sites settings.
2. Add these DNS records:

   | Type  | Host | Value |
   |-------|------|-------|
   | A     | @    | 185.199.108.153 |
   | A     | @    | 185.199.109.153 |
   | A     | @    | 185.199.110.153 |
   | A     | @    | 185.199.111.153 |
   | CNAME | www  | `<username>.github.io` |

3. DNS can take from minutes up to ~24 h to propagate. When GitHub's
   Pages settings shows the domain check passed, tick **Enforce HTTPS**
   (the certificate is issued automatically and renews itself — free).

`https://purna.online` and `https://www.purna.online` will both work.

## 4. Hand it over

1. Send Purna the `HOW-TO-UPDATE.md` file (it's written for him).
2. Replace the placeholder `assets/cv/Purna-CV.pdf` with his real CV
   (same filename).
3. Work through every `[bracketed placeholder]` in:
   `_config.yml`, `index.md`, `about.md`, `publications.md`,
   `teaching.md`, `awards.md`.
4. Once he has them, paste his Google Scholar and ORCID URLs into
   `_config.yml` — buttons and footer links appear automatically.

## Notes

- **Backups:** the GitHub repo *is* the backup — every version of every
  file is kept forever and can be restored from the History tab.
- **Local preview (optional):** `bundle install && bundle exec jekyll serve`
  with Ruby installed. Never required — GitHub builds it for you.
- **Costs:** $0 beyond the domain renewal. GitHub Pages is free for
  public repos, HTTPS certificates are free and automatic.
- **Scaling later:** add a new page by copying any `.md` file, changing
  its `title` and `permalink`, and adding one line to the nav in
  `_layouts/default.html`. A blog can be added later with Jekyll's
  built-in `_posts` folder — no re-platforming needed.
