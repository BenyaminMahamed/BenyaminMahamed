<div align="center">

# Benyamin Mahamed

<samp>Backend Engineering · Applied AI · Computer Vision</samp>

<samp>BSc (Hons) Computer Science — University of Westminster, 2026 — London, UK</samp>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/benyamin-mahamed)
[![Email](https://img.shields.io/badge/Email-benyaminmahamed%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:benyaminmahamed@gmail.com)

</div>

<br/>

> I build things at the intersection of backend engineering and AI — RAG pipelines, computer vision systems, editorial platforms. Currently looking for junior backend / AI engineering roles.

<br/>

<div align="center"><samp>— NOW BUILDING —</samp></div>
<br/>

| Project | What it is |
|---|---|
| **Basketball GM engine** | Possession-based Monte Carlo dynasty simulator, tuned phase-by-phase against real NBA statistical distributions (scoring, margins, pace), with a 1,000-game batch validation harness |
| **Embedded CV performance** | Profiling where the milliseconds actually go in a classical vision loop on the Raspberry Pi 5 |

<br/>

<div align="center"><samp>— SHIPPED —</samp></div>
<br/>

### [Lexis — AI Research Assistant](https://github.com/BenyaminMahamed/AI-Research-Assistant)

A RAG pipeline built from scratch — no LangChain, no abstractions. PDFs are extracted page-by-page with PyMuPDF, chunked into 500-word overlapping windows, embedded with `all-MiniLM-L6-v2` (384-dim, normalised), and indexed in FAISS. Queries run nearest-neighbour search and pass the top-k chunks as grounded context to Gemini 2.0 Flash.

Four modes — Q&A, structured summarisation, peer-review critique, multi-paper comparison. Every answer surfaces the source chunks and page numbers it was based on. Built because tools like ChatPDF felt like black boxes with no source grounding.

<samp>Django · DRF · FAISS · Sentence-Transformers · PyMuPDF · Gemini 2.0 Flash · SQLite</samp>

<br/>

### [The BluePrint Brief](https://theblueprintbrief.com) — private repo, live in production

Co-founded this live editorial platform for legal and commercial content, and develop it as part of a three-person engineering team. A Django-powered editorial CMS — a lightweight version of what a newsroom would run internally.

My ownership: the Render deployment, the Cloudinary media layer, domain and email infrastructure, and primary production debugging. Shipped end-to-end: an access-gated Student Resources system, Beehiiv newsletter integration, and the submission notification pipeline. **1,000+ active users.** Architecture write-up: [blueprint-brief-architecture](https://github.com/BenyaminMahamed/blueprint-brief-architecture)

<samp>Django · PostgreSQL · JavaScript · HTML/CSS · Linux · Gunicorn</samp>

<br/>

### [Autonomous Navigation System](https://github.com/BenyaminMahamed/FINALYEARPROJECT) — final year project

Real-time lane following and obstacle detection on a Raspberry Pi 5, built as a proof-of-concept for affordable assistive mobility. The core question: can you replicate the navigation capabilities of £5,000+ commercial systems for under £200?

Validated across a 10,298-frame integration session on physical hardware:

<div align="center">

| Metric | Target | Result |
|---|:---:|:---:|
| Processing latency | < 200ms | **~10ms** (20× margin) |
| Frame rate | ≥ 8 FPS | **~14 FPS** sustained |
| Obstacle detection reliability | 100% | **100%**, zero false positives |
| Manual override response | < 50ms | **< 10ms** |
| Hardware cost | — | **< £200** |

</div>

Deliberately Classical CV rather than deep learning — YOLOv5 on a Pi CPU costs 80–120ms per frame before anything else, and a probabilistic model can't guarantee the 100% detection reliability a safety-critical assistive system needs. A class-agnostic blob detector can, in under 5ms.

<samp>Python · OpenCV · NumPy · Picamera2 · Raspberry Pi 5 · PiCar-X SDK</samp>

<br/>

<div align="center"><samp>— STACK —</samp></div>
<br/>

<table>
<tr>
<td valign="top" width="50%">

**Languages**

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

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

**Web & Backend**

![Django](https://img.shields.io/badge/django-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

</td>
<td valign="top" width="50%">

**Embedded, Security & Infrastructure**

![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557CF2?style=for-the-badge&logo=kali-linux&logoColor=white)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-%23000000.svg?style=for-the-badge&logo=owasp&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)

</td>
</tr>
</table>

<br/>

<div align="center">

<samp>The best way to reach me is <a href="https://linkedin.com/in/benyamin-mahamed">LinkedIn</a> or <a href="mailto:benyaminmahamed@gmail.com">email</a>.</samp>

</div>
