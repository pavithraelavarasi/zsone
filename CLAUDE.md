# About Me
- I am building a full stack development training program called **Mindframe**
- I run an in-product tutor company teaching students who have completed 12th grade (with or without computer science background)
- My teaching philosophy: students learn by observing, reverse engineering, and thinking — not by copying syntax

# Project Context
- This is a 52-week full stack development curriculum
- The curriculum is hosted on Zoho Catalyst Slate and AppSail
- Reviewer dashboard is a separate internal tool for instructors — not for students
- Learning platform is student-facing — built as standalone HTML pages

# Curriculum Structure
- Phase 1 (Weeks 1–12): Foundations — no code, system thinking, mental models
- Phase 2 (Weeks 13–23): Frontend
- Phase 3 (Weeks 24–35): Backend and Full Stack
- Phase 4 (Weeks 36–52): Advanced and Career

# Completed Weeks
- Week 1: Map a Product You Love — system mapping, SSH/SCP terminal submission
- Week 2: Trace a Request — request-response journey, DevTools network tab
- Week 3: Read the Web's Language — 20 developer terms, jargon translation, ping/curl terminal tasks

# Each Week Has Three Deliverables
1. Assignment question (given to students)
2. Learning page (student-facing, hosted on Slate — teaches concepts WITHOUT revealing assignment answers)
3. Reviewer dashboard entry (instructor-facing — assignment, learning guide summary, reviewer questions with good/weak answer guides)

# Tech Stack
- Frontend: Plain HTML, CSS, JavaScript — no frameworks
- Hosting: Zoho Catalyst Slate (student pages), Zoho Catalyst AppSail (backend proxy)
- Backend proxy: Node.js Express on AppSail (server.js)
- AI Tutor: Gemini API via AppSail proxy (Zoho internal PlatformAI blocked externally)
- Reviewer dashboard: Single HTML file with slate gray + teal theme

# Key Design Decisions
- Learning pages teach concepts using NEUTRAL examples only (ATM, library, canteen, train booking, hospital) — never the 4 assignment products (Instagram, YouTube, Zomato, Rapido)
- Assignment questions never give away commands or answers — students must research and figure out
- Terminal submission is part of every assignment — students SSH and SCP files to a remote server
- Reviewer questions are split into Core (every student), Deep (strong submissions), Stretch (exceptional)

# Assignment Submission Pattern
- Students produce 3 PDFs per week
- Files go to specific folders on a remote server via SSH + SCP
- Server path pattern: /home/submissions/weekN/

# Student Profile
- Just completed 12th grade
- Mix of computer science and non-computer science backgrounds
- Complete beginners to development
- Already use Instagram, YouTube, Zomato, Rapido daily

# Learning Page Pattern
- 5–6 lessons per page
- Sidebar with progress tracking
- Animated interactive elements (no answers revealed)
- AI tutor (floating 🎓 button) — explains concepts only, never does assignment for student
- Tutor system prompt: concept-only, no code, no assignment answers, neutral examples only

# AppSail Proxy Details
- URL: https://zsone-app-50042017815.development.catalystappsail.in/api/tutor
- Endpoint: POST /api/tutor
- Request body: { userMessage: "string" }
- Response body: { reply: "string" }
- Environment variables: GEMINI_API_KEY, ZOHO_CLIENT_ID, ZOHO_CLIENT_SECRET, ZOHO_REFRESH_TOKEN

# Slate URLs
- Week 1 learning: https://zsone-quvftyvt.onslate.in/week1_learningTutor.html
- Week 2 learning: https://zsone-quvftyvt.onslate.in/week2_learning.html
- Week 3 learning: https://zsone-quvftyvt.onslate.in/week3_learning.html

# Preferences
- Never give assignment answers in learning pages
- Never show terminal commands directly — describe what they do conceptually
- Keep responses concise and direct
- When building learning pages: use animations and interactive elements to keep it engaging
- When building reviewer questions: always include hint, good answer, weak answer for each question
- Design style: clean, minimal, professional — no dark themes for student pages
- Reviewer dashboard theme: slate gray background with teal accents
