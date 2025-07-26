# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

- `npm run dev` - Start development server with Turbopack for fast rebuilds
- `npm run build` - Build production application  
- `npm run start` - Start production server
- `npm run lint` - Run ESLint for code quality checks

## Tech Stack

- **Framework**: Next.js 15.4.4 with App Router
- **Language**: TypeScript with strict mode
- **Styling**: Tailwind CSS v4 with CSS custom properties
- **Fonts**: Geist Sans and Geist Mono via next/font
- **Linting**: ESLint with Next.js and TypeScript configs
- **Package Manager**: npm

## Architecture

This is a Next.js application using the App Router architecture with:

- **Server Components by default** - Components render on server unless explicitly made client-side
- **File-based routing** - Routes defined by folder structure in `src/app/`
- **TypeScript path mapping** - `@/*` maps to `src/*` for clean imports
- **CSS Custom Properties** - Theme colors defined as CSS variables with automatic dark mode
- **Modular design** - Planned structure for components, lib utilities, and API routes

## Project Structure

```
src/
├── app/                    # App Router pages and layouts
│   ├── layout.tsx         # Root layout with fonts and metadata
│   ├── page.tsx           # Homepage component
│   ├── globals.css        # Global styles and Tailwind imports
│   └── favicon.ico        # App icon
```

## Planned Architecture (from docs)

The application is designed to scale with:
- Route groups for marketing vs app pages: `(marketing)/` and `app/`  
- Component organization by domain: `components/ui/`, `components/marketing/`, `components/app/`
- Utility functions in `lib/` directory
- API routes in `app/api/` following REST conventions

## Development Notes

- Uses Turbopack in development for faster builds
- TypeScript strict mode enabled for better type safety
- Tailwind CSS v4 with new @theme directive for theming
- ESLint configured with Next.js and TypeScript recommended rules
- Dark mode support via CSS custom properties and `prefers-color-scheme`
- Font optimization with Geist font family loaded via next/font