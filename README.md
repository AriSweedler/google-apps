# google-apps

Google requires every app that uses Google sign-in to have a public homepage and privacy policy URL on its OAuth consent screen. This repo hosts those pages for Ari's Google apps at [google-apps.sweedler.com](https://google-apps.sweedler.com).

| App | Homepage | Privacy policy |
| --- | --- | --- |
| Ari's Calendar Assistant | [/app/aris-calendar-assistant/](https://google-apps.sweedler.com/app/aris-calendar-assistant/) | [/app/aris-calendar-assistant/privacy-policy/](https://google-apps.sweedler.com/app/aris-calendar-assistant/privacy-policy/) |

GitHub Pages serves `main` as plain HTML. Cloudflare DNS points `google-apps.sweedler.com` at `arisweedler.github.io` with its proxy off, so GitHub can issue the HTTPS certificate.

To add an app, create `app/<name>/index.html` and `app/<name>/privacy-policy/index.html`, link it from the root `index.html`, and add a row above.
