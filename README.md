<div align="center">

# Shapline Industry

**TanStack Start · React 19 · Firebase · Cloudflare Workers**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-shapline--industry.vercel.app-black?style=flat-square&logo=vercel)](https://shapline-industry.vercel.app)
[![TypeScript](https://img.shields.io/badge/TypeScript-97.8%25-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-19.2-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev/)
[![Firebase](https://img.shields.io/badge/Database-Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)](https://firebase.google.com/)
[![Cloudflare Workers](https://img.shields.io/badge/Backend-Cloudflare%20Workers-F38020?style=flat-square&logo=cloudflare&logoColor=white)](https://workers.cloudflare.com/)
[![Deployed on Vercel](https://img.shields.io/badge/Deployed%20on-Vercel-black?style=flat-square&logo=vercel)](https://vercel.com/)

</div>

---

## Overview

Shapline Industry is a full-stack web application built on the cutting edge of the React ecosystem — **React 19**, **TanStack Start**, and **TanStack Router** for file-based routing, **Firebase Firestore** for real-time data, and **Cloudflare Workers** for serverless edge compute. The UI is powered by Shadcn/ui with Tailwind CSS 4, delivering a fast, type-safe, production-ready experience.

🌐 **Live:** [shapline-industry.vercel.app](https://shapline-industry.vercel.app)

---

## Tech Stack

| Layer | Technology |
|---|---|
| **Framework** | TanStack Start 1.167 |
| **Language** | TypeScript (97.8%) |
| **UI Library** | React 19.2 |
| **Router** | TanStack React Router 1.168 |
| **Styling** | Tailwind CSS 4.2 |
| **UI Components** | Shadcn/ui · 20+ Radix UI primitives |
| **Forms** | React Hook Form 7 + Zod 3.24 |
| **Data Fetching** | TanStack React Query v5 |
| **Charts** | Recharts 2.15 |
| **Database** | Firebase 12 (Firestore) |
| **Backend** | Cloudflare Workers (via Wrangler) |
| **Build Tool** | Vite 7.3 |
| **Package Manager** | Bun |
| **Deployment** | Vercel |

---

## Project Structure

```
shapline-industry/
├── src/                    # Application source code
│   ├── routes/             # TanStack Router file-based routes
│   ├── components/         # Reusable UI components (Shadcn/ui)
│   └── lib/                # Utilities, Firebase config, helpers
├── .vite/                  # Vite cache
├── vite.config.ts          # Vite + TanStack Start configuration
├── tsconfig.json           # TypeScript configuration
├── eslint.config.js        # ESLint rules
├── .prettierrc             # Prettier formatting config
├── components.json         # Shadcn/ui metadata
├── firebase.json           # Firebase project config
├── firestore.rules         # Firestore security rules
├── wrangler.jsonc          # Cloudflare Workers config
├── bunfig.toml             # Bun config
└── package.json
```

---

## Getting Started

### Prerequisites

- [Bun](https://bun.sh/) (primary package manager)
- Node.js 18+
- Firebase project with Firestore enabled
- Cloudflare account (for Workers)

### Installation

```bash
git clone https://github.com/Hamid-GenAI-Eng/shapline-industry.git
cd shapline-industry
bun install
```

### Environment Setup

Create a `.env` file in the root:

```env
VITE_FIREBASE_API_KEY=your-api-key
VITE_FIREBASE_AUTH_DOMAIN=your-auth-domain
VITE_FIREBASE_PROJECT_ID=your-project-id
VITE_FIREBASE_STORAGE_BUCKET=your-storage-bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your-sender-id
VITE_FIREBASE_APP_ID=your-app-id
```

### Run Locally

```bash
bun run dev
```

Opens at `http://localhost:3000`

---

## Scripts

| Command | Description |
|---|---|
| `bun run dev` | Start development server |
| `bun run build` | TypeScript check + production build |
| `bun run build:dev` | Dev-mode build |
| `bun run preview` | Preview production build locally |
| `bun run lint` | Run ESLint |
| `bun run format` | Format code with Prettier |

---

## Firebase & Cloudflare Setup

### Firestore

```bash
# Install Firebase CLI
npm i -g firebase-tools

# Login & initialize
firebase login
firebase init firestore

# Deploy security rules
firebase deploy --only firestore:rules
```

### Cloudflare Workers

```bash
# Install Wrangler CLI
npm i -g wrangler

# Login
wrangler login

# Run Workers locally
wrangler dev

# Deploy Workers
wrangler deploy
```

---

## Deployment

Frontend is deployed on **Vercel** with automatic CI/CD. Cloudflare Workers handle edge serverless functions independently via Wrangler.

```bash
# Deploy frontend
vercel --prod

# Deploy Workers
wrangler deploy
```

---

## Built By

**Hamid Saifullah** — Tech Lead at [Code Envision Technologies](https://github.com/Hamid-GenAI-Eng)

[![GitHub](https://img.shields.io/badge/GitHub-Hamid--GenAI--Eng-181717?style=flat-square&logo=github)](https://codeenvisiontechnologies.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-hamid--saifullah-black?style=flat-square&logo=vercel)](https://hamid-saifullah-portfolio-nexus.vercel.app)
