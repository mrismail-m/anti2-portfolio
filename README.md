# anti2 — Static Portfolio Terminal

Minimalist Black & White dashboard with Green / Red accents for real-time tracking of `anti2` algorithmic paper-trading on Appwrite Cloud.

## Features
- **Pure Black & White**: High-contrast dark theme `#000000` with mono typography (JetBrains Mono).
- **Green & Red Highlights**: Dynamic P&L coloring strictly for positive and negative values.
- **Direct Appwrite Cloud Sync**: Reads directly from Appwrite Cloud DB (`current_portfolio` and `trades` collections).
- **Real-Time Streaming Mark Price**: Fetches live tick prices from Binance to calculate live unrealized P&L in real time.
- **Zero Server Compute Overhead**: 100% static client-side web application — 0 impact on Appwrite Function execution quota.

## Deployment to Vercel

### Option 1: Vercel CLI
From this folder:
```bash
cd web
vercel
```
When prompted, select default settings. Deploy to production with:
```bash
vercel --prod
```

### Option 2: Push to GitHub & Import to Vercel
1. Push this repository (or just the `web` folder) to GitHub.
2. In the Vercel Dashboard, click **Add New Project** -> **Import Git Repository**.
3. Set the Root Directory to `web` (or root if deploying the whole repo).
4. Framework Preset: **Other** (Static HTML).
5. Click **Deploy**.
