
# Architecture

This document outlines the architecture of the Alpha X App.

## Overview

The application is built using a modular architecture with a clear separation of concerns. It follows the principles of Domain-Driven Design (DDD) to ensure the codebase is scalable and maintainable.

## Components

- **Next.js App Router:** Handles routing and server-side rendering.
- **React Server Components (RSC):** Used for rendering components on the server.
- **React Client Components:** Used for interactive UI components.
- **Tailwind CSS:** For styling the application.
- **TypeScript:** For static typing.

## Directory Structure

```
/src
|-- /app
|   |-- /(marketing)
|   |   |-- page.tsx
|   |-- /app
|   |   |-- layout.tsx
|   |   |-- page.tsx
|   |-- /api
|   |   |-- /trpc
|   |   |   |-- /[trpc]
|   |   |   |   |-- route.ts
|-- /components
|   |-- /ui
|   |-- /marketing
|   |-- /app
|-- /lib
|   |-- /db
|   |-- /utils.ts
|-- /styles
|   |-- /globals.css
```

- **`/app/(marketing)`:** Marketing pages (e.g., landing page, pricing).
- **`/app/app`:** Authenticated application pages.
- **`/app/api`:** API routes.
- **`/components`:** Reusable components.
- **`/lib`:** Utility functions and database access.
- **`/styles`:** Global styles.
