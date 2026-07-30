# How to update your website (no coding needed)

Your website is a small set of plain-text pages stored on **github.com**.
You edit them the same way you'd edit a Google Doc — in the browser,
on any computer. Every change you save goes live on **purna.online**
within about a minute, and every old version is kept, so nothing you
do can permanently break anything.

## The golden rules

1. You only ever edit **text between the markers** — never delete lines
   that look like code (`---`, `<div>`, `{{ }}`).
2. Anything in `[square brackets]` is a placeholder waiting for your
   real information.
3. If a page ever looks wrong after a change, don't panic — email the
   person who set this up, or use GitHub's **History** button on that
   file to see and restore the previous version.

## Which file is which

| To change… | Edit this file |
|---|---|
| Your name, email, tagline, Scholar/ORCID links (shown on every page) | `_config.yml` |
| The home page | `index.md` |
| Your bio and education | `about.md` |
| Publications list | `publications.md` |
| Courses and teaching | `teaching.md` |
| Awards and grants | `awards.md` |
| The CV file itself | see "Updating your CV" below |

## Editing a page (example: adding a publication)

1. Go to your repository on github.com and sign in.
2. Click `publications.md`.
3. Click the **pencil icon** (✏️, top right of the file).
4. Find the right section heading (they start with `##`). Copy an
   existing line that starts with `-`, paste it below, and change the
   details. Words wrapped in `*asterisks*` come out in *italics*.
5. Click the green **Commit changes…** button, then **Commit changes**
   again in the pop-up. That's it — check purna.online in a minute.

The same five steps work for every page.

## Updating your CV

1. Save your CV as a PDF named **exactly** `Purna-CV.pdf`.
2. On github.com, open the `assets` folder, then the `cv` folder.
3. Click **Add file → Upload files**, drag the new PDF in, and commit.
   Because the name matches, it replaces the old one and every
   "Download CV" button on the site now serves the new file.
4. Open `_config.yml`, click the pencil, and update the
   `cv_updated:` line (e.g. `"September 2026"`), so visitors can see
   the CV is current.

## Small formatting cheatsheet

| You type | Visitors see |
|---|---|
| `*Journal of Writing Studies*` | *Journal of Writing Studies* |
| `**Award name**` | **Award name** |
| `## Heading` | a new section with the red § mark |
| `[link text](https://example.com)` | a clickable link |
| `- Some item` | a list item |
| a blank line | a new paragraph |

## A habit worth keeping

Once a month, update the one-line **Currently** section at the bottom
of `index.md` (a talk you're giving, an article accepted, being on the
market). A current site signals an active scholar; a stale one signals
the opposite.
