# Credas Connect – ID & AML check demo (client branding)

A clickable demo of the applicant journey, built from the Figma export "ID & AML Check – Credas". The branding panel lets you re-skin it per client: logo, client name, header, buttons, photo panel, progress steps, page background and the optional "Powered by Credas" mark.

Everything is in `index.html`: the screens, images and code are all inlined. The only external request is Google Fonts (Inter and Lato).

## Files

| File | Purpose |
|---|---|
| `index.html` | The demo itself |
| `.nojekyll` | Tells GitHub Pages to serve the file as-is |
| `README.md` | This file |

## Publishing on GitHub Pages

1. Add `index.html` and `.nojekyll` to the root of the repository (or to a `/docs` folder) and commit.
2. In the repository, open **Settings → Pages**, choose **Deploy from a branch**, then pick the branch and the folder you used.
3. After a minute or two the demo is live at `https://<account>.github.io/<repository>/`.

If the demo lives in a sub-folder of an existing Pages site (for example alongside the Connect training suite), drop `index.html` into its own folder, such as `/connect-demo/`. It is then served at `…/connect-demo/`.

## Using it

- **Present** (or press `P`) hides the branding panel. Use it before screen-sharing so the saved client list isn't visible.
- **Arrow keys** or the bottom bar move between screens. Buttons inside the screens follow the real journey, including the UK and non-UK address branches.
- **As designed / Desktop / Phone** switches which devices are shown.
- Each screen has its own link, so you can start partway through, for example `…/index.html#poi-select`.

Screen links: `#invite`, `#welcome`, `#terms`, `#personal`, `#address`, `#address-uk`, `#address-finder`, `#address-filled`, `#address-non-uk`, `#poa-info`, `#poa`, `#poa-picker`, `#poa-done`, `#poi-select`, `#poi-capture`, `#nfc-intro`, `#nfc-reading`, `#nfc-done`, `#selfie-info`, `#selfie-review`, `#selfie-done`, `#all-done`

## Saved client branding

Branding is saved in the browser you're using, not in the repository. To move it between people or machines:

- **Export** copies the saved clients to the clipboard as JSON. Save that text as a `.json` file.
- **Import** takes that JSON, pasted or as a file, and adds or updates the clients.

Committing a shared `branding.json` to the repository is a good way to keep the team's client set in one place. Each person then imports it once.

## Updating the screens

The screens are cut from the Figma export, so a change to a screen in Figma means re-exporting the PDF and regenerating `index.html`.
