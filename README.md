# Next.js 14 Boilerplate

Table of Contents

-   [Getting Started](#getting-started)
-   [Project Structure](#project-structure)
-   [Best Practices for Using App Router](#best-practices-for-using-app-router)

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

## Naming Convention

**General Rule:**

-   JavaScript without JSX (JS): `.js`
-   JavaScript with JSX (JSX): `.jsx`
-   TypeScript without JSX (TS):` .ts`
-   TypeScript with JSX (TSX): `.tsx`

**File and Folder Naming Rule:**

-   Folder Name: folder name all in lowercase
-   File Name: file name when JSX is used Capitalize the first letter of each word

## Best Practices for Using App Router

### Utilize Server and Client Components

-   **Use Server Components** (`.tsx` by default) to keep your app fast and efficient.
-   **Use Client Components** (`'use client'` directive) only when interactivity is needed.

### Leverage Layouts and Nested Routing

-   Create multiple layouts to handle different parts of the app (e.g., authentication layout, dashboard layout).
-   Use nested routing to define sub-pages or sections within a layout.

### Data Fetching Strategies

-   Use `getServerSideProps`, `getStaticProps`, or `fetch` within Server Components to fetch data directly from the server.

### Performance Optimization

-   Use `React.Suspense` and `next/link` for lazy loading and prefetching.
-   Take advantage of automatic code splitting provided by Next.js.

### Error and Loading Handling

-   Create `error.tsx` and `loading.tsx` components within specific routes to handle errors and loading states elegantly.

## Learn More

To learn more about Next.js, take a look at the following resources:

-   [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
-   [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
