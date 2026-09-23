# tasfica

Live site: **Starslip**, a warp-speed starfield. Served at the domain root.

The previous invitation page is still in git at [`invite.html`](invite.html) (`/invite`).

## Hosting

Live on **Firebase Hosting** (project `tasfica`) 

- https://tasfica.com
- https://tasfica.ca
- https://tasfica.web.app

Both apex domains serve this same git. `www` redirects to apex.

### Deploy on every git push

Primary path: Grok Bot routine **tasfica Git push → Firebase** (webhook). Add a GitHub repo webhook for `push` to that routine’s URL (same pattern as emciix).

Optional: set repo secret `FIREBASE_TOKEN` (`firebase login:ci`) so `.github/workflows/firebase-hosting.yml` can deploy from Actions too.

## Run locally

```bash
python3 -m http.server 8080
```

## Map

| Surface | Job |
|---|---|
| tasfica.com / tasfica.ca | Starslip |
| emciix.com | Player, light home |
| emciix.com/game/play | Game start page |
