---
trigger: glob
description: Whenever working on Javascript files or UI designs invoke this rule
globs: *.js, *.css, *.html, *.ts, *.jsx
---

# Front‑End Engineering Guidelines
## Tech Stack
  - You are an expert in TypeScript, Node.js, Next.js App Router, React, Shadcn UI, Radix UI, and Tailwind CSS

## Code Style & Structure
  - Write concise, technical TypeScript; use **functional & declarative** patterns—no classes.
  - Prefer **iteration & modularization** over duplication.
  - Use descriptive variables with auxiliary verbs (e.g., `isLoading`, `hasError`).
  - **File layout**
    ```
    component.tsx # exported component
    subcomponents/ # related UI pieces
    lib/ # helpers & utilities
    static/ # assets
    types.ts # shared interfaces
    ```

## Naming
  - Directories: `lowercase-with-dashes` (e.g., `components/auth-wizard`).
  - Export components as **named exports**.
## TypeScript
  - Prefer **interfaces** over `type`.
  - Avoid `enum`; use object **maps** instead.
  - All components are **functional** with typed props.
## Syntax & Formatting
  - Use the `function` keyword for pure helpers.
  - Omit braces for simple one‑line conditionals.
  - Embrace **declarative JSX**.
## UI & Styling
  - Build UI with **Shadcn + Radix** primitives; style with **Tailwind**.
  - Implement **mobile‑first** responsive design.
## Performance
  - Default to **React Server Components**; minimize `use client`, `useEffect`, `setState`.
  - Wrap client components in `<Suspense>` with graceful fallbacks.
  - **Dynamically import** non‑critical components.
  - **Optimize images**: WebP format, explicit dimensions, `loading="lazy"`.
## URL State & Web Vitals
  - Manage URL parameters with **nuqs**.
  - Optimize **LCP, CLS, FID**.
## `use client` Rules
  - Reserve for small components needing browser‑only APIs.
  - **Never** use for data fetching or global state; prefer Next.js SSR patterns.
Refer to the official **Next.js documentation** for data fetching, rendering, and routing specifics.