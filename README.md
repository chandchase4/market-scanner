# Market Scanner

A responsive React starter for a market scanner. Market data and scanning logic are planned; the current interface contains no live data.

## Requirements

- Node.js 22.12+ (or 20.19+)
- npm

## Install and develop

```sh
cd client
npm install
npm run dev
```

Open the local URL printed by Vite. On Windows, if PowerShell blocks `npm.ps1`, use `npm.cmd` in place of `npm`.

## Checks and production build

Run these commands inside `client/`:

```sh
npm run lint
npm run build
npm run preview
```

The build is written to `client/dist/`. Preview serves that build locally; it is not a production server.

## Project layout

- `client/`: React application, Vite configuration, and dependencies.
- `PROJECT_PLAN.md`: living blueprint, decisions, and next steps.

Market data, backend services, and deployment are not configured yet. Never place private API credentials in browser code or Vite environment variables exposed to the client.
