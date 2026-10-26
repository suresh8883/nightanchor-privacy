# nightanchor-privacy

The public privacy policy page for the NightAnchor Android app (sibling repo
`nightanchor-android`, publisher ThaksTech). One file matters: `index.html`. GitHub Pages
serves it from `main` at the repo root (legacy build, no CNAME, no Jekyll) at
https://suresh8883.github.io/nightanchor-privacy/ , the privacy-policy URL given to the
Play Console. Live and in use; not an archive. `README.md` is a one-line stub.

**Read this file first. It replaces exploring the project.**

## Hard rules

1. **The policy text is user-facing legal copy and a Play Store commitment.** Every
   factual claim in `index.html` must stay consistent with
   `../nightanchor-android/DATA_SAFETY.md` (the Data Safety form answers) and the Play
   listing. Change wording only when asked, and only after checking the app's real
   behaviour in `nightanchor-android` (what is stored, what can leave the device).
2. **Order when the app changes data handling:** update and publish this page first, then
   the Data Safety form, then ship the app. The policy's "Changes" section promises this.
3. On any wording change bump the `Effective:` date and say what changed and why in the
   commit body (commit 894d413 is the pattern).
4. No scripts, analytics, web fonts or other external requests in `index.html`; the page
   itself must not collect anything.
5. Agents may commit on a branch and open a PR; never push to `main` (Pages deploys it).

## Current state (2026-10-18)

- Effective 2026-08-09; the "Team rosters" section covers v0.5.0 photo import of team
  duty sheets. `nightanchor-android/PRIVACY_POLICY.md` (last touched 2026-07-13) lacks
  that section and still reads "Effective: [fill the date]"; `index.html` is the source
  of truth, the .md is the older draft.
- `nightanchor-android/DATA_SAFETY.md` is still headed v0.4.1 / versionCode 5 while the
  app is 0.5.0 / versionCode 6. Verify against code before relying on it for new claims.
- Preview with `open index.html`; there is no build step. Do not modernise the page
  (frameworks, CSS tooling) unless asked.
