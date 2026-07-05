<div align="center">

# Hey, I'm Benyamin 👋

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1200&center=true&vCenter=true&width=600&lines=Backend+Engineering+%C2%B7+Applied+AI;RAG+Pipelines+%C2%B7+Computer+Vision;BSc+(Hons)+Computer+Science%2C+2026;Open+to+junior+backend+%2F+AI+roles" alt="Typing intro"/>

CS graduate (University of Westminster, 2026) based in London.
I build things at the intersection of backend engineering and AI — RAG pipelines, computer vision systems, editorial platforms.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/benyamin-mahamed)
[![Email](https://img.shields.io/badge/Email-benyaminmahamed%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:benyaminmahamed@gmail.com)

</div>

<br/>

## 🔭 Now building

|  |  |
|---|---|
| 🏀 **Basketball GM engine** | Possession-based Monte Carlo dynasty simulator, tuned phase-by-phase against real NBA statistical distributions (scoring, margins, pace), with a 1,000-game batch validation harness |
| ⚡ **Embedded CV performance** | Profiling where the milliseconds actually go in a classical vision loop on the Raspberry Pi 5 |

<br/>

## 🚢 Shipped

<div align="center">

<a href="https://github.com/BenyaminMahamed/AI-Research-Assistant">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=BenyaminMahamed&repo=AI-Research-Assistant&theme=github_dark&hide_border=true" alt="Lexis"/>
</a>
<a href="https://github.com/BenyaminMahamed/FINALYEARPROJECT">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=BenyaminMahamed&repo=FINALYEARPROJECT&theme=github_dark&hide_border=true" alt="Autonomous Navigation System"/>
</a>
<a href="https://github.com/BenyaminMahamed/blueprint-brief-architecture">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=BenyaminMahamed&repo=blueprint-brief-architecture&theme=github_dark&hide_border=true" alt="BluePrint Brief architecture"/>
</a>

</div>

<details open>
<summary><b>🧠 Lexis — AI Research Assistant</b></summary>
<br/>

A RAG pipeline built from scratch — no LangChain, no abstractions. PDFs are extracted page-by-page with PyMuPDF, chunked into 500-word overlapping windows, embedded with `all-MiniLM-L6-v2` (384-dim, normalised), and indexed in FAISS. Queries run nearest-neighbour search and pass the top-k chunks as grounded context to Gemini 2.0 Flash.

Four modes — Q&A, structured summarisation, peer-review critique, multi-paper comparison. Every answer surfaces the source chunks and page numbers it was based on. Built because tools like ChatPDF felt like black boxes with no source grounding.

**Stack:** Django · DRF · FAISS · Sentence-Transformers · PyMuPDF · Gemini 2.0 Flash · SQLite

</details>

<details open>
<summary><b>📰 The BluePrint Brief</b> — <i>private repo, live in production</i></summary>
<br/>

Co-founded this live editorial platform for legal and commercial content, and develop it as part of a three-person engineering team. A Django-powered editorial CMS — a lightweight version of what a newsroom would run internally.

My ownership: the Render deployment, the Cloudinary media layer, domain and email infrastructure, and primary production debugging. Shipped end-to-end: an access-gated Student Resources system, Beehiiv newsletter integration, and the submission notification pipeline. **1,000+ active users.** Architecture write-up: [blueprint-brief-architecture](https://github.com/BenyaminMahamed/blueprint-brief-architecture)

**Stack:** Django · PostgreSQL · JavaScript · HTML/CSS · Linux · Gunicorn

</details>

<details open>
<summary><b>🤖 Autonomous Navigation System</b> — <i>final year project</i></summary>
<br/>

Real-time lane following and obstacle detection on a Raspberry Pi 5, built as a proof-of-concept for affordable assistive mobility. The core question: can you replicate the navigation capabilities of £5,000+ commercial systems for under £200?

From a 10,298-frame integration session on physical hardware: **~10ms** average processing latency against a 200ms target (20× margin), **~14 FPS** sustained, **100%** obstacle detection reliability with zero false positives, manual override response under 10ms. All CPU-only, on-device, no cloud inference.

Deliberately Classical CV rather than deep learning — YOLOv5 on a Pi CPU costs 80–120ms per frame before anything else, and a probabilistic model can't guarantee the 100% detection reliability a safety-critical assistive system needs. A class-agnostic blob detector can, in under 5ms.

**Stack:** Python · OpenCV · NumPy · Picamera2 · Raspberry Pi 5 · PiCar-X SDK

</details>

<br/>

## 📊 Stats

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=BenyaminMahamed&show_icons=true&theme=github_dark&hide_border=true" height="165" alt="GitHub stats"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=BenyaminMahamed&layout=compact&theme=github_dark&hide_border=true" height="165" alt="Top languages"/>

<img src="https://streak-stats.demolab.com?user=BenyaminMahamed&theme=github-dark-blue&hide_border=true" height="165" alt="Contribution streak"/>

</div>

<br/>

## 🛠️ Stack

<details>
<summary><b>Languages</b></summary>
<br/>

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

</details>

<details>
<summary><b>AI / ML</b></summary>
<br/>

![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-%23FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=black)
![Google Gemini](https://img.shields.io/badge/Gemini-%234285F4.svg?style=for-the-badge&logo=google&logoColor=white)

</details>

<details>
<summary><b>Web & Backend</b></summary>
<br/>

![Django](https://img.shields.io/badge/django-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

</details>

<details>
<summary><b>Embedded, Security & Infrastructure</b></summary>
<br/>

![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557CF2?style=for-the-badge&logo=kali-linux&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-%23000000.svg?style=for-the-badge&logo=owasp&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)

</details>

<br/>

## 🐍 Contributions

<div align="center">
<img src="https://raw.githubusercontent.com/BenyaminMahamed/BenyaminMahamed/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake"/>
</div>

<br/>

<div align="center">

*Thanks for stopping by — the best way to reach me is [LinkedIn](https://linkedin.com/in/benyamin-mahamed) or [email](mailto:benyaminmahamed@gmail.com).*

</div>
