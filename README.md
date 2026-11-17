<div align="center">

<img src="assets/header.svg" width="100%" alt="Spencer Wood — ML Engineer &amp; Builder"/>

<img src="assets/tagline.svg" width="100%" alt="how hard could it be?"/>

</div>

I've been taking things apart since I was a kid. I fried the motherboard of my first PC at 10, rebuilt it out of necessity, and that loop — break → understand → rebuild — never really stopped.

These days it shows up as a refusal to rent the layer below the one I need. I built a small enterprise network in a spare room to see what traffic actually does, put models on top of it, then services on top of those. Lately it has turned outward: businesses that have no data at all, where the thing they need isn't for sale. So I build the whole stack — the capture that creates the record, the schema that holds it, the models that read it, and the screens the people running the place actually touch.

On the way I taught an AI to land a rocket, rebuilt Shazam from scratch, and mapped where a fruit grows that nobody can farm. Half my life in the US, half in Europe. I still take the long route first — it's what makes the shortcuts obvious.

<br>

<img src="assets/sec-now.svg" width="100%" alt="01 · Now"/>

<div align="center">
<a href="https://github.com/BOYSABIO/muttmetrics"><img src="assets/card-muttmetrics.svg" width="32%" alt="MuttMetrics — in production. The data layer for a dog-grooming business."/></a>
<img src="assets/card-cveda.svg" width="32%" alt="Cveda — piloted, iterating. Private language-learning platform."/>
<img src="assets/card-examguard.svg" width="32%" alt="ExamGuard — client project, ML phase. Proctoring that flags, never removes."/>
</div>

<details>
<summary><sub>The longer version of all three</sub></summary>
<br>

**[MuttMetrics](https://github.com/BOYSABIO/muttmetrics)** — I run the technical side of a dog-grooming salon: the site, the database, the backend, the interfaces the people there use, and the analytics on top. MuttMetrics is the layer underneath: owner and dog records, breed and service priors, and a model of how long the work really takes by breed, coat condition and service. It has run in production on its own server since November, with grooms logged from the salon floor. A groom that runs an hour long isn't a scheduling problem, it's a margin problem — and until it's measured nobody knows which jobs are paying for themselves.

**Cveda** 🔒 — A full product, built end to end and deployed: vocabulary tracking with morphology awareness, a document editor with click-to-translate, teacher–student collaboration, practice tools, analytics. Piloted with six tutors and their students, now iterating on what they actually did with it. Private because it's a product rather than a portfolio piece — which is the point.

**ExamGuard** 🔒 — A modular proctoring layer running alongside Safe Exam Browser. Client-side webcam inference — phone detection, gaze estimation, multi-person detection — producing timestamped flags with confidence scores. It never removes a student; it only flags. Ring-buffer clip upload keeps bandwidth sane, professors review and label in a dashboard, and those labels feed a fine-tuning loop.

</details>

<br>

<img src="assets/sec-stack.svg" width="100%" alt="02 · The stack I own"/>

<img src="assets/stack-pipeline.svg" width="100%" alt="Homelab → Network Monitoring → SOC Triage Agent; MuttMetrics, the Huckleberry API and a Discord bot also run on the homelab"/>

**[Homelab](https://github.com/BOYSABIO/homelab)** · **[Network Monitoring](https://github.com/BOYSABIO/Network-Monitoring)** · **[SOC Triage Agent](https://github.com/BOYSABIO/SOC-Triage-Agent)** — three repos, one system, each built because the one below it made it possible. The homelab doubles as the deployment target for everything above. The interesting problem in the agent isn't security, it's architecture: when to gate, what context to fetch, how to make a model's output land as a decision rather than a paragraph.

<br>

<img src="assets/sec-shipped.svg" width="100%" alt="03 · Shipped"/>

| | |
|---|---|
| **[Huckleberry Habitat Model](https://github.com/BOYSABIO/Huckleberry-Habitat-Suitability-Model)** <br><sub>Microsoft capstone · honors</sub> | The brief was *"monetize Microsoft GridMET climate data."* ~450GB of environmental data became a >90%-accuracy habitat model, then a service you can call: FastAPI `/predict` with per-tree confidence intervals, an MLflow registry, Docker, CI, hosted on the homelab. |
| **[Audio Fingerprinting](https://github.com/BOYSABIO/Audio-Fingerprinting-Matching-Pipeline)** <br><sub>Shazam, rebuilt</sub> | Bronze → Silver → Gold lakehouse on Databricks, PySpark fingerprint hashing, confidence-scored matching. |
| **[Screen Snooper Detection](https://github.com/BOYSABIO/Screen-Snooper-Detection)** <br><sub>computer vision</sub> | Catches someone reading over your shoulder in real time: YOLOv8 + MediaPipe gaze, a custom dataset labeled with Grounding DINO, primary-user exclusion. |
| **[Modular MLOps Pipeline](https://github.com/BOYSABIO/MLOps)** <br><sub>where production started</sub> | A simple CNN rebuilt as a production system: modular steps, Hydra config, MLflow + W&B, containerized FastAPI serving, pytest and CI. |

<br>

<img src="assets/sec-parked.svg" width="100%" alt="04 · Parked"/>

**LLM-Lab** 🔒 &nbsp;![parked](https://img.shields.io/badge/parked_·_Nov_2026-414868?style=flat-square)
The pipeline the frontier labs run, rebuilt to understand it from the inside: data curation → pre-training → SFT → DPO → evals → inference optimization. Designed end to end, with a proxy ladder (1M → 100M params) for cheap ablations before anything big gets trained. It reached a working nanoGPT, then I parked it — it's the first one back when a slot frees.

<br>

<img src="assets/sec-tools.svg" width="100%" alt="05 · Toolbox"/>

<div align="center">

<img src="https://skillicons.dev/icons?i=py,ts,r,pytorch,tensorflow,sklearn,fastapi,postgres,prisma&theme=dark" alt="Python, TypeScript, R, PyTorch, TensorFlow, scikit-learn, FastAPI, PostgreSQL, Prisma"/>
<br>
<img src="https://skillicons.dev/icons?i=docker,githubactions,linux,azure,kafka,nextjs,react,nodejs,vercel&theme=dark" alt="Docker, GitHub Actions, Linux, Azure, Kafka, Next.js, React, Node.js, Vercel"/>

<sub>plus LangGraph · Hugging Face · TRL · vLLM · MLflow · W&amp;B · PySpark · Databricks · Proxmox · OPNsense · Zeek · YOLOv8 · MediaPipe</sub>

</div>

<details>
<summary><sub><b>The full list</b></sub></summary>
<br>
<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-414868?style=flat-square) ![R](https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=black) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![Hugging Face](https://img.shields.io/badge/Hugging_Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![YOLOv8](https://img.shields.io/badge/YOLOv8-414868?style=flat-square) ![MediaPipe](https://img.shields.io/badge/MediaPipe-414868?style=flat-square) ![Grounding DINO](https://img.shields.io/badge/Grounding_DINO-414868?style=flat-square) ![Gymnasium](https://img.shields.io/badge/Gymnasium-414868?style=flat-square) ![Librosa](https://img.shields.io/badge/Librosa-414868?style=flat-square) ![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square) ![TRL](https://img.shields.io/badge/TRL-414868?style=flat-square) ![PEFT](https://img.shields.io/badge/PEFT-414868?style=flat-square) ![vLLM](https://img.shields.io/badge/vLLM-414868?style=flat-square) ![lm-eval-harness](https://img.shields.io/badge/lm--eval--harness-414868?style=flat-square) ![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white) ![Weights & Biases](https://img.shields.io/badge/Weights_%26_Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white) ![Hydra](https://img.shields.io/badge/Hydra-414868?style=flat-square) ![pytest](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white) ![Ruff](https://img.shields.io/badge/Ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white) ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white) ![Alembic](https://img.shields.io/badge/Alembic-414868?style=flat-square) ![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=flat-square&logo=prisma&logoColor=white) ![Neon](https://img.shields.io/badge/Neon-00E599?style=flat-square&logo=neon&logoColor=black) ![Node.js](https://img.shields.io/badge/Node.js-5FA04E?style=flat-square&logo=nodedotjs&logoColor=white) ![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=flat-square&logo=databricks&logoColor=white) ![Apache Kafka](https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white) ![Apache NiFi](https://img.shields.io/badge/Apache_NiFi-728E9B?style=flat-square&logo=apachenifi&logoColor=white) ![Azure](https://img.shields.io/badge/Azure-0089D6?style=flat-square&logo=microsoftazure&logoColor=white) ![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white) ![Proxmox](https://img.shields.io/badge/Proxmox-E57000?style=flat-square&logo=proxmox&logoColor=white) ![OPNsense](https://img.shields.io/badge/OPNsense-D94F00?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black) ![MinIO / S3](https://img.shields.io/badge/MinIO_%2F_S3-C72E49?style=flat-square&logo=minio&logoColor=white) ![Zeek](https://img.shields.io/badge/Zeek-414868?style=flat-square) ![Wireshark](https://img.shields.io/badge/Wireshark-1679A7?style=flat-square&logo=wireshark&logoColor=white) ![PCAP analysis](https://img.shields.io/badge/PCAP_analysis-414868?style=flat-square) ![IDS/IPS](https://img.shields.io/badge/IDS%2FIPS-414868?style=flat-square) ![VLAN segmentation](https://img.shields.io/badge/VLAN_segmentation-414868?style=flat-square) ![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white) ![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black) ![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white) ![CSS Modules](https://img.shields.io/badge/CSS_Modules-000000?style=flat-square&logo=cssmodules&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

</div>
</details>

---

<details>
<summary><sub><b>Archives</b> &nbsp;·&nbsp; every other project, by domain</sub></summary>
<br>

**Products**

- **[MuttMetrics](https://github.com/BOYSABIO/muttmetrics)** — the data and prediction layer for a working dog grooming salon; capture-first design, Postgres + FastAPI
- **Cveda** 🔒 — AI-assisted platform for tutors and students; Next.js, Prisma, Neon, Vercel
- **ExamGuard** 🔒 — proctoring layer for Safe Exam Browser; human-in-the-loop review, fine-tuning flywheel
- **[Discord Music Bot](https://github.com/BOYSABIO/discord-music-bot)** — self-hosted; Lavalink v4, Riffy, Docker Compose, deployed to its own homelab container

**Machine Learning & AI**

- **LLM-Lab** 🔒 — full model pipeline from scratch: curation, pre-training, SFT, DPO, evals, inference optimization *(parked)*
- **[Huckleberry Habitat Suitability Model](https://github.com/BOYSABIO/Huckleberry-Habitat-Suitability-Model)** — Microsoft capstone, ~450GB GridMET data, honors; extended into a deployed FastAPI service with MLflow registry, Docker, CI, homelab hosting
- **[Predicting Hotel Cancellations](https://github.com/BOYSABIO/Hotel-Cancellations-Prediction-Model)** — ensemble ML with feature engineering and optimization
- **[CO₂ Emissions Forecast](https://github.com/BOYSABIO/CO2-Emission-Forecast-Model)** — time-series forecasting of global flight emissions

**Systems & Security**

- **[Homelab](https://github.com/BOYSABIO/homelab)** — OPNsense, VLANs, Proxmox, IDS/IPS, isolated malware testing. Foundation and deployment target for everything above.
- **[Network Monitoring & Traffic Analysis](https://github.com/BOYSABIO/Network-Monitoring)** — PCAP → flow features → ML/DL classifier → ndjson; feeds the triage agent
- **[SOC Triage Agent](https://github.com/BOYSABIO/SOC-Triage-Agent)** — LangGraph agent: alert gating, case briefs, tool-calling reasoning loop, structured verdicts

**MLOps & Data Engineering**

- **[MNIST MLOps Pipeline](https://github.com/BOYSABIO/MLOps)** — modular pipeline steps, Hydra config, MLflow + W&B, containerized FastAPI serving, pytest + CI
- **[Audio Fingerprinting & Matching](https://github.com/BOYSABIO/Audio-Fingerprinting-Matching-Pipeline)** — Shazam-inspired at scale: Bronze → Silver → Gold lakehouse on Databricks, PySpark fingerprint hashing, confidence-scored matching

**Computer Vision**

- **[Pool Detection CNN](https://github.com/BOYSABIO/Pool-Detection-CNN)** — YOLO on satellite imagery, with oriented bounding boxes that rotate to fit pools of any shape
- **[Screen Snooper Detection](https://github.com/BOYSABIO/Screen-Snooper-Detection)** — real-time detection of someone reading your screen; YOLOv8 + MediaPipe gaze, custom dataset labeled with Grounding DINO, primary-user exclusion
- **[Image to ASCII](https://github.com/BOYSABIO/Image-to-Ascii)** — image → ASCII art converter, built because the manual process annoyed me

**Quantitative Finance**

- **[Stock Analysis & Prediction Dashboard](https://github.com/BOYSABIO/Stock-Analysis-Prediction-Dashboard)** — real-time analysis and prediction (Streamlit)
- **[Asset Price Path Simulator](https://github.com/BOYSABIO/Asset-Price-Path-Sim)** — Bachelier and Samuelson models
- **[ARCH/GARCH Volatility Modeling](https://github.com/BOYSABIO/OM-group-project-2)** — volatility models on CrowdStrike data

**Reinforcement Learning**

- **[Lunar Lander & Car Racing](https://github.com/BOYSABIO/DQN-DDQN-Gymnasium)** — DQN and DDQN agents on Gymnasium control tasks

🔒 = private repository. Happy to walk through any of these in a conversation.

</details>

<details>
<summary><sub><b>Notes</b> &nbsp;·&nbsp; coursework and study notes, in public</sub></summary>
<br>

- **[MSc Data Science — IE University](https://github.com/BOYSABIO/IE-University)** — coursework and academic projects
- **[CompTIA Security+ Notes](https://github.com/BOYSABIO/CompTIA-SecurityPlus-Notes)** — *in progress*

</details>

---

<div align="center">

**Conviction comes from contact. Everything here is something I got into before I was ready.**

[![Portfolio](https://img.shields.io/badge/Portfolio-1a1b27?style=flat-square&logo=vercel&logoColor=white)](https://spencerwood-site.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/spencersvedawood/)
[![Email](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:spencer@jsveda.com)

</div>
