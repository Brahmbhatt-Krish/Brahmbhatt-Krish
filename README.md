<div align="center">

<img src="./assests/hero.svg" width="100%" alt="Krish Brahmbhatt — Software Engineer | Full Stack | Backend | AI/ML | Systems. Building things that ship > things that slide."/>

<a href="https://krishbrahmbhatt.vercel.app"><img src="https://img.shields.io/badge/Portfolio-0d1117?style=for-the-badge&logo=vercel&logoColor=00FF9C" alt="Portfolio"/></a>
<a href="https://linkedin.com/in/krishbrahmbhatt23"><img src="https://img.shields.io/badge/LinkedIn-0d1117?style=for-the-badge&logo=linkedin&logoColor=00FF9C" alt="LinkedIn"/></a>
<a href="https://leetcode.com/u/Krish_2326/"><img src="https://img.shields.io/badge/LeetCode-0d1117?style=for-the-badge&logo=leetcode&logoColor=00FF9C" alt="LeetCode"/></a>
<a href="mailto:krish.dev.404@gmail.com"><img src="https://img.shields.io/badge/Email-0d1117?style=for-the-badge&logo=gmail&logoColor=00FF9C" alt="Email"/></a>

</div>

<br>

## About

Most of my work sits in three overlapping areas:

- **Full stack & backend.** React / Next.js frontends on Node.js + Express REST APIs, with JWT auth, MongoDB, and Socket.io where real-time matters. Shipped for freelance clients and for my own projects.
- **AI/ML in real software.** Schema-validating LLM output (Gemini + Zod), a local RAG pipeline (Whisper → BGE-M3 embeddings → Llama 3.2 via Ollama), and Pandas / NumPy / Scikit-learn for data work.
- **Systems & debugging.** A multi-threaded Deep Packet Inspection engine in C++, plus internship work debugging rate-limit failures and designing logging for root-cause analysis across 30+ exchange integrations.

Strong OOP fundamentals in **Java** and **Python**. I solve LeetCode in **C++**.

<br>

## Experience

### Software Developer Intern · Xorvest
<sub>May 2026 – July 2026 · Remote</sub>

- Engineered a **unified REST API integration layer in Python** across **30+ cryptocurrency exchanges**, using a **layered service architecture** that decouples business logic from external integrations.
- Troubleshot and resolved exchange **rate-limit failures** by implementing a **Token Bucket** rate limiter that throttles requests *before* they turn into client-side errors.
- Designed a **four-level logging system** (DEBUG / INFO / WARNING / ERROR) to support **root-cause debugging** and end-to-end request traceability.

### Full Stack Developer · Freelance
<sub>December 2025 – Present · Remote</sub>

- Build and deploy full-stack JavaScript applications with **React.js, Next.js, Node.js, Express.js, MongoDB, and Tailwind CSS** for client-focused work.
- Design and consume **RESTful APIs**, implement **JWT authentication**, build reusable React components, and manage application state.
- Engineer backend services in Node.js / Express.js, integrate third-party APIs, add **Socket.io** real-time communication, and deploy through Git-based workflows.

<br>

## Featured Projects

<sub>The diagrams are live: each one is an animated SVG of how the system actually works.</sub>

### 🔬 Deep Packet Inspection System

<img src="./assests/dpi.svg" width="100%" alt="Animated pipeline: Reader → Load Balancer (consistent hashing) → 3 Fast Path threads (TLS SNI → rules) → Writer. Green packets allowed, red packets blocked."/>

Classifies live network traffic by extracting the **TLS SNI** from the Client Hello, then enforces per-flow rules in real time.

- **Multi-threaded pipeline** (Reader → Load Balancer → Fast Path → Writer) with **consistent hashing** so each flow's state lives on one worker.
- **Thread-safe producer-consumer queue** built on mutexes and condition variables.
- **Flow-based rule enforcement** (IP / app / domain blocking) with real-time traffic reporting.

`C++` `Multithreading` `Network Programming` `TLS` &nbsp;·&nbsp; [**Source →**](https://github.com/Brahmbhatt-Krish/Deep-Packet-Inspection-System)

<br>

### 🧠 HireSense

<img src="./assests/hiresense.svg" width="100%" alt="Animated flow: Resume → Gemini API → Zod schema validation → Puppeteer PDF export. A malformed response is rejected at the schema step and retried."/>

AI-powered recruitment platform for resume parsing and interview report generation. The interesting part is making the LLM dependable, not just calling it.

- **Gemini API + Zod schema validation** so every AI response is structured and verified before it reaches the UI.
- **Express.js REST API** with **bcrypt** password hashing and **JWT** authentication.
- Responsive React.js frontend with **PDF export** via Puppeteer.

`React.js` `Node.js` `Express.js` `MongoDB` `Google Gemini` `Zod` `JWT` &nbsp;·&nbsp; [**Live →**](https://hire-sense-swart.vercel.app/login) · [**Source →**](https://github.com/Brahmbhatt-Krish/HireSense)

<br>

### ⚔️ CodeArena

<img src="./assests/arena.svg" width="100%" alt="Animated live leaderboard reordering in real time next to a Socket.io event feed."/>

Full-stack LeetCode progress tracker where multiple users go head-to-head in **live coding battles**.

- **Real-time battle system on Socket.io** with live leaderboard updates for 30+ users.
- **Google OAuth 2.0** sign-in with **JWT** session management.
- Automated **LeetCode stat scraping** visualised with Chart.js donut charts by difficulty.

`React.js` `Node.js` `Socket.io` `MongoDB Atlas` `OAuth 2.0` `Chart.js` &nbsp;·&nbsp; [**Live →**](https://krish2323-codearena.hf.space/) · [**Source →**](https://github.com/Brahmbhatt-Krish/CodeArena)

<br>

### 📚 RAG AI Teaching Assistant

<img src="./assests/rag.svg" width="100%" alt="Animated RAG pipeline: lecture video → Whisper transcript → BGE-M3 embeddings via Ollama → cosine retrieval → Llama 3.2 grounded answer."/>

Ask a question about a lecture, get an answer grounded in the actual transcript instead of a hallucinated one. Runs entirely on local models.

- **4-stage RAG pipeline:** FFmpeg + Whisper large-v2 transcription → Ollama BGE-M3 embeddings → cosine-similarity retrieval → local Llama 3.2 generation.
- Retrieval grounds every answer in transcript chunks, which cuts hallucination.
- No hosted LLM API required.

`Python` `OpenAI Whisper` `Ollama` `Llama 3.2` `Scikit-learn` &nbsp;·&nbsp; [**Source →**](https://github.com/Brahmbhatt-Krish/RAG-based-AI-Teaching_Assistant)

<br>

## Tech Stack

<table>
<tr>
<td align="right"><b>Languages</b></td>
<td><img src="https://skillicons.dev/icons?i=java,py,js,cpp" height="40" alt="Java, Python, JavaScript, C++"/><br><sub>Java · Python · JavaScript · C++</sub></td>
</tr>
<tr>
<td align="right"><b>Frontend</b></td>
<td><img src="https://skillicons.dev/icons?i=react,nextjs,vite,tailwind,html,css" height="40" alt="React, Next.js, Vite, Tailwind CSS, HTML5, CSS3"/><br><sub>React.js · Next.js · Vite · Tailwind CSS · HTML5 · CSS3</sub></td>
</tr>
<tr>
<td align="right"><b>Backend</b></td>
<td><img src="https://skillicons.dev/icons?i=nodejs,express" height="40" alt="Node.js, Express.js"/><br><sub>Node.js · Express.js · REST APIs · Layered Service Architecture · JWT Authentication · Socket.io</sub></td>
</tr>
<tr>
<td align="right"><b>AI / ML</b></td>
<td><img src="https://skillicons.dev/icons?i=sklearn" height="40" alt="Scikit-learn"/> <img src="https://img.shields.io/badge/Google_Gemini-0D1117?style=flat-square&logo=googlegemini&logoColor=00FF9C" height="28" alt="Google Gemini"/> <img src="https://img.shields.io/badge/Llama_3.2-0D1117?style=flat-square&logo=meta&logoColor=00FF9C" height="28" alt="Llama 3.2"/> <img src="https://img.shields.io/badge/Ollama-0D1117?style=flat-square&logo=ollama&logoColor=00FF9C" height="28" alt="Ollama"/><br><sub>LLM Integration (Google Gemini, Llama 3.2) · RAG · Ollama · OpenAI Whisper · Pandas · NumPy · Scikit-learn</sub></td>
</tr>
<tr>
<td align="right"><b>Databases</b></td>
<td><img src="https://skillicons.dev/icons?i=mongodb,firebase,sqlite" height="40" alt="MongoDB, Firebase, SQLite"/><br><sub>MongoDB · MongoDB Atlas · Firebase · SQLite</sub></td>
</tr>
<tr>
<td align="right"><b>Cloud / Infra</b></td>
<td><img src="https://skillicons.dev/icons?i=aws,docker" height="40" alt="AWS, Docker"/><br><sub>AWS (EC2, S3, IAM, Lambda) · Docker</sub></td>
</tr>
<tr>
<td align="right"><b>Tools</b></td>
<td><img src="https://skillicons.dev/icons?i=git,github,postman" height="40" alt="Git, GitHub, Postman"/><br><sub>Git · GitHub · Postman</sub></td>
</tr>
</table>

<br>

## Engineering Problems I've Worked On

| Problem space | Where I've done it |
|:--|:--|
| **REST API design & layered architecture** | Xorvest (30+ exchange integrations) · HireSense · freelance work |
| **Authentication** (JWT · bcrypt · Google OAuth 2.0) | HireSense · CodeArena · freelance work |
| **Rate limiting** (Token Bucket) | Xorvest |
| **Logging & traceability** (four-level severity, root-cause debugging) | Xorvest |
| **Real-time communication** (Socket.io) | CodeArena · freelance work |
| **Multithreading & concurrency** (producer-consumer, mutexes, condition variables) | Deep Packet Inspection System |
| **Network programming** (TLS Client Hello parsing, per-flow state, consistent hashing) | Deep Packet Inspection System |
| **LLM integration with structured, validated output** | HireSense |
| **RAG pipelines & local inference** | RAG AI Teaching Assistant |
| **Cloud fundamentals** (EC2, S3, IAM, RDS, Lambda) | AWS Academy Cloud Foundations labs |

<br>

## Education & Achievements

<table>
<tr>
<td width="50%" valign="top">

<h3>🎓 Education</h3>

<b>Bachelor of Engineering, Computer Engineering</b><br>
Sardar Vallabhbhai Patel Institute of Technology<br>
<sub>Expected May 2027 · CGPA 8.65 / 10</sub>

</td>
<td width="50%" valign="top">

<h3>🏆 Achievements & Certifications</h3>

<ul>
<li><b>Top 1% statewide</b>, Gujarat HSC Board Examination (2023)</li>
<li><b>170+ LeetCode problems</b> solved in C++</li>
<li><b>AWS Academy Cloud Foundations</b>: 20+ labs across EC2, S3, IAM, RDS, Lambda</li>
<li><b>The Ultimate Data Science Course</b> (Code With Harry): 25+ exercises in NumPy, Pandas, Matplotlib</li>
</ul>

</td>
</tr>
</table>

<br>

## Activity

<div align="center">

<img src="https://leetcard.jacoblin.cool/Krish_2326?theme=dark&font=Fira%20Code&ext=heatmap&border=0&radius=10" width="49%" alt="LeetCode stats for Krish_2326"/>
<img src="https://streak-stats.demolab.com/?user=Brahmbhatt-Krish&theme=dark&hide_border=true&background=0D1117&ring=00FF9C&fire=00FF9C&currStreakLabel=00FF9C" width="49%" alt="GitHub contribution streak"/>

<br><br>

<img src="https://raw.githubusercontent.com/Brahmbhatt-Krish/Brahmbhatt-Krish/refs/heads/output/github-snake-dark.svg" width="100%" alt="Contribution graph snake animation"/>

</div>

<br>

<div align="center">

```bash
$ connect --no-spam
```

<a href="https://linkedin.com/in/krishbrahmbhatt23"><img src="https://img.shields.io/badge/LinkedIn-880808?style=for-the-badge&logo=linkedin&logoColor=ffffff" alt="LinkedIn"/></a>
<a href="https://github.com/Brahmbhatt-Krish"><img src="https://img.shields.io/badge/GitHub-880808?style=for-the-badge&logo=github&logoColor=ffffff" alt="GitHub"/></a>
<a href="https://leetcode.com/u/Krish_2326/"><img src="https://img.shields.io/badge/LeetCode-880808?style=for-the-badge&logo=leetcode&logoColor=ffffff" alt="LeetCode"/></a>
<a href="https://krishbrahmbhatt.vercel.app"><img src="https://img.shields.io/badge/Portfolio-880808?style=for-the-badge&logo=vercel&logoColor=ffffff" alt="Portfolio"/></a>
<a href="mailto:krish.dev.404@gmail.com"><img src="https://img.shields.io/badge/Email-880808?style=for-the-badge&logo=gmail&logoColor=ffffff" alt="Email"/></a>

<br><br>

```bash
$ echo "ships > slides. graduating May 2027, open to SDE roles."
```

</div>
