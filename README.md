# padelstreak

The public website for **Padel Streak**, a padel scoreboard and stats app for
iPhone and Apple Watch. Two static pages, served by GitHub Pages:

| Page | URL | Used for |
|------|-----|----------|
| Support | https://kessiacastro.github.io/padelstreak/ | App Store Connect "Support URL" (required) |
| Privacy policy | https://kessiacastro.github.io/padelstreak/privacy/ | App Store Connect "Privacy Policy URL" (required) |

This repo is **public** because GitHub Pages requires it on a free plan. It holds
only the website — the app source lives in a separate private repo.

## Editing

Plain HTML with inline CSS, no build step and no dependencies. Edit the file,
commit, push; Pages redeploys in a minute or two.

- `index.html` — support page
- `privacy/index.html` — privacy policy
- `.nojekyll` — skips Jekyll processing, since these are hand-written pages

## Things to keep in mind

- **The contact address appears on both pages.** It's currently a personal
  address; when a dedicated support address exists, change it in `index.html`
  and `privacy/index.html` (one `mailto:` and one link text in each).
- **Changing the privacy policy means bumping its effective date**, which is
  stated at the top of `privacy/index.html`. The policy itself promises this.
- **Don't change these URLs once the app is submitted.** They're filed with
  App Store Connect, and a dead privacy policy URL is grounds for rejection.
  Renaming this repo or the `privacy/` folder would break them.
- The canonical copy of the policy text also lives in the app repo at
  `store/PRIVACY_POLICY.md`; keep the two in step if you edit either.
