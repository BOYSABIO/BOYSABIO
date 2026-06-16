<div align="center">

## Spencer Wood

**ML Engineer & Builder**  
Deep Learning · Agentic AI Systems · Security Analytics · Data Engineering

Master's in Business Analytics & Data Science — IE Madrid

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/spencersvedawood/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:spencer@jsveda.com)

</div>

---

## About

I've been taking things apart since I was a kid. I fried the motherboard of my first PC at 10, rebuilt it out of necessity, and that loop — break → understand → rebuild — never really stopped.

At some point my ML and deep learning work started pulling toward the same place as my obsession with networks and systems. So I built a homelab the right way: OPNsense firewall, proper VLANs, Proxmox virtualization, isolated malware environments. Not to configure tools others built — to understand how infrastructure actually works from the inside. That gave me real data. Then I applied ML and DL to it: network traffic classification, multi-class attack detection, anomaly signals from flow features. Then I built a LangGraph agent to reason over those signals at scale. That's the stack I work in now — real infrastructure at the bottom, ML/DL in the middle, agentic reasoning on top.

Alongside that I shipped an AI-powered product from scratch — a language learning platform — from idea to live deployment, currently in pilot with real users.

I spent roughly half my life in the US and half in Europe, which forced me to adapt fast and think in systems. I care about solutions that close real feedback loops and that push toward technical mastery. I'll usually take the harder path first — understanding the long route makes the shortcuts obvious.

<table>
  <tr>
    <td valign="top" width="50%">

**What I build**

- ML & deep learning pipelines — from raw signals to production inference
- Agentic systems — multi-step LLM-backed reasoning loops (LangGraph)
- Security analytics infrastructure — network monitoring, traffic classification, alert triage
- Data platforms — lakehouse architecture, streaming, observability

    </td>
    <td valign="top" width="50%">

**Current focus**

- SOC Triage Agent — LangGraph multi-step agent for security alert reasoning
- Network Monitoring → SOC Agent — end-to-end security ML pipeline
- AI product development — language learning platform in live pilot
- Expanding agentic AI and multi-step reasoning depth

    </td>
  </tr>
</table>

**Stack**  
Python, R, SQL · PyTorch, TensorFlow, scikit-learn, LangChain, LangGraph · MLflow, W&B, Docker · PySpark, Databricks, Kafka · Linux, networking, Zeek, Wireshark

---

## Featured projects

### The Security ML Stack — Homelab → Network Monitoring → SOC Triage Agent
**Infrastructure · ML/DL · Agentic Reasoning — built layer by layer**

Three connected projects that form a complete, end-to-end system. Each layer was built intentionally — not as a portfolio exercise, but to actually run in real infrastructure and solve a real problem.

**Layer 1 — [Homelab](https://github.com/BOYSABIO/homelab)**  
OPNsense firewall, VLANs, Proxmox hypervisor, isolated malware testing environments, IDS/IPS. Built from scratch to understand how infrastructure works from the inside — not to configure other people's tools.

**Layer 2 — [Network Monitoring & Traffic Analysis](https://github.com/BOYSABIO/Network-Monitoring)**  
PCAP capture → flow feature extraction → ML/DL classifier (~80% accuracy on benign/malicious classification, multi-class attack detection) → clean ndjson output. Runs against the homelab. Data pipeline feeds Layer 3.

**Layer 3 — [SOC Triage Agent](https://github.com/BOYSABIO/SOC-Triage-Agent)**  
LangGraph multi-step agent. Ingests ndjson alerts from Layer 2, uses an LLM-backed reasoning loop to look up context, enrich, and produce structured triage decisions — reducing analyst toil on L1 work.

Three layers. Real infrastructure. Real data. Real inference.

---

### Huckleberry Habitat Suitability Model (Microsoft Capstone)
**Enterprise ML + creative problem framing**

Challenge: *"Monetize Microsoft GridMET climate data."* Delivered a feasibility study predicting huckleberry habitat suitability for ecological and commercial stakeholders. ~450GB of environmental and location data, >90% accuracy, versioned artifacts, confidence outputs, and interactive habitat maps.

Awarded **honors**. Dean's List capstone.

[🔗 Huckleberry Habitat Suitability Model](https://github.com/BOYSABIO/Huckleberry-Habitat-Suitability-Model)

---

### Modular MLOps Pipeline (MNIST)
**Engineering-heavy ML system**

Refactored a simple MNIST CNN notebook into a full production-style ML pipeline. The point isn't MNIST — it's the engineering: modular config management, experiment tracking with MLflow, REST API, CI/CD, Docker. Shows how I think about maintainable, deployment-ready systems.

[🔗 MLOps](https://github.com/BOYSABIO/MLOps)

---

### Audio Fingerprinting & Matching Pipeline
**Large-scale distributed system**

Full-scale Shazam-inspired fingerprinting and matching system. Bronze → Silver → Gold lakehouse architecture on Databricks. Extracts audio from YouTube, fingerprints via Librosa, hashes and matches query clips against a song database with confidence scores.

[🔗 Audio Fingerprinting & Matching Pipeline](https://github.com/BOYSABIO/Audio-Fingerprinting-Matching-Pipeline)

---

<details>
  <summary><b>📂 Full project catalogue by domain</b></summary>

<br>

### Security & Infrastructure

- **[Homelab](https://github.com/BOYSABIO/homelab)** — OPNsense, VLANs, Proxmox, IDS/IPS, isolated malware testing. Foundation for the security ML stack.
- **[Network Monitoring & Traffic Analysis Lab](https://github.com/BOYSABIO/Network-Monitoring)** — PCAP → flow features → ML/DL classifier → ndjson; feeds SOC Triage Agent
- **SOC Triage Agent** *(private — in progress)* — LangGraph multi-step agent for security alert triage; consumes Network Monitoring output

### Machine Learning & AI

- **[Huckleberry Habitat Suitability Model](https://github.com/BOYSABIO/Huckleberry-Habitat-Suitability-Model)** — Microsoft-supported capstone; environmental ML predicting huckleberry habitat from ~450GB of GridMET climate data. Honors.
- **[Predicting Hotel Cancellations](https://github.com/BOYSABIO/Hotel-Cancellations-Prediction-Model)** — Ensemble ML for booking cancellation prediction with feature engineering and optimization
- **[CO₂ Emissions Forecast Model](https://github.com/BOYSABIO/CO2-Emission-Forecast-Model)** — Time-series forecasting of global flight CO₂ emissions using advanced statistical methods
- **[Marketing Mix Model](https://github.com/BOYSABIO/Marketing-Mix-Model)** — Marketing attribution and ROI analysis using statistical modeling

### Big Data & Data Engineering

- **[Audio Fingerprinting & Matching](https://github.com/BOYSABIO/Audio-Fingerprinting-Matching-Pipeline)** — Shazam-inspired system; Bronze → Silver → Gold lakehouse on Databricks + PySpark

### MLOps

- **[MNIST MLOps Pipeline](https://github.com/BOYSABIO/MLOps)** — Production-style ML pipeline: Docker, MLflow, CI/CD, REST API, modular config management

### Computer Vision

- **[Pool Detection CNN](https://github.com/BOYSABIO/Pool-Detection-CNN)** — YOLO-based object detection on satellite imagery; includes oriented bounding boxes (OBB) to fit pools of any shape or angle
- **[Screen Snooper Detector](https://github.com/BOYSABIO/Screen-Snooper-Detection)** — Real-time CV model detecting if someone is looking at your screen; multi-person detection with false-positive filtering

### Algorithmic Trading & Finance

- **[Stock Price Prediction Dashboard](https://github.com/BOYSABIO/Stock-Analysis-Prediction-Dashboard)** — Real-time stock analysis and prediction dashboard (Streamlit)
- **[Asset Price Path Simulator](https://github.com/BOYSABIO/Asset-Price-Path-Sim)** — Asset price simulation using Bachelier & Samuelson models
- **[Order Book Simulation](https://github.com/BOYSABIO/orderbook-simulation)** — High-performance limit order book simulation using real LOB messages for market microstructure analysis
- **[ARCH/GARCH Volatility Modeling](https://github.com/BOYSABIO/OM-group-project-2)** — Volatility models applied to CrowdStrike stock data

### Reinforcement Learning

- **[Lunar Lander & Car Racing](https://github.com/BOYSABIO/DQN-DDQN-Gymnasium)** — DQN and DDQN agents on Gymnasium control tasks

</details>

---

## Skill stack

<details>
  <summary><b>📂 Languages, frameworks, and tools</b></summary>

<br>

### Programming Languages

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![R](https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-000000?style=for-the-badge&logo=mysql&logoColor=white)

### Machine Learning & Deep Learning

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)

### Agentic AI & LLMs

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white)

### MLOps & Experiment Tracking

![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white)
![Weights & Biases](https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=for-the-badge&logo=weightsandbiases&logoColor=black)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)

### Data & Infrastructure

![Apache Spark](https://img.shields.io/badge/Apache_Spark-E25A1C?style=for-the-badge&logo=apache-spark&logoColor=white)
![Databricks](https://img.shields.io/badge/Databricks-FF3621?style=for-the-badge&logo=databricks&logoColor=white)
![Kafka](https://img.shields.io/badge/Apache%20Kafka-231F20?style=for-the-badge&logo=apache-kafka&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0089D6?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Apache NiFi](https://img.shields.io/badge/Apache%20NiFi-0081C6?style=for-the-badge&logo=apache-nifi&logoColor=white)

### Visualization

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)
![PowerBI](https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=tableau&logoColor=white)

</details>

---

## Learning & notes

<details>
  <summary><b>📂 Open notes & learning repositories</b></summary>

<br>

- **[Masters Data Science — IE University](https://github.com/BOYSABIO/IE-University)** — Academic projects and coursework
- **[CompTIA Security+ Study Notes](https://github.com/BOYSABIO/CompTIA-SecurityPlus-Notes)** — *In progress*

</details>

---

## GitHub activity

<details>
  <summary><b>📂 Stats</b></summary>

<br>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=BOYSABIO&theme=radical" alt="GitHub Streak Stats">
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=BOYSABIO&show_icons=true&theme=radical" width="450px">
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=BOYSABIO&layout=compact&theme=radical" width="450px">
</p>

</details>

---

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/spencersvedawood/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:spencer@jsveda.com)

**Email:** spencer@jsveda.com · **LinkedIn:** [Spencer Wood](https://www.linkedin.com/in/spencersvedawood/)

![Profile Views](https://komarev.com/ghpvc/?username=BOYSABIO&color=red&style=flat-square)

</div>
