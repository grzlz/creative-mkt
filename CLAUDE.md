# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- **Start development server**: `npm run dev`
- **Build for production**: `npm run build`
- **Preview production build**: `npm run preview`
- **Format code**: `npm run format` (prettier)
- **Lint code**: `npm run lint` (prettier + eslint)

## Project Architecture

This is a **SvelteKit 5** project with **TailwindCSS 4** for styling.

### Key Structure
- `src/routes/` - File-based routing (SvelteKit convention)
- `src/lib/` - Shared components and utilities (accessible via `$lib` alias)
- `src/lib/assets/` - Static assets like icons
- `src/app.html` - HTML template
- `src/app.css` - Global styles with TailwindCSS

### Technology Stack
- **Framework**: SvelteKit 5 with Svelte 5 (uses `$props()` syntax)
- **Styling**: TailwindCSS 4 (configured in `vite.config.js`)
- **Build Tool**: Vite 7
- **Package Manager**: npm
- **Code Quality**: ESLint + Prettier

### Important Notes
- Uses **JavaScript** (not TypeScript) - note `jsconfig.json` instead of `tsconfig.json`
- Svelte 5 syntax with `$props()`, `{@render children?.()}` patterns
- TailwindCSS is integrated via Vite plugin, not separate config file
- Auto-adapter configured for deployment flexibility