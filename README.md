# Digima Messenger CRM — Privacy Center

Standalone, responsive static website designed for Digima Web Solutions Inc.'s Meta App Review preparation. Uses the company logo supplied for this project.

## Contents

- `/` — branded homepage with navigation
- `/privacy-policy/` — proposed CRM privacy notice
- `/data-deletion/` — proposed privacy and data deletion procedure
- `/contact/` — company contact / privacy channel information
- `/assets/` — styles and Digima logo

**Current status: REVIEW DRAFT — NOT APPROVED FOR PUBLICATION.**

No real customer data, tracking, forms, third-party fonts, libraries, analytics, API calls, or backend services are included. The official logo is a user-supplied PNG. All links between pages work without JavaScript.

## Required approval before publication

1. Confirm the business representative's permission to publish the company's privacy policy and to host it under a company-controlled Netlify account.
2. Approve the business's *actual* privacy policy (with legal/privacy officer as appropriate), including lawful purposes and processing bases.
3. Replace every "to be confirmed", "pending" and draft annotation with real verified content. Identify actual hosting location and service providers, privacy contact email, registered address and authorized deletion process.
4. Confirm actual retention periods or valid criteria for messages, files, logs and backups. Avoid promises the application cannot keep.
5. Test that privacy and deletion requests are received and handled. Confirm company policy for Page-owner roles and deletion exceptions.
6. Remove the prominent draft banner (`draft-notice` block), draft-only labels and review text from all four HTML pages **only after** approval. Remove the draft phrase in the footer and replace it with the approved effective date.
7. Verify Meta's current App Review fields, public reachability, HTTPS, and URL accessibility without authentication or geoblocking.
8. Add the *approved, working URLs* to the Meta app settings; do not use hypothetical domain names.

### Locating unfinished material

Run `grep -RinE 'pending|to be confirmed|awaiting company|draft|company review|not approved|confirmation needed' --include='*.html' .` from the project folder. Every relevant occurrence must be examined, not blindly replaced.

## Preview locally (Ubuntu)

```bash
cd digima-privacy-center
python3 -m http.server 8000
```

Visit `http://localhost:8000` and explore the navigation. Press Ctrl+C to end the local server.

## Publish to Netlify after approval

1. Sign in to **Digima's own Netlify account** (or a corporate team account). Avoid an intern's personal account as the sole owner of an official legal notice.
2. Extract the supplied ZIP. Ensure the folder contains `index.html` at its root.
3. Go to https://app.netlify.com/drop and drag the entire `digima-privacy-center` folder into the deploy zone. (Do not drag the ZIP; Netlify's current primary documentation asks users to unzip first.)
4. Open the provided HTTPS `*.netlify.app` domain and test the homepage, `/privacy-policy/`, `/data-deletion/` and `/contact/` on desktop and mobile. Make sure all links work in a private/incognito window.
5. Optionally configure an official custom subdomain later. The suggested hostname is **not reserved**; availability must be confirmed when deploying.
6. Add the exact **live** privacy policy URL to Meta for Developers and (where required) data deletion instructions URL.
7. Document who is responsible for updating the site when the CRM changes.

Netlify docs: https://docs.netlify.com/deploy/create-deploys/

## Important

This site is an informational artifact only. It does not implement data deletion, authenticate customers, or change Digima's CRM, database, Facebook Pages, or Meta app settings. Company's lawful processing and privacy program must match the eventual published notice.
# Digima-Privacy-Policy
