# LibreChat Custom Deployment

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/template/v9QL5u?referralCode=0l6gRB)

This is a customized version of LibreChat with enhanced Railway deployment support.

## Quick Deploy
1. Click the "Deploy on Railway" button above
2. Configure your environment variables
3. Wait for the deployment to complete

## Environment Variables
Required variables:
- `MONGODB_URI` (auto-filled by Railway)
- `CREDS_KEY` (random string for encryption)
- `CREDS_IV` (16-char random string)
- `JWT_SECRET` (random string)
- `VOLUME_SIZE=1024`
- `STORAGE_PATH=/data`

## Keeping Updated
This repository is a fork of [danny-avila/LibreChat](https://github.com/danny-avila/LibreChat). To keep it updated:

1. Sync with upstream:
```bash
git fetch upstream
git merge upstream/main
git push origin dev
```

2. Railway will automatically redeploy when changes are pushed to the dev branch.

## Customization
Make your customizations in the `dev` branch. Railway will automatically deploy changes when you push to this branch.
