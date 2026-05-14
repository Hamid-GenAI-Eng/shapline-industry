# Shapline Industry

A modern, full-stack industrial web application built with **TanStack Start**, **React 19**, and **TypeScript** — featuring a component-driven UI, real-time Firestore backend, and serverless Cloudflare Workers compute. Deployed on Vercel.

🌐 **Live:** [shapline-industry.vercel.app](https://shapline-industry.vercel.app)

---

## Tech Stack

| Layer | Technology |
|---|---|
| **Framework** | TanStack Start + React 19.2.0 |
| **Language** | TypeScript 5.x |
| **Router** | TanStack React Router 1.168.0 |
| **State / Data** | TanStack Query 5.83.0 |
| **Styling** | Tailwind CSS 4.2.1 |
| **UI Components** | shadcn/ui (Radix UI) |
| **Forms** | React Hook Form + Zod |
| **Charts** | Recharts |
| **Database** | Firebase Firestore |
| **Serverless** | Cloudflare Workers (Wrangler) |
| **Build Tool** | Vite 7.3.1 |
| **Package Manager** | Bun |
| **Deployment** | Vercel |

---

## Features

- **Type-safe routing** via TanStack Router with file-based route definitions
- **Server-side rendering** support through TanStack Start
- **Real-time data** with Firebase Firestore integration
- **Edge compute** via Cloudflare Workers for low-latency serverless logic
- **Rich component library** — 20+ Radix UI primitives, carousels, resizable panels, toast notifications
- **Form validation** with React Hook Form + Zod schema validation
- **Data visualization** with Recharts
- **Code quality** enforced via ESLint + Prettier

---

## Getting Started

### Prerequisites

- [Bun](https://bun.sh) >= 1.x
- [Node.js](https://nodejs.org) >= 20.x (for tooling compatibility)
- A Firebase project with Firestore enabled
- A Cloudflare account (for Workers deployment)

### Installation

```bash
# Clone the repository
git clone https://github.com/Hamid-GenAI-Eng/shapline-industry.git
cd shapline-industry

# Install dependencies
bun install
```

### Environment Setup

Create a `.env` file in the root directory and add your Firebase configuration:

```env
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_storage_bucket
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

### Development

```bash
bun run dev
```

The app will be available at `http://localhost:3000`.

---

## Scripts

| Command | Description |
|---|---|
| `bun run dev` | Start development server |
| `bun run build` | Production build (type-check + Vite) |
| `bun run build:dev` | Development mode build |
| `bun run preview` | Preview production build locally |
| `bun run lint` | Run ESLint |
| `bun run format` | Format code with Prettier |

---

## Project Structure

```
shapline-industry/
├── src/                    # Application source code
│   ├── components/         # Reusable UI components (shadcn/ui + custom)
│   ├── routes/             # TanStack Router file-based routes
│   ├── lib/                # Utilities, Firebase config, helpers
│   └── ...
├── .vite/                  # Vite cache
├── vite.config.ts          # Vite bundler configuration
├── tsconfig.json           # TypeScript configuration
├── eslint.config.js        # ESLint rules
├── .prettierrc             # Prettier formatting rules
├── components.json         # shadcn/ui components metadata
├── firebase.json           # Firebase project configuration
├── firestore.rules         # Firestore security rules
├── wrangler.jsonc          # Cloudflare Workers configuration
└── bunfig.toml             # Bun configuration
```

---

## Deployment

### Vercel (Frontend)

The app is configured for Vercel deployment. Push to `main` to trigger automatic deployments.

```bash
# Manual deploy via Vercel CLI
vercel --prod
```

### Cloudflare Workers (Backend)

```bash
# Deploy Workers via Wrangler
bunx wrangler deploy
```

### Firestore Rules

Deploy Firestore security rules:

```bash
firebase deploy --only firestore:rules
```

---

## Key Dependencies

```json
{
  "react": "19.2.0",
  "@tanstack/react-start": "1.167.14",
  "@tanstack/react-router": "1.168.0",
  "@tanstack/react-query": "5.83.0",
  "tailwindcss": "4.2.1",
  "firebase": "12.12.1",
  "react-hook-form": "7.71.2",
  "zod": "3.24.2",
  "recharts": "2.15.4",
  "date-fns": "4.1.0"
}
```

---

## Contributing

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'feat: add your feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## Author

**Hamid Saifullah** — Tech Lead at [Code Envision Technologies](https://codeenvisiontechnologies.com)

- GitHub: [@Hamid-GenAI-Eng](https://github.com/Hamid-GenAI-Eng)
- Portfolio: [hamid-saifullah-portfolio-nexus.vercel.app](https://hamid-saifullah-portfolio-nexus.vercel.app)

---

*Built with TanStack Start · Powered by Firebase & Cloudflare · Deployed on Vercel*
