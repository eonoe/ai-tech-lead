# Tech Lead 2.0

Landing page for a self-guided course on building with coding agents. It has two tracks: a free **Coding Agents 101** and a deeper, project-based **Tech Lead 2.0** built around seven phases.

It is one static HTML file. No framework, no build step. The only external dependency is Google Fonts, loaded over HTTPS.

## Run it locally

Open `index.html` in a browser. That is the whole thing.

## Deploy on GitHub Pages

1. Push this repo to GitHub (public repo, free Pages).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick **main** and the **/ (root)** folder, and save.
4. Wait about a minute. The live URL appears on the same screen, in the form `https://<username>.github.io/<repo>/`.

To update the live site, commit a new version of `index.html`. Pages redeploys on its own.

## Editing

Everything lives in `index.html`. The page copy and structure are mostly inline, and three sections are rendered from small JavaScript arrays near the bottom of the file:

- `phases` — the seven phases (number, tag, name, the learning, what you apply, what you ship)
- `fits` — the "Is this for you?" list
- `faqs` — the FAQ

Those strings use single quotes, so avoid apostrophes inside them or the script will break. Use "do not" instead of "don't", and so on.

## Before going live

The call-to-action buttons are placeholders (`onclick="return false"`). Point them at your real signup or checkout links before you share the page.
