# Frontend Documentation

## Executive Summary

This component is a Next.js frontend (React) scaffold for the term-insurance-chatbot. It serves the user interface and static assets, and communicates with the backend over HTTP.

## Architecture Overview

- The frontend is built with Next.js (App Router) and React. Static assets live in `public/` and pages are under `src/app/`.
- The app can be run in development with Next's development server and built for production with `next build`.

## Technology Stack

- Next.js 15.5.4
- React 19.1.0
- Tailwind CSS (v4) for styling
- TypeScript for type safety (dev dependency)

## Getting Started

1. cd into `frontend`
2. Install dependencies: `npm install`
3. Development server: `npm run dev` (this runs `next dev --turbopack`)
4. Build for production: `npm run build`
5. Start built app: `npm run start`

## Scripts

- `npm run dev` - Starts Next.js in development mode (with Turbopack)
- `npm run build` - Builds the production assets
- `npm run start` - Starts the production server
- `npm run lint` - Runs ESLint

## Configuration

- Environment variables can be provided at runtime or via `.env` files. Typical variables:
  - NEXT_PUBLIC_API_BASE - Base URL for backend API (e.g., `http://localhost:8000`)

## Dependencies

See `package.json` for exact versions. Key dependencies:

- next, react, react-dom, tailwindcss, typescript (dev)

## Change History

### 2025-09-27 - v0.1 - FEATURE

**Components Affected**: frontend
**Summary**: Added frontend documentation following repository template.
**Details**:

- Documented scripts, dependencies, and basic run instructions.
  **Breaking Changes**: None
  **Migration Notes**: None

---

## Troubleshooting

- If styling or Tailwind classes don't apply, ensure Tailwind is installed and `globals.css` imports the Tailwind directives.
- If API requests fail during development, verify `NEXT_PUBLIC_API_BASE` points to the running backend.

## Contributing

When adding pages or components, update this doc with any new build steps or environment requirements.
