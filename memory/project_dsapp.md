---
name: dsapp — project context
description: Dance school app project overview, team, tech stack, and constraints
type: project
---

App for a dance school "Танцевальная команда КИД" (Belgorod). Client is Dima (owner) + Kristina (admin/wife). No payment from client, no deadlines — win-win-win learning project.

**Team:**
- Anzor: BA, architect, DevOps, AI operator → directs Claude on frontend
- Claude: writes React frontend (SPA)
- Student: Java + Spring backend

**Tech stack:**
- Frontend: React SPA
- Backend: Java + Spring (REST API)
- Auth: JWT (simple, no OAuth on v1)
- DB: Postgres
- Infra: VPS + nginx + docker
- Optional later: Telegram Mini App (same SPA, just surfaced via bot)

**Approach:** iterative. Start with one core feature (payment tracking), validate on one group, then grow.

**Constraints:**
- School works with cash only (no online payments in MVP)
- Payment marked as paid/unpaid manually by admin
- No public schedule (competitive sensitivity)
- Simple UI is critical — Kristina tried "Мой класс" and found it too complex

**Why:** detailed business processes documented in `src/main/resources/business_analysis_kickoff.md`
