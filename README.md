<div align="center">

# Shreya Singh Chauhan

### Full Stack Developer · AI Engineer

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=7AA2F7&center=true&vCenter=true&width=560&lines=I+ship+products+that+real+people+use.;AI+systems+%E2%80%A2+real-time+apps+%E2%80%A2+backend+pipelines;Next.js+%C2%B7+FastAPI+%C2%B7+Postgres+%C2%B7+LLMs" alt="Typing SVG" />

<br/>

<a href="https://my-portfolio-three-cyan-76.vercel.app">
  <img src="https://img.shields.io/badge/Portfolio-0B0F19?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" />
</a>
<a href="https://www.linkedin.com/in/shreya-chauhan-1026b9278">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
</a>
<a href="mailto:chauhanshreyasingh94@gmail.com">
  <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
</a>

</div>

---

## About

I'm a final-year B.Tech CSE student at **Bennett University** (CGPA 8.97) who would rather deploy something than demo it.

Most of what's on this profile is **live and reachable** — a GitHub App that reviews pull requests, a mental-health platform with an AI chatbot, a real-time messenger, a sign-language translator that runs off your webcam. I care about the parts that don't show up in a screenshot: durable job queues, verified LLM output, sane database schemas, and apps that survive a cold start on free-tier hosting.

- Building AI-powered developer tooling and accessibility-focused products
- Comfortable across the stack — Next.js/React on top, FastAPI/Express/Postgres underneath
- Interested in LLM systems that are *grounded* — RAG, structured output, validation over vibes
- Open to internships and new-grad roles in full stack / AI engineering

---

## Featured Projects

### AI PR Reviewer
> Every pull request gets an automatic review — bugs, security issues, and sloppy code flagged as inline comments before a human looks.

A GitHub App that listens for PR webhooks, enqueues jobs on a **Postgres-backed durable queue** (`SELECT ... FOR UPDATE SKIP LOCKED` — no Redis, survives restarts), sends diffs to **Groq / Llama 3.3**, then validates every finding against the real diff hunks so a hallucinated line number gets dropped instead of breaking the review. Ships with a dashboard tracking findings by severity across repos.

`Node.js` `TypeScript` `Express` `Next.js` `Postgres` `Groq` `zod` `octokit`

**[Live app](https://code-review-assistant-bwf8.onrender.com)** · **[Install the App](https://github.com/apps/shreya-ai-reviewer)** · **[Watch it catch a real bug](https://github.com/Shreya-singh22/theme-9-jewellery/pull/1/files)** · [Code](https://github.com/Shreya-singh22/Code-review-assistant)

<br/>

### You Matter Now — Mental Health Platform
> Accessible, always-on emotional support: an empathetic AI chatbot, secure journaling with mood tracking, self-assessment screeners, and therapist discovery.

Built around the idea that support should be available at 3am, not just during office hours. Groq-hosted Llama 3 handles conversation; journaling, gratitude prompts, and wellness games handle everything the model shouldn't.

`TypeScript` `React` `Vite` `Tailwind` `shadcn/ui` `Groq`

**[Live demo](https://you-matter-games-journal-main.vercel.app)** · [Code](https://github.com/Shreya-singh22/you-matter-now)

<br/>

### Sign Language Detector
> Show an ASL sign to your webcam and the letter appears — live, in the browser.

Frames stream to a Flask backend where **MediaPipe Hands** extracts 21 landmarks and a Random Forest classifier maps them to 28 classes (A–Z, space, nothing). Hold a sign steady for one second and it commits the letter to your sentence. Landmark-based rather than pixel-based, so it's fast enough to feel instant.

`Python` `Flask` `MediaPipe` `scikit-learn` `OpenCV`

**[Try it live](https://sign-lang-ai.onrender.com)** · [Code](https://github.com/Shreya-singh22/sign-lang-detector-)

<br/>

### Signal Clone — Real-Time Messenger
> Full-stack Signal-inspired messenger: 1:1 and group chat over WebSockets, typing indicators, read receipts, reactions, replies, attachments, and disappearing messages.

Everything except the cryptography is real — genuine auth, persistence, real-time delivery, and group management against a live database and socket connection. (Encryption is deliberately mocked; no Double Ratchet here, and the README says so.)

`Next.js 16` `TypeScript` `FastAPI` `SQLAlchemy` `WebSockets` `Framer Motion`

**[Live demo](https://signal-clone-drab.vercel.app)** · [Code](https://github.com/Shreya-singh22/Signal-clone)

---

## More Things I've Built

| Project | What it does | Stack |
|---|---|---|
| **[NexHire](https://github.com/Shreya-singh22/NexHire)** | Agentic recruiting suite — scores résumés across a weighted 5-dimension matrix with human-in-the-loop validation and PII redaction before anything hits an LLM | LangGraph, Gemini, FAISS + BM25, Streamlit |
| **[Transaction Pipeline](https://github.com/Shreya-singh22/txn-pipeline)** | Async pipeline that ingests messy financial CSVs, cleans them, detects anomalies, classifies with an LLM, and returns a narrative risk summary via a job-polling API | FastAPI, Celery, Redis, Postgres, Gemini, Docker |
| **[Google Calendar Clone](https://google-calendar-clone-iota.vercel.app)** | Multi-calendar management, recurring events, dark mode, offline-first fallback — fully deployed | Next.js 16, Express, Prisma, Postgres |
| **[PII Redaction Tool](https://github.com/Shreya-singh22/PII-Redaction-Tool)** | Redacts names, IDs, and contact info from `.docx` files while preserving formatting, with consistent fake replacements and a precision/recall eval harness | Python, spaCy NER, Faker, Flask |
| **[Mental Health RAG](https://github.com/Shreya-singh22/mental-health-rag-endee)** | Fully local RAG pipeline — grounded answers from a vector DB instead of hallucinated ones | Sentence Transformers, Endee, Flan-T5, Docker |
| **[YourSakhi](https://github.com/Shreya-singh22/YourSakhi-Dti-Project)** | Women's health platform — menstrual tracking, personalized guidance, and a wellness chatbot | TypeScript, React, Tailwind |
| **[Micro Marketplace](https://micro-marketplace-mu.vercel.app)** | Full-stack marketplace with auth, cart, checkout, and favourites — web *and* React Native mobile | Node, Express, Prisma, React, Expo |
| **[Tripzy](https://tripzy-indol.vercel.app)** | Travel-booking SPA with JWT auth and server-computed booking totals | Node, Express, Prisma, JWT |

---

## Tech Stack

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=python,ts,js,java,cpp,rust" />

**Frontend**

<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite,threejs,figma" />

**Backend & Data**

<img src="https://skillicons.dev/icons?i=nodejs,express,fastapi,flask,postgres,prisma,redis,mongodb" />

**AI & Infra**

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn,docker,git,vercel" />

</div>

---

## Experience

**Full Stack Developer Intern** — Evoc Labs · *Jan 2026 – May 2026*
Built responsive React/TypeScript applications, authored a reusable component library that cut development time ~30%, and shipped 10+ production features with the team.

**Social Media Head** — Zenevia Tech Fest · *Feb 2024 – Feb 2025*
Led the social presence for the university tech fest and grew engagement by 60%.

**Organizer** — CodeChef BU & Career Advancement Club
Ran 10+ technical events and 5+ workshops for the campus developer community.

---

## GitHub

<div align="center">

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Shreya-singh22&theme=tokyonight" alt="Profile summary" />

<img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Shreya-singh22&theme=tokyonight" alt="Languages by repo" />
<img height="180" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Shreya-singh22&theme=tokyonight" alt="Languages by commit" />

<img src="https://streak-stats.demolab.com?user=Shreya-singh22&theme=tokyonight&hide_border=true&background=0D1117" alt="GitHub streak" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Shreya-singh22&theme=tokyo-night&hide_border=true&bg_color=0D1117&area=true" alt="Contribution graph" />

</div>

---

<div align="center">

### Let's build something

<a href="mailto:chauhanshreyasingh94@gmail.com">chauhanshreyasingh94@gmail.com</a> · <a href="https://www.linkedin.com/in/shreya-chauhan-1026b9278">LinkedIn</a> · <a href="https://my-portfolio-three-cyan-76.vercel.app">Portfolio</a>

<sub>Building technology that empowers, heals, and includes.</sub>

</div>
