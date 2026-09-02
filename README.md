<div align="center">

# Benyamin Mahamed

<samp>Recent Computer Science Graduate · Backend Engineering · Applied AI</samp>

<samp>BSc (Hons) Computer Science, 2:1 — University of Westminster, 2026 — London, UK</samp>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/benyamin-mahamed)
[![Portfolio](https://img.shields.io/badge/Portfolio-benyaminmahamed.netlify.app-orange?style=for-the-badge&logo=firefox&logoColor=white)](https://benyaminmahamed.netlify.app)
[![Email](https://img.shields.io/badge/Email-benyaminmahamed%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:benyaminmahamed@gmail.com)

</div>

<br/>

> I build things at the intersection of backend engineering and AI — RAG pipelines, computer vision systems, editorial platforms serving real users. Currently looking for junior software engineering / full-stack roles in London.

<br/>

<div align="center"><samp>— NOW BUILDING —</samp></div>
<br/>

### [Court Vision](https://court-vision-ng9w.onrender.com) — live

A free basketball film-study web app. Two features: a searchable library of basketball actions (pistol, Spain pick-and-roll, horns) mapping named concepts to written breakdowns and key reads — and **interactive NBA shot charts where clicking any shot opens that exact possession's clip on NBA.com**. Built to solve a real problem: when you start studying film you can't name what you're watching, stats sites give you numbers with no film, and pro film tools are paywalled and coach-facing.

Live and in active development.

- **~50,000 shots across 50 players** (2025–26 season), pulled via `nba_api` through a local, resumable, idempotent ingestion pipeline. NBA's API blocks cloud IPs, so ingestion runs locally and the deployed app only reads from the DB — FG% validated against real stats.
- **Interactive SVG shot charts** rendered from raw court coordinates (orange makes / grey misses), with per-zone shooting splits, a stat strip, season filter, and a dots/zones toggle.
- **Click-to-film:** each shot dot is a native SVG link to its exact possession on NBA.com, built purely from stored game/event/season fields — no video hosting, no caching, legal by construction.

<samp>Django · PostgreSQL (Neon) · nba_api · Render · WhiteNoise</samp>

*Next up:* shot-type filtering — pull-up vs. catch-and-shoot, with in-page clips (`action_type` data already stored).

<br/>

<div align="center"><samp>— SHIPPED —</samp></div>
<br/>

### [Lexis — AI Research Assistant](https://github.com/BenyaminMahamed/AI-Research-Assistant)

A RAG pipeline built from scratch — no LangChain, no abstractions. PDFs are extracted page-by-page with PyMuPDF, chunked into 500-word overlapping windows, embedded with `all-MiniLM-L6-v2` (384-dim, normalised), and indexed in FAISS. Queries run nearest-neighbour search and pass the top-k chunks as grounded context to Gemini 2.0 Flash.

Four modes — Q&A, structured summarisation, peer-review critique, multi-paper comparison. Every answer surfaces the source chunks and page numbers it was based on. Containerised with Docker and covered by a 13-test suite running in GitHub Actions CI. Built because tools like ChatPDF felt like black boxes with no source grounding.

<samp>Django · DRF · FAISS · Sentence-Transformers · PyMuPDF · Gemini 2.0 Flash · Docker</samp>

<br/>

### [The BluePrint Brief](https://theblueprintbrief.com) — private repo, live in production

Co-founded this live editorial platform for legal and commercial content in March 2025, and develop it as part of a three-person engineering team. A Django-powered editorial CMS — a lightweight version of what a newsroom would run internally.

My ownership: the Render deployment, the Cloudinary media layer, domain and email infrastructure, and primary production debugging. Shipped end-to-end: an access-gated Student Resources system, Beehiiv newsletter integration, and the submission notification pipeline. **Grew to 1,000+ registered users within five months of launch.** Architecture write-up: [blueprint-brief-architecture](https://github.com/BenyaminMahamed/blueprint-brief-architecture)

<samp>Django · PostgreSQL · JavaScript · HTML/CSS · Linux · Gunicorn</samp>

<br/>

### [Autonomous Navigation System](https://github.com/BenyaminMahamed/FINALYEARPROJECT) — Final Year Project

Real-time lane following and obstacle detection on a Raspberry Pi 5, built as a proof-of-concept for affordable assistive mobility. The core question: can you replicate the navigation capabilities of £5,000+ commercial systems for under £200?

Validated across a 10,298-frame integration session on physical hardware:

<div align="center">

| Metric | Target | Result |
|---|:---:|:---:|
| Processing latency | < 200ms | **~10ms** (20× margin) |
| Frame rate | ≥ 8 FPS | **~14 FPS** sustained |
| Obstacle detection | 100% in-session | **100% in-session**, zero false positives |
| Manual override response | < 50ms | **< 10ms** |
| Hardware cost | — | **< £200** |

</div>

Deliberately classical CV rather than deep learning — YOLOv5 on a Pi CPU costs 80–120ms per frame before anything else, and for a safety-critical assistive system I wanted deterministic, inspectable failure modes over a probabilistic model. A class-agnostic blob detector delivered that in under 5ms per frame. [Full demo video →](https://www.youtube.com/watch?v=ol9_oAe9Ogk)

<samp>Python · OpenCV · NumPy · Picamera2 · Raspberry Pi 5 · PiCar-X SDK</samp>

<br/>

<div align="center"><samp>— STACK —</samp></div>
<br/>

<table>
<tr>
<td valign="top" width="50%">

**Backend & Web**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Django](https://img.shields.io/badge/django-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

</td>
<td valign="top" width="50%">

**AI / ML**

![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-%23FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=black)
![Google Gemini](https://img.shields.io/badge/Gemini-%234285F4.svg?style=for-the-badge&logo=google&logoColor=white)

</td>
</tr>
<tr>
<td valign="top" width="50%">

**Languages**

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

</td>
<td valign="top" width="50%">

**Tools & Infrastructure**

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)

</td>
</tr>
</table>

<br/>

<div align="center">

<samp>The best way to reach me is <a href="https://linkedin.com/in/benyamin-mahamed">LinkedIn</a> or <a href="mailto:benyaminmahamed@gmail.com">email</a>.</samp>

</div>
