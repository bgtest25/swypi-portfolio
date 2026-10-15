# Swypi: Full-Stack Social Platform

**Role:** Sole Developer & Architect  
**Timeline:** January 2026 - Present  
**Status:** Live in Production (iOS App Store)

---

## Overview

Swypi is a social media platform for content creators, featuring short-form video sharing, real-time interactions, live streaming, and an integrated creator economy. I designed, built, and deployed the entire platform solo, from mobile app to backend infrastructure.

---

## Technical Architecture

### Monorepo Structure
- **6 applications** managed via Turborepo for unified builds and shared tooling
- TypeScript throughout (100% type coverage, zero `any` types)
- Shared packages for common utilities, types, and configurations

### Applications Built

| App | Stack | Purpose |
|-----|-------|---------|
| Mobile | React Native (Expo) | Primary iOS app |
| API | NestJS | RESTful backend services |
| Web | Next.js | Creator profiles & public pages |
| Landing | Next.js | Marketing site with AI assistant |
| Admin | React | Internal moderation tools |
| RAG Assistant | LangChain | AI-powered customer support |

### Infrastructure
- **Database:** PostgreSQL with Row-Level Security (RLS) policies
- **Auth:** JWT-based authentication with secure session management
- **Real-time:** WebSocket subscriptions for live updates
- **Media:** Cloud storage for video/image assets
- **Hosting:** Railway (API), Vercel (web apps), EAS (mobile builds)
- **CI/CD:** Automated builds, linting, type-checking, and deployments

---

## Key Technical Achievements

### 1. Creator Economy System
Built a complete financial infrastructure supporting:
- In-app purchases via RevenueCat
- Virtual currency gifting between users
- Creator payout system with balance tracking
- Transaction audit logging for compliance

### 2. Real-Time Communication
- Voice/video calling in DMs (WebRTC-based)
- Live streaming infrastructure
- Push notifications with silent background updates
- Optimistic UI with automatic rollback on errors

### 3. Security & Trust
- Bot farm defense using behavioral analysis + CAPTCHA
- Rate limiting and abuse prevention
- Secure API design (no sensitive data in URLs, proper auth flows)
- Row-level security ensuring users only access their own data

### 4. AI Integration
- RAG-based customer support chatbot on landing page
- Vector embeddings for semantic search
- Context-aware responses trained on product documentation

### 5. E-commerce Integration
- Shopify Storefront API for merchandise sales
- Embedded store experience within the app
- Inventory sync and order management

---

## Development Practices

- **Migration-driven schema changes** (never manual database edits)
- **Type-safe database queries** with generated TypeScript types
- **Comprehensive error handling** with loading/empty/error states on all screens
- **Code quality gates:** ESLint, Prettier, Husky pre-commit hooks
- **Incremental commits** after each working feature

---

## Scale & Complexity

- **50+ database tables** with RLS policies
- **100+ API endpoints** across multiple domains
- **Native iOS features:** VoIP push notifications, background audio, deep linking
- **App Store approved:** Passed Apple review including VoIP entitlements

---

## Lessons Learned

1. **RLS from day one** prevents security debt accumulating
2. **Monorepo tooling** (Turborepo) dramatically improves DX for multi-app projects
3. **Optimistic UI** makes apps feel instant even with network latency
4. **Type generation** from database schema eliminates an entire class of bugs

---

## Technologies Used

**Frontend:** React Native, Expo, Next.js, React, TypeScript, TailwindCSS  
**Backend:** NestJS, Node.js, PostgreSQL, WebSockets  
**AI/ML:** LangChain, Vector Embeddings, RAG Architecture  
**Infrastructure:** Railway, Vercel, EAS, Supabase  
**Integrations:** RevenueCat, Shopify, WebRTC, Push Notifications  
**Tooling:** Turborepo, ESLint, Prettier, Husky, GitHub Actions

---

## Contact

This project demonstrates my ability to architect, build, and ship a production-grade platform independently. I'm happy to discuss technical decisions, trade-offs, and implementation details in an interview setting.

---

*This case study describes publicly available functionality. No proprietary code, API keys, or sensitive implementation details are included.*
