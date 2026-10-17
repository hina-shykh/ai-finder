# AI Finder

AI Finder is a responsive directory for discovering useful AI tools across creative work, coding, writing, audio, and productivity.

- Live site: <https://aifinderr.netlify.app>
- Source repository: <https://github.com/hina-shykh/ai-finder>

## Features

- Browse 25 AI tools in six categories
- Search tools by name and filter by category or free/freemium availability
- Save and remove favorites; favorites persist in browser `localStorage`
- See each tool's pricing label and visit its official website
- Responsive layout for desktop and mobile

## Technologies

- React 19 with TypeScript/TSX
- Vite 7
- Tailwind CSS 4
- Lucide React icons
- Browser `localStorage` for favorites

This project is frontend-only. It does not require a database, backend, API key, or authentication.

## Run locally

Install Node.js 20.19 or newer, then run these commands from the project folder:

```bash
npm install
npm run dev
```

Vite prints the local development URL in the terminal.

## Build for production

```bash
npm run build
npm run preview
```

The production site is generated in `dist/`.

## Deploy from GitHub to Netlify

The included `netlify.toml` sets the build command to `npm run build` and the publish directory to `dist`. Connect the GitHub repository to Netlify and use those settings if Netlify does not detect them automatically.

## Main source files

- `src/App.tsx` — page structure, search, filters, favorites, and tool cards
- `src/data/tools.ts` — tool directory data and category definitions
- `src/index.css` — theme and responsive styling
- `src/main.tsx` — React entry point and error boundary
- `public/` — favicon, crawler rules, and Netlify route fallback
