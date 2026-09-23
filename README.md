# 🎈 Bambiboo — Preschool & Daycare Web Application

Welcome to the official repository for **Bambiboo**, a modern, high-performance web platform for early childhood education, daycare, and enrichment programmes.

Built with **TanStack Start**, **React 19**, **Vite**, and **Tailwind CSS v4**, this application provides a fast, responsive, and SEO-optimized experience for parents, guardians, and educators.

---

## 🚀 Tech Stack Overview

| Category | Technology |
|---|---|
| **Framework & SSR** | [TanStack Start](https://tanstack.com/router) + [React 19](https://react.dev/) + [Nitro Engine](https://nitro.unjs.io/) |
| **Routing** | [TanStack Router](https://tanstack.com/router) (File-based, Type-safe routing) |
| **Styling & UI** | [Tailwind CSS v4](https://tailwindcss.com/) + [Radix UI Primitives](https://www.radix-ui.com/) + [shadcn/ui](https://ui.shadcn.com/) |
| **Icons & Visuals** | [Lucide React](https://lucide.dev/) + [Embla Carousel](https://www.embla-carousel.com/) + [Recharts](https://recharts.org/) |
| **State & Data** | [TanStack React Query](https://tanstack.com/query) |
| **Form Handling** | [React Hook Form](https://react-hook-form.com/) + [Zod Validation](https://zod.dev/) |
| **Build & Tooling** | [Vite 8](https://vitejs.dev/) + TypeScript 5.8 + ESLint + Prettier |

---

## ✨ Key Features

- 🎒 **Comprehensive Programmes Hub**: Dedicated pages for Parent & Toddler, Playgroup, Nursery, LKG, UKG, Daycare, and Hobby Center.
- 🎨 **Beyond Academics**: Information on Arts, Music, Yoga, Festivals, and Field Trips.
- 🏫 **Parents Portal**: Admission guidelines, curriculum overview, daily schedules, safety protocols, transport details, and FAQs.
- 💡 **Interactive Components**:
  - **Programme Finder**: Quick filtering for parents based on child age/needs.
  - **Daily Rhythm Explorer**: Interactive timeline showing child schedules.
  - **Admission Portal Modal**: Embedded multi-step application form with validation.
  - **Blog & TOC**: Articles, readiness guides, and category filtering.
- 📱 **Responsive Design & Accessibility**: Fully mobile-optimized with accessible Radix UI primitives and custom theme mood capabilities.
- 🔍 **SEO & Performance**: Server-side rendering (SSR), dynamic XML sitemap generation (`/sitemap.xml`), and fast client hydration.

---

## 📁 Project Structure

```text
bambiboo-main/
├── public/                 # Static assets, logos, and images
├── src/
│   ├── assets/             # Images and design assets
│   ├── components/
│   │   ├── site/           # Domain-specific components (AdmissionForm, Header, Footer, etc.)
│   │   └── ui/             # Reusable UI primitives (Dialog, Button, Input, Accordion, etc.)
│   ├── hooks/              # Custom React hooks
│   ├── lib/                # Utilities, helpers, and error handling wrappers
│   ├── routes/             # File-based routes (TanStack Start)
│   │   ├── __root.tsx      # Root application shell & layout
│   │   ├── index.tsx       # Homepage
│   │   ├── about.tsx       # About Us page
│   │   ├── programmes.*    # Programme routes
│   │   ├── parents.*       # Parent resource routes
│   │   ├── world.*         # Campus & facilities routes
│   │   ├── beyond.*        # Beyond academics routes
│   │   └── blogs.*         # Blog engine routes
│   ├── routeTree.gen.ts    # Auto-generated route tree (Do not edit manually)
│   ├── router.tsx          # TanStack Router instance setup
│   ├── server.ts          # SSR server entry and error page handler
│   ├── start.ts           # Hydration & client entry point
│   └── styles.css          # Global Tailwind CSS styles
├── package.json            # Dependencies and scripts
├── vite.config.ts          # Vite & TanStack Start build configuration
└── tsconfig.json           # TypeScript configuration
```

---

## 🛠️ Getting Started

### Prerequisites

Make sure you have Node.js (v18 or higher) and `npm` installed.

```bash
node -v
npm -v
```

### Installation

1. Clone or navigate to the project directory:
   ```bash
   cd bambiboo-main
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

### Running Development Server

To start the development server:

```bash
npm run dev
```

*Note for Windows PowerShell users:* If PowerShell script execution restrictions prevent `npm` from running directly in PowerShell, execute via CMD:
```bash
cmd /c npm run dev
```

The application will be available at **`http://localhost:8080/`**.

---

## 📜 Available Scripts

| Script | Command | Description |
|---|---|---|
| `dev` | `npm run dev` | Starts Vite dev server with hot module reloading (HMR). |
| `build` | `npm run build` | Builds production bundle with Nitro SSR server. |
| `build:dev` | `npm run build:dev` | Builds development-mode production artifact. |
| `preview` | `npm run preview` | Runs local server preview of the production build. |
| `lint` | `npm run lint` | Runs ESLint for code quality verification. |
| `format` | `npm run format` | Formats project code using Prettier. |

---

## 📌 Development Guidelines

- **Routing**: Routes are defined in `src/routes/` via file-based conventions. The route tree file `src/routeTree.gen.ts` is generated automatically by TanStack Router during development; do not modify it manually.
- **Lovable Integration**: This repository syncs with Lovable. Avoid force-pushing or rewriting published Git history to ensure project history integrity.

---

## 📄 License

Internal / Proprietary project for Bambiboo Preschool & Daycare. All rights reserved.
