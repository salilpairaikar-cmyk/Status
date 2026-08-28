# Production Status Board

## Run locally

```powershell
npm.cmd start
```

Open `http://localhost:3000` for the operator/admin sign-in and `http://localhost:3000/display` for the read-only displays.

## Render deployment

This repository includes `render.yaml`. It configures a Render Web Service with a persistent disk at `/var/data`; the application stores its SQLite database in `/var/data/production-board.db` when deployed.

Use a paid Render web-service plan: Render persistent disks are not available on free web services. Do not deploy the board publicly if its production information should remain private, because `/display` does not require login.
