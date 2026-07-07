# Eduard-George Iliescu

Automation & Computer Science, Technical University of Civil Engineering Bucharest (UTCB), entering 4th year
edi2004george@gmail.com · +40 754 044 031
GitHub: github.com/ed0one · LinkedIn: linkedin.com/in/eduard-iliescu-582ab22b4

I build full-stack web applications. Most recently: an AI-powered task management app, live in production, built in a team of 4 during a summer internship.

## Projects

### TaskCapture — AI task management · [live: taskcapture.xyz](https://www.taskcapture.xyz) · [code](https://github.com/ed0one/practica_devidevs)

Role: tech lead in a team of 4 (DeviDevs internship, June–July 2026).

- Built the pipeline that turns free-form text into structured tasks: prompt with the current date injected (resolves relative deadlines like "by Friday"), extraction from LLM output (NVIDIA NIM, Llama 3.1), and Zod validation that coerces invalid fields to `null` instead of failing the whole task.
- Implemented email notifications (Resend): a daily digest at each user's local hour (per-timezone computation) plus per-task reminders, idempotent, driven by a hybrid Vercel + Supabase pg_cron scheduler to work around the daily-cron limit on the Hobby plan.
- Built the full auth flow: email/password + Google/GitHub OAuth via Supabase with PKCE, route-protection middleware, password reset, and per-user data isolation through Row-Level Security.
- Shipped the app to production on Vercel with a custom domain, rate limiting (Upstash Redis), and unit test suites (Vitest) covering the critical logic.

## Technical skills

- Languages: TypeScript/JavaScript, SQL, Java, C/C++, Python
- Web: Next.js (App Router), React, Node, Tailwind CSS
- Data & infra: Supabase, PostgreSQL (RLS), Vercel, Git, Upstash Redis
- AI/tooling: LLM integration (OpenAI SDK), prompt design + Zod validation, AI coding agents (Claude Code, opencode), Vitest

## Education

Technical University of Civil Engineering Bucharest (UTCB) — Automation & Computer Science, entering 4th year (expected graduation 2027). Coursework: Java, C/C++, Python, databases, algorithms.
