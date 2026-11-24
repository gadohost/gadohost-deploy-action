# GadoHost Auto-Deploy GitHub Action

Trigger automatic zero-downtime deployments on [GadoHost Cloud](https://gadohost.com) every time you push to your `main` branch.

## Setup (30 Seconds)

1. Open your Node.js app in [gadohost.com/dashboard](https://gadohost.com/dashboard) and copy your **Git Deploy Webhook URL**.
2. In your GitHub repository, go to **Settings -> Secrets and variables -> Actions -> New repository secret**.
3. Create a secret named **`GADOHOST_WEBHOOK_URL`** and paste your webhook URL.
4. Copy `.github/workflows/gadohost-deploy.yml` into your repository.

Every push to `main` will now automatically pull, build, and reload your PM2 process on GadoHost with zero downtime.

## Documentation

- [GadoHost Git Auto-Deploy Guide](https://gadohost.com/docs)
- [GadoHost Node.js Cloud](https://gadohost.com/nodejs-hosting)
