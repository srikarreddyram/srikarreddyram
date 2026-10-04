<a href="https://github.com/srikarreddyram">
  <img src="./images/banner.png" alt="Srikar Reddy, ML and Software Engineer" width="100%">
</a>

<p align="center">
  <a href="https://www.linkedin.com/in/srikarreddyram/"><img src="https://img.shields.io/badge/LinkedIn-srikarreddyram-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="mailto:srikarreddy.ram@gmail.com"><img src="https://img.shields.io/badge/Email-srikarreddy.ram%40gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://leetcode.com/u/srikar_reddy_/"><img src="https://img.shields.io/badge/LeetCode-srikar__reddy__-FFA116?style=flat-square&logo=leetcode&logoColor=white" alt="LeetCode"></a>
</p>

I'm **Ramachandra Tejsrikar Reddy (Srikar)**, a final-year Computer Science student at SRM Institute of Science and Technology and a Research Intern at the National Centre for Polar and Ocean Research (NCPOR). I build machine learning and backend systems with honest evaluation: held-out test sets, ablations, load tests, and results reported as measured, including the ones that didn't go my way.

- **Currently:** Research Intern at NCPOR, Goa, working on Arctic sea-ice forecasting from satellite climate data
- **Education:** B.Tech Computer Science, SRMIST, Chennai (2023 – 2027), CGPA 8.81
- **Research:** paper accepted in *Soft Computing* (Springer Nature); presented at the Fourth World Ocean Science Congress (WOSC 2026)
- **Open to:** software engineering, machine learning and data roles, including internships and 2027 graduate positions

---

## Experience

**Research Intern** · National Centre for Polar and Ocean Research (NCPOR), Goa · *Jun 2026 – Present*

- Benchmarked 10 forecasting models (LSTM, GRU, CNN-LSTM, ConvLSTM, XGBoost, Holt-Winters) for monthly Arctic sea ice across 12 regions at 1 to 12 month lead times, using satellite records back to 1979.
- Tested the proposed EMD + LSTM method against a no-decomposition baseline, and showed that non-causal EMD leaks future data into the inputs and inflates apparent skill.
- Built the dataset for a follow-up study on whether Arctic sea ice can help predict Indian heatwaves, and caught a 0.58 °C gap between two temperature sources (IMD and NOAA CPC) that could have produced a false signal.

---

## Selected Projects

### Machine learning and LLMs

| Project | Summary | Stack |
|:---|:---|:---|
| **[FinSight](https://github.com/srikarreddyram/FinSight)** | Citation-first RAG copilot over SEC filings. On FinanceBench (150 questions), hybrid search with a cross-encoder reranker raised **recall@10 from 41% to 81%** at **96% citation precision**, with **100% correct refusals** on unanswerable questions. The LLM never writes a number: Python checks every figure against its cited page. | Python, Gemini API, Qdrant, Docling, FastAPI, React |
| **[FraudGuard](https://github.com/srikarreddyram/fraud-guard)** | Fraud scoring for the Razorpay AI Buildathon 2026. **0.511 PR-AUC** on a time-split holdout of 590K transactions (about 15× random). Ranking cases by expected loss to fit analyst review capacity recovered **$77K (21.5%) more** from the same model. | Python, XGBoost, FastAPI, Redis, PostgreSQL, Docker |
| **[Shot Vision](https://github.com/srikarreddyram/Shot-Stat)** | Shot-quality and matchup models trained on **2.1M NBA shots**, served to a React app with TreeSHAP explanations in plain language. Features are point-in-time and shared between training and serving, enforced by a parity test. | Python, XGBoost, SHAP, DuckDB, FastAPI, React |
| **[RaceIQ](https://github.com/srikarreddyram/raceiq)** | Formula 1 strategy simulator driven by seven models trained on every race since 2018. On 15 unseen 2026 races it predicts finishing positions within **2.1 places** on average (rank correlation **0.87**). | Python, LightGBM, PyTorch, DuckDB, MLflow, FastAPI |

### Backend and systems

| Project | Summary | Stack |
|:---|:---|:---|
| **[SportsGateway](https://github.com/srikarreddyram/SportsGateway)** | API gateway over a live sports data feed. Under k6 load tests: **98.2% fewer upstream calls** at a 99.8% cache hit rate, **zero client errors** through a full provider outage, and throughput scaling from 2,746 to **7,249 req/s** across three replicas. | Node.js, Express, Redis, MongoDB, Nginx, Prometheus |
| **[Bellwether](https://github.com/srikarreddyram/bellwether)** | Progressive delivery platform that runs stable and canary builds of any repository side by side behind its own traffic proxy, promotes through nine stages, and rolls back automatically when canary latency or error rate crosses a threshold. | Python, React, WebSockets, Docker |
| **[TDMA Schedule Optimizer](https://github.com/srikarreddyram/tdma-schedule-optimizer)** | Conflict-free wireless slot scheduling via distance-2 graph colouring. Produces the provably minimal 9-slot frame on a 16-node grid; in an EMANE radio emulation it delivered **99.9% of packets with zero collisions**, against 34.5% for the 5-slot schedule given in the task. | Python, NetworkX, EMANE, Docker |
| **[SMTP Simulator](https://github.com/srikarreddyram/smtp-sim)** | SMTP and POP3 servers written from scratch on raw Java sockets with no external libraries: two mail domains, relaying, retries with back-off, bounces, SMTP AUTH and MIME, covered by 33 end-to-end tests. | Java, TCP sockets |

Also on GitHub: [ComplaintIQ](https://github.com/srikarreddyram/complaintiq) (in progress: Hadoop and Spark pipeline over 17.6M CFPB complaints) · [GreenCart](https://github.com/srikarreddyram/GreenCart) · [Apple Music Organizer](https://github.com/srikarreddyram/apple-music-organizer) · [AI Radar](https://github.com/srikarreddyram/AI_radar)

---

## Research and Publications

- **Optimizing Network Performance in LTE using Fuzzy Logic and MFO.** Accepted in *Soft Computing*, Springer Nature.
- **Fourth World Ocean Science Congress (WOSC 2026), Goa.** Represented SRMIST and presented research, February 2026.

---

## Technical Skills

| Area | Tools |
|:---|:---|
| Languages | Python, Java, TypeScript, JavaScript, SQL |
| Machine learning | XGBoost, LightGBM, PyTorch, SHAP, LSTM / ConvLSTM, time-series forecasting, MLflow |
| LLMs and retrieval | RAG, structured outputs, LLM-as-judge evaluation, Gemini API, Qdrant, hybrid search and reranking |
| Backend | FastAPI, Node.js, Express, React, SQLAlchemy, REST APIs |
| Data | PostgreSQL, Redis, MongoDB, DuckDB, SQLite, Spark, Hive |
| Infrastructure | AWS, Docker, Nginx, GitHub Actions, Prometheus, k6, Git |

---

## Certifications

| Credential | Issuer | Valid | |
|:---|:---|:---:|:---:|
| AWS Certified Solutions Architect – Associate | Amazon Web Services | 2026 – 2029 | [Verify](https://www.credly.com/badges/244fece6-a129-43ad-aae3-470401ba92e5) |
| AWS Certified Data Engineer – Associate | Amazon Web Services | 2026 – 2029 | [Verify](https://www.credly.com/badges/2e608a60-349e-48ab-bf50-5a5de4a609f0) |
| AWS Certified Cloud Practitioner | Amazon Web Services | 2026 – 2029 | [Verify](https://www.credly.com/badges/875fc7ec-9014-4951-94d7-e402f6baf15b) |
| OCI 2025 Certified Generative AI Professional | Oracle | 2026 – 2028 | [Verify](https://catalog-education.oracle.com/ords/certview/sharebadge?id=68F789E6FB1B545B93F366B25E5642F75B2B9CB2969794B3023E5B584623BB88) |

---

## Leadership

- **Organizing Head**, PASUMAI and BharatBuild Hackathons, SRMIST Startup Summit

---

## GitHub Activity

<p align="center">
  <img src="https://github-readme-stats-three-nu-85.vercel.app/api?username=srikarreddyram&show_icons=true&theme=github_dark&hide_border=true&count_private=true&include_all_commits=true&title_color=E3C16F&icon_color=E3C16F&text_color=c9d1d9&bg_color=0d1117" height="165" alt="GitHub stats">
  <img src="https://github-readme-stats-three-nu-85.vercel.app/api/top-langs/?username=srikarreddyram&layout=compact&theme=github_dark&hide_border=true&langs_count=8&title_color=E3C16F&text_color=c9d1d9&bg_color=0d1117" height="165" alt="Top languages">
</p>

<details>
<summary>LeetCode</summary>
<br>
<p align="center">
  <a href="https://leetcode.com/u/srikar_reddy_/"><img src="https://leetcard.jacoblin.cool/srikar_reddy_?theme=dark&font=Inter&ext=heatmap" alt="LeetCode stats"></a>
</p>
</details>
