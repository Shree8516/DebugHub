<div align="center">

```
██████╗ ███████╗██████╗ ██╗   ██╗ ██████╗ ██╗  ██╗██╗   ██╗██████╗
██╔══██╗██╔════╝██╔══██╗██║   ██║██╔════╝ ██║  ██║██║   ██║██╔══██╗
██║  ██║█████╗  ██████╔╝██║   ██║██║  ███╗███████║██║   ██║██████╔╝
██║  ██║██╔══╝  ██╔══██╗██║   ██║██║   ██║██╔══██║██║   ██║██╔══██╗
██████╔╝███████╗██████╔╝╚██████╔╝╚██████╔╝██║  ██║╚██████╔╝██████╔╝
╚═════╝ ╚══════╝╚═════╝  ╚═════╝  ╚═════╝ ╚═╝  ╚═╝ ╚═════╝ ╚═════╝
```

### *Build a debugging instinct. One bug at a time.*

<br/>

[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-3178C6?style=for-the-badge&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)](https://www.prisma.io/)

<br/>

> **Built at Zenith Hackathon 2026** · Team 404

</div>

---

<br/>

## The Problem

Every platform teaches you to write code from a blank screen. Your job hands you someone else's broken codebase and a deadline. **67% of developers say they spend more time debugging since adopting AI tools.** The skill that matters most is the one nobody trains.

DebugHub fixes that.

<br/>

---

## Features

<table>
<tr>
<td width="50%" valign="top">

### 🎯 Daily Bug & Practice Challenges

One curated real-world bug every day inside a live Monaco Editor. Streaks reward consistency, a Rhythm Score tracks long-term habit, and shareable milestone cards let you prove it. Powered by **Gemini 2.5 Flash** for infinite AI-generated practice across any language, difficulty, and bug type.

</td>
<td width="50%" valign="top">

### 🧠 Diagnostic Path

A split-screen comparison of your debugging steps against an AI agent's reasoning and an expert's optimal path. Not just the answer — the *thinking* behind it. See exactly where your diagnosis diverged and why.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 💥 Production Incident Simulator

Practice incident response before facing real outages. Real scenarios — API outages, latency spikes, database overload. Inspect logs, trace failures, diagnose root cause, deploy fixes. Includes the **Knight Capital 2012** case study: $440M lost in 45 minutes from one undetected bug.

</td>
<td width="50%" valign="top">

### 🤝 Community & User Portfolio

Post real bugs, solve others', earn Trust Points. Your profile dashboard visualises debugging activity, skill distribution across bug types, language coverage, streaks, and community impact — a portfolio that proves what you can *fix*, not just what you built.

</td>
</tr>
</table>

<br/>

---

## Tech Stack

<div align="center">

### Frontend
![React](https://img.shields.io/badge/React_18-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Monaco](https://img.shields.io/badge/Monaco_Editor-0078D4?style=for-the-badge&logo=visualstudiocode&logoColor=white)
![Zustand](https://img.shields.io/badge/Zustand-443E38?style=for-the-badge&logo=react&logoColor=white)

### Backend
![NodeJS](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

### AI & Services
![Gemini](https://img.shields.io/badge/Gemini_2.5_Flash-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Google OAuth](https://img.shields.io/badge/Google_OAuth2-EA4335?style=for-the-badge&logo=google&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white)
![Razorpay](https://img.shields.io/badge/Razorpay-02042B?style=for-the-badge&logo=razorpay&logoColor=3395FF)

</div>

<br/>

---

## Getting Started

### Prerequisites

```bash
node --version   # v18+
psql --version   # PostgreSQL running locally
```

You'll also need a [Google Cloud Console](https://console.cloud.google.com) OAuth project, a [Google AI Studio](https://aistudio.google.com) API key, and a [Razorpay](https://razorpay.com) account.

<br/>

### 1 — Clone

```bash
git clone https://github.com/yourusername/DebugHub.git
cd DebugHub
```

### 2 — Backend

```bash
cd backend && npm install
```

Create `backend/.env`:

```env
PORT=3001
DATABASE_URL="postgresql://user:password@localhost:5432/debughub"
FRONTEND_URL="http://localhost:5173"

GOOGLE_CLIENT_ID="your_google_client_id"
GOOGLE_CLIENT_SECRET="your_google_client_secret"
GOOGLE_CALLBACK_URL="http://localhost:3001/auth/google/callback"
JWT_SECRET="your_ultra_secure_jwt_secret"

GEMINI_API_KEY="your_google_ai_studio_api_key"

EMAIL_USER="your-email@gmail.com"
EMAIL_PASS="your-app-password"
```

```bash
npx prisma generate && npx prisma db push
npm run dev
```

### 3 — Frontend

```bash
cd frontend && npm install
```

Create `frontend/.env`:

```env
VITE_API_URL="http://localhost:3001"
VITE_RAZORPAY_KEY="your_razorpay_key_id"
VITE_APP_URL="http://localhost:5173"
VITE_SALES_EMAIL="sales@debughub.com"
```

```bash
npm run dev
```

<br/>

---

## Pricing

| | **Freemium** | **Pro — ₹999/mo** | **Recruiter — ₹4,999/mo** |
|---|:---:|:---:|:---:|
| Daily Bug Challenge | ✓ | ✓ | ✓ |
| Community Feed | ✓ | ✓ | ✓ |
| Infinite Practice | 3/day | Unlimited | Unlimited |
| Diagnostic Path Reports | — | ✓ | ✓ |
| Verified Resume Badge | — | ✓ | ✓ |
| War Room — Incident Simulator | — | — | ✓ |

<br/>

---
## 📊 Project Status

<p align="center">

<img src="https://img.shields.io/website?down_color=red&down_message=offline&label=Deployment&up_color=00C853&up_message=live&url=https%3A%2F%2Fdebughub1.vercel.app&style=for-the-badge"/>

<img src="https://komarev.com/ghpvc/?username=Shree8516&repo=DebugHub&label=Visitors&color=8A2BE2&style=for-the-badge"/>

<img src="https://img.shields.io/github/last-commit/Shree8516/DebugHub?style=for-the-badge"/>

<img src="https://img.shields.io/github/languages/top/Shree8516/DebugHub?style=for-the-badge"/>

</p>
