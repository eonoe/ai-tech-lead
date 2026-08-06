# ai-tech-lead

The Google Apps Script that collects signups, plus redirect stubs for URLs this repo used to serve.

**The pages moved.** They all live in [eonoe/eonoe.github.io](https://github.com/eonoe/eonoe.github.io) now — edit them there, not here.

| Old URL | Redirects to |
|---|---|
| `/ai-tech-lead/` | <https://eonoe.github.io/course/> — Tech Lead 2.0 |
| `/ai-tech-lead/d/dayevent.html` | <https://eonoe.github.io/> — Coding Agents 101, now the landing page |
| `/ai-tech-lead/d/dayevent_es.html` | <https://eonoe.github.io/es.html> — the Spanish workshop page |

GitHub Pages cannot serve a real 301, so each stub is a `<meta refresh>` plus a script that carries the URL hash across, so shared `#get` and `#pricing` links still land on the right anchor.

## apps-script/

`Code.gs` is a Google Apps Script web app deployed at the `SIGNUP_ENDPOINT` URL the pages POST to. It is not deployed from this repo — see `apps-script/README.md`. This is the only thing here that is still edited.
