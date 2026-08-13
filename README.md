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

Most of what's on this profile is **live and clickable** — a GitHub App that reviews pull requests, an async pipeline that risk-scores financial data with an LLM, a mental-health platform with an AI chatbot, a sign-language translator that runs off your webcam.

- Next.js/React on top, FastAPI/Express/Postgres underneath
- LLM systems that are grounded — RAG, structured output, validation before anything gets shown
- Shipped 10+ production features as a full stack intern at Evoc Labs
- Open to internships and new-grad roles in full stack / AI engineering

---

## Featured Projects

### AI PR Reviewer
**[Live app](https://code-review-assistant-bwf8.onrender.com)** · **[Install the GitHub App](https://github.com/apps/shreya-ai-reviewer)** · **[See it catch a real bug](https://github.com/Shreya-singh22/theme-9-jewellery/pull/1/files)** · [Code](https://github.com/Shreya-singh22/Code-review-assistant)

Install it on a repo and every PR gets reviewed automatically — inline comments on bugs, security issues, and leftover debug logs.

- Opening or updating a PR fires a webhook that enqueues a job
- Job queue runs on Postgres with `SELECT ... FOR UPDATE SKIP LOCKED` — durable across restarts, no Redis
- Groq / Llama 3.3 returns findings as JSON, validated with `zod`
- Every finding is matched against the actual diff hunks; hallucinated line numbers get dropped, not posted
- Dashboard tracks review history and findings by severity across all your repos

`Node.js` `TypeScript` `Express` `Next.js` `Postgres` `Groq` `octokit`

<br/>

### Transaction Processing Pipeline
[Code](https://github.com/Shreya-singh22/txn-pipeline)

Ingests messy financial CSVs and returns a risk summary through a job-polling API.

- Cleans the data: ISO 8601 dates, stripped `$` signs, normalized currency/status, deduped rows
- Flags anomalies, then classifies each transaction with Gemini
- FastAPI enqueues to Redis, Celery workers process, Postgres stores jobs and results
- Whole thing runs on Docker Compose — api, worker, redis, db

`FastAPI` `Celery` `Redis` `Postgres` `Gemini` `Docker`

<br/>

### You Matter Now — Mental Health Platform
**[Live demo](https://you-matter-games-journal-main.vercel.app)** · [Code](https://github.com/Shreya-singh22/you-matter-now)

Mental health support that's available at 3am, not just office hours.

- 24/7 AI chatbot for empathetic conversation, running on Groq's Llama 3
- Journaling with mood tracking and gratitude prompts
- Anxiety and depression self-assessment screeners
- Therapist and doctor discovery
- Mindfulness games for stress reduction

`TypeScript` `React` `Vite` `Tailwind` `shadcn/ui` `Groq`

<br/>

### NexHire — Agentic Recruiter Suite
[Code](https://github.com/Shreya-singh22/NexHire)

Screens résumés against a job description and ranks candidates on a sortable leaderboard.

- LangGraph state machine handles ingest branching and human-in-the-loop validation
- Scores across 5 weighted dimensions: skills (30%), relevance (25%), production experience (20%), credentials (15%), writing (10%)
- Hybrid retrieval — FAISS vectors fused with BM25 keyword ranking
- PII is stripped before anything leaves for an external LLM

`LangGraph` `Gemini` `FAISS` `BM25` `Streamlit` `Docker`

<br/>

### Sign Language Detector
**[Try it live](https://sign-lang-ai.onrender.com)** · [Code](https://github.com/Shreya-singh22/sign-lang-detector-)

Show an ASL sign to your webcam and the letter appears, live.

- Browser streams webcam frames to a Flask backend as base64 JPEG
- MediaPipe Hands pulls 21 hand landmarks out of each frame
- A Random Forest classifier maps those coordinates to 28 classes (A–Z, space, nothing)
- Hold a sign steady for 1 second and it commits the letter to your sentence
- Annotated frames come back with landmarks and bounding box drawn on

`Python` `Flask` `MediaPipe` `scikit-learn` `OpenCV`

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

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Shreya-singh22&theme=tokyo-night&hide_border=true&bg_color=0D1117&area=true" alt="Contribution graph" />

</div>

---

<div align="center">

### Let's build something

<a href="mailto:chauhanshreyasingh94@gmail.com">chauhanshreyasingh94@gmail.com</a> · <a href="https://www.linkedin.com/in/shreya-chauhan-1026b9278">LinkedIn</a> · <a href="https://my-portfolio-three-cyan-76.vercel.app">Portfolio</a>

<sub>Building technology that empowers, heals, and includes.</sub>

</div>
