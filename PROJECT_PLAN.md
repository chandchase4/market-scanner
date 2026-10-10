# Market Scanner — Project Blueprint

## Vision
Build a responsive workspace for finding market opportunities using configurable scanner filters. The supplied vision was incomplete ("A..."); audience, asset classes, and detailed workflows remain to be defined.

## Goals
- Provide a clear interface that works on desktop and mobile.
- Connect a suitable market data provider after requirements are defined.
- Support useful, configurable scanner filters and readable results.
- Keep the foundation understandable and easy to extend.

## Architecture
- `client/`: React application built with Vite and JavaScript.
- `client/src/App.jsx`: starter application interface.
- `client/src/App.css` and `index.css`: responsive styles and global defaults.
- Market data: TBD; provider access and licensing must be evaluated.
- Backend: TBD; add a server if credentials, persistence, or data processing require it.
- Deployment: TBD; Vite produces static assets in `client/dist/`.

## Decisions
- Start with JavaScript, as requested.
- Use plain CSS for the minimal interface; no UI framework is needed yet.
- Keep the initial dependency set small: React, React DOM, and Vite's development and lint tooling.
- Show an honest empty state until market data and scanner logic are implemented.
- Do not select a data provider or imply live results before requirements are settled.

## Roadmap
1. Initialize React, create a responsive starter, document setup, and verify the build.
2. Define target markets, scanner workflows, filter definitions, and results layout.
3. Select and connect market data, including loading and error states.
4. Implement scanner filters and results with meaningful validation.
5. Test supported devices, polish accessibility and performance, and deploy.

## Future Ecosystem
Trading journal, analytics, and ML apps. Integration boundaries will be defined as these projects take shape.

## TODOs
- Complete the product vision and identify the intended users.
- Choose asset classes, exchanges, refresh frequency, and delayed versus real-time data.
- Define initial filters, sorting, and result columns.
- Evaluate provider coverage, costs, licensing, and API limits.
- Decide whether accounts, saved scans, persistence, and a backend are needed.
- Add feature tests when scanner behavior is introduced.
- Select hosting and configure deployment.

## Current Status
Initialization complete (2026-10-10).
- Created the React + Vite JavaScript app in `client/` and installed dependencies with a committed-ready npm lockfile.
- Built a minimal, responsive Market Scanner interface with an explicit disconnected-data empty state.
- Removed Vite demo components, imagery, links, and template documentation.
- Added installation, development, build, and preview instructions in the root README.
- Added repository ignore rules for dependencies, build output, and local environment files.
- Verified `npm.cmd run build` and `npm.cmd run lint`: both passed.
- Installation audit reported zero vulnerabilities.
- Browser-based visual verification has not been performed.
- Market data, filters, backend, and deployment remain future work.
