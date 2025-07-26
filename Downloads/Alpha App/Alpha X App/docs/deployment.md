
# Deployment

This document describes the deployment process for the Alpha X App.

## Vercel

The application is deployed on Vercel. The deployment is automated through a Git integration.

### Steps

1. **Push to `main` branch:** A new deployment is automatically triggered.
2. **Vercel builds the project:** It installs dependencies and builds the Next.js app.
3. **The app is deployed:** The new version is available at the production URL.

## Environment Variables

The following environment variables need to be set on Vercel:

- `DATABASE_URL`
- `NEXTAUTH_URL`
- `NEXTAUTH_SECRET`

These variables are stored securely in the Vercel project settings.
