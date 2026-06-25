# Musaix Engine

A desktop application for music analysis and audio pipeline management, built with Electron. Features a dark, glass-panel UI with real-time system metrics, Spotify integration, and a modular audio pipeline.

## Tech Stack

- **Shell**: Electron (Node.js)
- **UI**: HTML + Tailwind CSS (CDN), Material Symbols icons
- **Backend**: Python (via `main.py`)
- **Database**: Supabase (PostgreSQL)
- **APIs**: Spotify Web API + Web Playback SDK, Last.fm

## Project Structure

```
desktop-chatbot-ui/
├── index.js                    # Electron main process
├── preload.js                  # Context bridge
├── main.py                     # Python entry point
├── musaix-stitch/
│   └── code/
│       ├── config.js           # API credentials (gitignored)
│       ├── dashboard-overview.html
│       ├── audio-pipeline-*.html
│       ├── cognition-engine-setup.html
│       ├── spotify-analysis.html
│       ├── creative-track-building.html
│       ├── external-integrations.html
│       ├── production-analytics.html
│       ├── system-settings.html
│       └── design-system.json
└── env.local                   # Local credentials (gitignored)
```

## Setup

1. **Install dependencies**
   ```bash
   npm install
   ```

2. **Configure credentials** — copy the values into `musaix-stitch/code/config.js`:
   ```js
   const SPOTIFY_CLIENT_ID      = '...';
   const SPOTIFY_CLIENT_SECRET  = '...';
   const LASTFM_API_KEY         = '...';
   const SUPABASE_URL           = '...';
   const SUPABASE_ANON_KEY      = '...';
   const SUPABASE_PUBLISHABLE_KEY = '...';
   ```

3. **Run**
   ```bash
   npm start
   ```

## Supabase

- Project: **Integrate React UI Deployment**
- Region: `us-east-2`
- Auth providers enabled: Email, GitHub, Google, Spotify

## Spotify App

- App: **Musaix Pro** (`musaix.com`)
- Redirect URI: `https://musaix-analyzer-s73rl.replit.app/`
- APIs: Web API, Web Playback SDK

## Security

`config.js` and `env.local` are gitignored — never commit credentials. The Supabase anon key is safe for client-side use; never expose the service role key.
