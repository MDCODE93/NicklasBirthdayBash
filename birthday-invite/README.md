# Birthday Invitation + QR

This folder contains a small invitation webpage and a QR page.

## Files

- `index.html`: invitation content for guests
- `qr.html`: auto-generates a QR code that points to your invitation URL
- `nicklasbirthdaybash.html`: simple target page showing "NicklasBirthdayBash"
- `styles.css`: shared styling for both pages

## What To Customize

1. In `index.html`, update:
   - name/title
   - date and time
   - location and map link
   - RSVP email and phone
2. In `qr.html`, set these constants:

```js
const GITHUB_USERNAME = "YOUR_GITHUB_USERNAME";
const GITHUB_REPOSITORY = "YOUR_REPOSITORY_NAME";
```

This auto-builds the final URL:

`https://<username>.github.io/<repository>/birthday-invite/nicklasbirthdaybash.html`

Optional override: paste any public URL in the input field and click "Generate QR From URL".

## How To Publish

This project now includes a GitHub Pages workflow file:

- `.github/workflows/deploy-pages.yml`

To publish:

1. Put `personal-website` content in a GitHub repository root.
2. Push to the `main` branch.
3. In GitHub: Settings -> Pages -> Source: GitHub Actions.
4. Wait for the `Deploy static site to GitHub Pages` workflow to finish.
5. Your page will be available at:

`https://<username>.github.io/<repository>/birthday-invite/nicklasbirthdaybash.html`

## Test

Open `qr.html` in browser and scan the code with a phone camera.
It should open your invitation page directly.
