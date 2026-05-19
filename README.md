# Multi-D-Infra (PropOS) — Showcase

> ⚠️ This is a **public showcase repository**. Source code is proprietary and maintained in a private repository. All rights reserved — Haley Ann Bird.

---

A multi-role, AI-driven property management platform for owners, contractors, tenants, and guests. The adaptive UI morphs based on the active user role, providing tailored dashboards, tools, and workflows for residential and commercial property operations.

## What Was Built

### Core Architecture
- **Full-stack TypeScript** — React 19 frontend + Node/Express backend, single-port deployment
- **Neon Postgres** via Drizzle ORM — type-safe schema, migrations via `drizzle-kit push`
- **Postgres-backed sessions** — `express-session` + `connect-pg-simple`, stateless-compute compatible
- **WebSocket layer** — real-time messaging and live updates via `ws`
- **Vite build pipeline** — HMR in dev, static assets served by Express in production

### Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 19, TypeScript, Tailwind CSS, Vite |
| Routing | Wouter |
| UI System | Radix UI / shadcn/ui, Framer Motion, Lucide |
| Charts | Recharts |
| Backend | Node.js, Express, TypeScript |
| Database | PostgreSQL (Neon) + Drizzle ORM |
| Auth | Passport.js + express-session |
| Real-time | WebSockets (ws) |
| CI | GitHub Actions (typecheck + build on every PR) |

---

## Features

### Role-Based Adaptive UI
The interface fully morphs across four user roles — no shared generic dashboard:
- **Owner** — Portfolio overview, property grid, AI predictive marketing campaigns, occupancy forecasting, active project boards
- **Contractor** — Task management, project boards, daily work logs, scheduling
- **Tenant** — Property browsing, booking confirmations, service requests, community announcements
- **Guest** — Property discovery, listing detail views, booking flow

### Platform Capabilities
- 📊 **Analytics** — Performance metrics, occupancy trends, conversion dashboards
- 📣 **AI Marketing** — Predictive campaigns with demographic targeting and conversion tracking
- 🏘️ **Property Management** — Listings, CRM, lead capture, listing detail views
- 📄 **Documents & Legal** — Document management and legal workflows
- 💬 **Messaging** — Built-in real-time messaging system
- 📱 **Mobile-Ready** — Bottom navigation and fully responsive layout

---

## Project Structure (overview)

```
client/          # React frontend — components, pages, hooks, role context
server/          # Express backend — API routes, auth, storage interface
shared/          # Shared Drizzle schema + Zod types (private)
script/          # Build scripts
docs/            # Internal documentation (private)
```

---

## Status

- ✅ CI pipeline active (GitHub Actions — typecheck + build)
- ✅ Environment config standardized (`.env.example`)
- 🔄 Deployment migration in progress (Replit → Fly.io / Render evaluation)
- 🔄 IP protection and licensing finalization in progress

---

## Legal

**© 2025–2026 Haley Ann Bird. All rights reserved.**

This showcase repository contains descriptive information only. No source code is included or licensed for reuse. The platform, its architecture, design, and implementation are proprietary works owned exclusively by Haley Ann Bird.

Unauthorized reproduction, distribution, or derivative use of any concepts, designs, or systems described herein is prohibited.

Contact: heyhaleybird@gmail.com
