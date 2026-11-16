<h1 align="center">Eliud Maina</h1>
<h3 align="center">Full-Stack Developer & Cybersecurity Specialist</h3>

<p align="center">
  <i>Building production-grade software, then breaking it to make sure no one else can</i>
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/eliud-maina-73b9691b7/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:meliud61@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <a href="https://eliudm.github.io/"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <img src="https://img.shields.io/badge/CEH-ECC2096578341-red?style=for-the-badge" />
</p>

<p align="center">⭐ From <b>Nairobi, Kenya</b> · Open to full-stack & security-focused opportunities</p>

---

### 🎯 Focus

I work across the full stack **and** the security stack — designing systems that hold up under real load, then pentesting them to find where they don't. That covers ERP and clinic SaaS platforms handling money and PII, a production Android POS app, and offensive-security tooling for mobile and network targets. Same mindset either way: assume the naive version is wrong, and prove it.

- 🏗️ **Application engineering** — NestJS/Next.js, TypeScript, React Native, concurrency-safe backends, event-driven systems
- 🔐 **Offensive security** — mobile & network penetration testing tooling, reconnaissance scripting, CEH-aligned methodology
- 💳 **Fintech & compliance integration** — M-Pesa Daraja STK Push, KRA eTIMS, payment idempotency, Africa's Talking SMS/WhatsApp
- 📱 **Mobile** — Expo/React Native offline-first apps; Kotlin/Jetpack Compose on clean architecture

---

### 🏆 Flagship Projects

#### Nexora ERP
*Full-featured, self-hosted ERP for Kenyan SMEs* — private repo

Fifteen production modules end to end, covering every core business function:

| Module | Highlights |
|---|---|
| **Sales & Invoicing** | Quotations → invoices → credit notes; recurring billing; customer statements; aged receivables |
| **Point of Sale** | Full POS terminal, cash/M-Pesa/credit/split payments, shift management, reconciliation |
| **Accounting** | Chart of accounts, double-entry journal entries, bank reconciliation, period close |
| **Financial Reports** | P&L, balance sheet, trial balance, cash flow, VAT return export for KRA iTax |
| **Inventory** | Products, warehouses, stock movements, stocktake, transfers, wastage tracking |
| **Procurement** | Suppliers, RFQs, purchase orders, GRN, vendor bills, purchase returns |
| **HR & Payroll** | Employees, PAYE (KRA bands), NHIF/NSSF, payslips, leave, attendance, appraisals |
| **CRM** | Lead pipeline, stage tracking, conversion analytics |
| **Messaging** | SMS & WhatsApp campaigns via Africa's Talking, automated invoice reminders |
| **Analytics** | 10 dashboards — sales trends, POS performance, pipeline funnel, expense breakdown |
| **eTIMS / KRA** | Real-time invoice submission, BullMQ async queue, QR codes, exponential-backoff retry |
| **Budget & MRP** | Budget vs actual reports, bills of materials, work orders |
| **AI Insights** | Stock alerts, payment risk flags, top-customer detection |
| **Help & Support** | 55-article knowledge base (8 categories), support ticket system with threaded replies |

- M-Pesa Daraja STK Push with callback handling, pending-payment queueing, and manual reconciliation fallback
- Multi-role JWT auth (ADMIN, ACCOUNTANT, SALES_USER, INVENTORY_MANAGER, HR_MANAGER, PROCUREMENT_OFFICER)
- Docker Compose for local dev; Nginx reverse proxy + SSL for production
- **Tech stack:** NestJS · TypeScript · Prisma · PostgreSQL · Redis · BullMQ · React 19 · Ant Design · Vite · TanStack Query · Recharts

---

#### Nexora POS
*Standalone Android Point of Sale for Kenyan businesses — works 100% offline* — private repo

A complete POS app with no server dependency. All data lives in SQLite on the device.

- **POS Terminal** — split-panel product grid + live cart, cash/M-Pesa/credit/split payments, hold/park sales, item & order discounts
- **M-Pesa Integration** — Daraja STK Push (auto-prompts customer's phone); manual entry fallback; confirmation code recording
- **Receipt Sharing** — post-sale WhatsApp and SMS delivery via Africa's Talking; Bluetooth and USB thermal printer support
- **Inventory** — product variants (size/colour with per-variant prices), stock tracking, low-stock alerts, suppliers, purchase orders, stocktake, wastage recording
- **Customers & Loyalty** — credit accounts, loyalty points (earn/redeem), layaway (deposit + instalment payments), customer statements
- **Quotations** — create, share as PDF, convert to sale
- **Reports & Analytics** — daily/weekly/monthly revenue, profit/loss (COGS), VAT report, cash drawer reconciliation, visual analytics (revenue trend, peak hours, payment mix, top products, category performance, cashier leaderboard)
- **Expenses** — log outgoings by category for net profit calculation
- **Multi-User** — cashier and admin roles, each with a 4-digit PIN; all sales tracked per cashier
- **eTIMS Ready** — VAT tracking and KRA PIN field prepared for eTIMS integration
- **Help & Support** — 111-article in-app FAQ across 11 sections (Getting Started, POS, Inventory, Customers, Reports, Printing, M-Pesa, eTIMS, Data & Backup, Troubleshooting, Tips & Tricks)
- **Google Play Billing** — KES 600/month subscription via RevenueCat
- **Tech stack:** Expo SDK 58 · React Native 0.88 · Expo Router · React Native Paper · expo-sqlite (WAL mode) · TanStack Query v5 · react-native-gifted-charts · TypeScript · EAS Build

---

#### MusicPlayer
*Production-grade Android music player* — private repo

- Full playback engine on Jetpack Compose + Media3, structured as domain/data/presentation clean architecture
- Collaborative **Jam Session** queueing, equalizer & audio effects, lyrics, and an audio trimmer
- Android Auto and Chromecast support, home-screen widgets, local backup/restore, targeting API 26–35
- **Tech stack:** Kotlin · Jetpack Compose · Media3 · Room · DataStore

---

### 🚀 Also Built

#### [AfyaFlow](https://github.com/eliudm/afyaflow)
*Production-grade multi-tenant clinic SaaS for Kenya*

- Zero double-bookings under concurrent load: Redis distributed lock as fast path, Postgres exclusion constraint as backstop
- Multi-tenant data isolation via a Prisma extension that auto-injects tenant scope into every query
- Real-time queue boards over SSE with Redis pub/sub fan-out; M-Pesa payment idempotency; full NHIF/SHA insurance claim state machine
- **Tech stack:** Next.js 16 · TypeScript · PostgreSQL · Redis · Prisma · Docker

#### [PentestDroid](https://github.com/eliudm/PentestDroid)
*Cross-platform mobile penetration testing suite*

- Full pentesting toolkit built in Python/Kivy, running natively on Android and desktop (Linux/macOS/Windows)
- Standard-library only by design — no third-party security dependencies
- **Tech stack:** Python · Kivy · Android · CI/CD (APK build pipeline)

#### [Network Security Toolkit](https://github.com/eliudm/Port_scanner_script)
*Recon & diagnostics script collection*

- Port scanning, banner grabbing, and TCP client/server tooling written from scratch in Python
- Built to understand the protocols they probe, not just wrap an existing library
- **Tech stack:** Python · Sockets · Nmap

---

### 🛠️ Technical Architecture

**Languages**

<p align="left">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white" />
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" />
</p>

**Frameworks & Backend**

<p align="left">
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=flat&logo=nestjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/React_Native-61DAFB?style=flat&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Expo-000020?style=flat&logo=expo&logoColor=white" />
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat&logo=nodedotjs&logoColor=white" />
  <img src="https://img.shields.io/badge/Prisma-2D3748?style=flat&logo=prisma&logoColor=white" />
  <img src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat&logo=jetpackcompose&logoColor=white" />
  <img src="https://img.shields.io/badge/Kivy-1a73e8?style=flat&logo=python&logoColor=white" />
</p>

**Data & Infrastructure**

<p align="left">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/BullMQ-B91C1C?style=flat" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white" />
</p>

**Integrations**

<p align="left">
  <img src="https://img.shields.io/badge/M--Pesa_Daraja-00A651?style=flat" />
  <img src="https://img.shields.io/badge/KRA_eTIMS-C8102E?style=flat" />
  <img src="https://img.shields.io/badge/Africa's_Talking-FF6600?style=flat" />
  <img src="https://img.shields.io/badge/RevenueCat-F25C00?style=flat" />
  <img src="https://img.shields.io/badge/Stripe-635BFF?style=flat&logo=stripe&logoColor=white" />
</p>

**Security & Tooling**

<p align="left">
  <img src="https://img.shields.io/badge/CEH-ECC2096578341-red?style=flat" />
  <img src="https://img.shields.io/badge/Nmap-4682B4?style=flat" />
  <img src="https://img.shields.io/badge/Burp%20Suite-FF6633?style=flat" />
  <img src="https://img.shields.io/badge/Wireshark-1679A7?style=flat&logo=wireshark&logoColor=white" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white" />
</p>

---

### 📊 GitHub Activity

<p align="left">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=eliudm&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=eliudm&layout=compact&hide_border=true" />
</p>
<p align="left">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=eliudm&hide_border=true" />
</p>

---

<p align="center"><i>"Ship it production-grade, then attack it like an adversary would — that's the only way either half of the job counts."</i></p>

<p align="center">📫 Reach out via <a href="https://www.linkedin.com/in/eliud-maina-73b9691b7/">LinkedIn</a> or <a href="mailto:meliud61@gmail.com">email</a></p>
