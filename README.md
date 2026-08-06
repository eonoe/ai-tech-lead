# ai-tech-lead

The free **Coding Agents 101** workshop pages, plus the Apps Script backend that collects signups.

The **Tech Lead 2.0** landing page used to live here at `index.html`. It moved to the root domain — repo [eonoe/eonoe.github.io](https://github.com/eonoe/eonoe.github.io), served at <https://eonoe.github.io/>. The `index.html` left here is only a redirect stub pointing at that root; edit the landing page in the other repo.

## What is here

| Path | Live URL | What it is |
|---|---|---|
| `d/dayevent.html` | <https://eonoe.github.io/ai-tech-lead/d/dayevent.html> | Coding Agents 101 workshop page (English) |
| `d/dayevent_es.html` | <https://eonoe.github.io/ai-tech-lead/d/dayevent_es.html> | Same page, Spanish |
| `index.html` | <https://eonoe.github.io/ai-tech-lead/> | Redirect stub → root domain |
| `apps-script/Code.gs` | — | Google Apps Script web app receiving signup POSTs |

Static HTML, no framework and no build step. The only external dependency is Google Fonts, loaded over HTTPS. Both workshop pages post to the same `SIGNUP_ENDPOINT` Apps Script URL, which the landing page also uses.

## Run it locally

Open `d/dayevent.html` in a browser. To also exercise the links between the landing page and the workshop pages, serve both repos under one origin:

```bash
mkdir -p /tmp/pagesroot
cp /path/to/eonoe.github.io/index.html /tmp/pagesroot/
ln -sfn /path/to/ai-tech-lead /tmp/pagesroot/ai-tech-lead
cd /tmp/pagesroot && python3 -m http.server 8765
```

Then open <http://localhost:8765/>.

## Deploy

GitHub Pages builds from `main` at the repo root and redeploys on its own after a merge.
