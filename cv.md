# Eduard-George Iliescu

Automation & Computer Science, Technical University of Civil Engineering Bucharest (UTCB), entering 4th year
eduard.iliescu.devidevs@gmail.com · +40 754 044 031
GitHub: github.com/ed0one · LinkedIn: linkedin.com/in/eduard-iliescu-582ab22b4

I build full-stack web applications. Most recently: an AI-powered task management app, live in production, built in a team of 4 during a summer internship.

## Projects

### TaskCapture — AI task management · [live: taskcapture.xyz](https://www.taskcapture.xyz) · [code](https://github.com/ed0one/practica_devidevs)

Role: tech lead in a team of 4 (DeviDevs internship, June–July 2026).

- Built the pipeline that turns free-form text into structured tasks: prompt with the current date injected (resolves relative deadlines like "by Friday"), extraction from LLM output (NVIDIA NIM, Llama 3.1), and Zod validation that coerces invalid fields to `null` instead of failing the whole task.
- Implemented email notifications (Resend): a daily digest at each user's local hour (per-timezone computation) plus per-task reminders, idempotent, driven by a hybrid Vercel + Supabase pg_cron scheduler to work around the daily-cron limit on the Hobby plan.
- Built the full auth flow: email/password + Google/GitHub OAuth via Supabase with PKCE, route-protection middleware, password reset, and per-user data isolation through Row-Level Security.
- Shipped the app to production on Vercel with a custom domain, rate limiting (Upstash Redis), and unit test suites (Vitest) covering the critical logic.

### Other projects

- **Fire Alarm System** — ESP32 sensor firmware → Node.js serial bridge (automatic port detection, multi-sensor alarm fusion) → React/Vite dashboard with Blynk push notifications. [code](https://github.com/ed0one/fire-alarm-system)
- **Smart Parking Management System** — Oracle PL/SQL schema (triggers, stored procedures) behind a Node.js/Express API, with auth, real-time spot availability, reservations, and subscriptions on a React dashboard. [code](https://github.com/ed0one/smart_parking_project)
- **SmartPot & IoT Telemetry** — Automated plant care and irrigation system: soil moisture sensor calibration, threshold-based solenoid control, low-power telemetry reporting. [code](https://github.com/ed0one/SmartPot_autowatering)
- **Job Board TW** — Full-stack career portal and candidate tracking system with role-based routing, structured MySQL schemas, and applicant management workflows. [live](https://jobboard-tw.vercel.app)
- **Second Brain / Context Engine** — Local-first associative memory architecture and knowledge graph engine: deterministic ingestion pipelines, semantic graph traversal, bidirectional markdown vault sync.
- **Personal OS** — Autonomous developer workspace runtime (Next.js 16, LLM Agent SDKs) with persistent file-backed associative memory for self-orchestrating task execution.

Full write-ups: [ed0one.github.io/portfolio](https://ed0one.github.io/portfolio/)

## Technical skills

- Languages: TypeScript/JavaScript, SQL, Java, C/C++, Python
- Web: Next.js (App Router), React, Node, Tailwind CSS
- Data & infra: Supabase, PostgreSQL (RLS), Vercel, Git, Upstash Redis
- AI/tooling: LLM integration (OpenAI SDK), prompt design + Zod validation, AI coding agents (Claude Code, opencode), Vitest

## Education

Technical University of Civil Engineering Bucharest (UTCB) — Automation & Computer Science, entering 4th year (expected graduation 2027). Coursework: Java, C/C++, Python, databases, algorithms.
