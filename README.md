# Taiwan Weather App

A realtime Taiwan weather app built while learning React Hooks.

## PWA

This project includes Progressive Web App support:

- `public/manifest.json` defines install metadata
- `src/index.js` registers the service worker
- GitHub Pages serves the built static files from the `gh-pages` branch

## Deployment

For this fork, GitHub Pages is published at:

`https://yogageek.github.io/learn-react-from-hook-realtime-weather-app`

Useful commands:

```bash
npm install
npm run build
npm run deploy
```

## Sunrise And Sunset Data

The app includes scripts to regenerate sunrise and sunset data when the upstream source changes:

```bash
npm run build:process-sunrise-sunset
npm run build:sunrise-sunset
```

If you use an API authorization key, place it in `.env`:

```bash
REACT_APP_API_AUTHORIZATION_KEY=CWB-***-***
```

## Branch Notes

- `main` is your current mainline
- `pwa` contains the PWA-related source changes
- `gh-pages` contains built static assets only
