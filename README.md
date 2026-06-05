# Hey, I'm Benyamin

CS Graduate based in London. I spend most of my time building things that sit at the intersection of backend engineering and AI — RAG pipelines, computer vision systems, editorial platforms. 

Currently looking for junior backend / AI engineering roles.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/benyamin-mahamed)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?style=for-the-badge&logo=github)](https://github.com/BenyaminMahamed)

---

## What I'm working on

- **Lexis** — a full-stack RAG research assistant. The interesting parts: semantic chunking with overlapping windows, FAISS inner-product similarity search, and a multi-mode LLM layer (Q&A, summarise, critique, compare) that always cites the exact chunks it used. Built it because existing tools like ChatPDF felt like black boxes with no source grounding.
- Exploring Physics-Informed Neural Networks — applying physics-aware loss constraints to neural nets for scientific imaging problems
- Squeezing more performance out of embedded CV pipelines — currently at sub-3ms latency on a Pi 5, trying to push further

---

## What I've shipped

### [Lexis — AI Research Assistant](https://github.com/BenyaminMahamed/AI-Research-Assistant)

A RAG pipeline I built from scratch — no LangChain, no abstractions, just the raw pipeline. PDFs go in, get extracted page-by-page with PyMuPDF, chunked into 500-word overlapping windows, embedded with `all-MiniLM-L6-v2` (384-dim, normalised), and indexed in FAISS. Queries hit the same embedding model, do nearest-neighbour search, retrieve the top-k chunks, and pass them as grounded context to Gemini 2.0 Flash.

Four modes: Q&A, structured summarisation, peer-review style critique, and multi-paper comparison. Every answer surfaces the source chunks and page numbers it was based on — no hallucination hiding behind vague responses.

**Stack:** Django, DRF, FAISS, Sentence-Transformers, PyMuPDF, Gemini 2.0 Flash, SQLite

---

### [The BluePrint Brief](https://theblueprintbrief.com) *(Private Repo)*

Co-founded this and built the entire platform as lead developer. It's a Django-powered editorial CMS — think a lightweight version of what a newsroom would run internally. Built custom role-based access control from scratch (writer, editor, admin tiers), an editorial workflow system, automated SEO metadata generation, and integrated analytics tracking.

Currently serving 1,000+ active users. The interesting engineering challenge was building a content delivery system that stays fast under real traffic without reaching for a CDN or expensive infrastructure — solved mostly through query optimisation and aggressive caching at the Django layer.

Can be viewed from an architecture standpoint at [The BluePrint Brief Architecture](https://github.com/BenyaminMahamed/blueprint-brief-architecture)

**Stack:** Django, PostgreSQL, JavaScript, HTML/CSS, Linux

---

### [[Autonomous Driving Prototype](https://github.com/BenyaminMahamed/Autonomous-Self-Driving-Car)](https://github.com/BenyaminMahamed/Autonomous-Driving-Prototype)

Real-time lane detection and obstacle avoidance running on a Raspberry Pi 5. The target was 60 FPS — ended up hitting 70+ FPS at 2.25ms latency, which on a Pi is genuinely not supposed to be possible. Got there through frame pipeline optimisation, model quantisation, and being very aggressive about cutting anything that wasn't doing useful work in the inference loop.

Built with OpenCV and PyTorch. The computer vision pipeline handles lane boundary detection, obstacle classification, and real-time steering decisions — all on-device, no cloud inference.

**Stack:** Python, OpenCV, PyTorch, Raspberry Pi 5, Arduino

---

## Stack

### Languages
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white)
![SQL](https://img.shields.io/badge/sql-%2300758F.svg?style=for-the-badge&logo=mysql&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![Bash](https://img.shields.io/badge/bash-%23121011.svg?style=for-the-badge&logo=gnu-bash&logoColor=white)

### AI / ML
![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=for-the-badge&logo=opencv&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-%23FFD21E.svg?style=for-the-badge&logo=huggingface&logoColor=black)
![Google Gemini](https://img.shields.io/badge/Gemini-%234285F4.svg?style=for-the-badge&logo=google&logoColor=white)

### Web & Backend
![Django](https://img.shields.io/badge/django-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Django REST Framework](https://img.shields.io/badge/DRF-%23092e20.svg?style=for-the-badge&logo=django&logoColor=white)
![Bootstrap](https://img.shields.io/badge/bootstrap-%238511FA.svg?style=for-the-badge&logo=bootstrap&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)

### Embedded & IoT
![Raspberry Pi](https://img.shields.io/badge/-RaspberryPi-C51A4A?style=for-the-badge&logo=Raspberry-Pi)
![Arduino](https://img.shields.io/badge/-Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white)

### Security & Infrastructure
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557CF2?style=for-the-badge&logo=kali-linux&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=for-the-badge&logo=wireshark&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP-%23000000.svg?style=for-the-badge&logo=owasp&logoColor=white)
![Git](https://img.shields.io/badge/git-%23F05033.svg?style=for-the-badge&logo=git&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)


---

## Contact

[![LinkedIn](https://img.shields.io/badge/LinkedIn-benyamin--mahamed-blue?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/benyamin-mahamed)
[![Email](https://img.shields.io/badge/Email-benyaminmahamed%40gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:benyaminmahamed@gmail.com)
