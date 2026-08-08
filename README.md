# ai-tech-lead

Redirect stubs. Nothing here is edited any more.

The site moved to [eonoe/eonoe.github.io](https://github.com/eonoe/eonoe.github.io) — pages and the Apps Script signup backend both. This repo exists only so the URLs it used to serve keep working.

| Old URL | Redirects to |
|---|---|
| `/ai-tech-lead/` | <https://eonoe.github.io/course/> — Tech Lead 2.0 |
| `/ai-tech-lead/d/dayevent.html` | <https://eonoe.github.io/> — Coding Agents 101, now the landing page |
| `/ai-tech-lead/d/dayevent_es.html` | <https://eonoe.github.io/es.html> — the Spanish workshop page |

GitHub Pages cannot serve a real 301, so each stub is a `<meta refresh>` plus a script that carries the URL hash across, so shared `#get` and `#pricing` links still land on the right anchor.

Do not delete this repo or turn off its Pages setting — the redirects go with it.
