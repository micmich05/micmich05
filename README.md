# Micol Michanie

**AI Engineer & Technical Lead** · Machine Learning · Mathematical Optimization · Applied AI

**AI Lead, Payments @ Rappi** · **B.Eng. in AI Engineering @ Universidad de San Andrés**

[LinkedIn](https://www.linkedin.com/in/micol-michanie-2556bb23a/) · [Email](mailto:micolmichanie@gmail.com) · [GitHub](https://github.com/micmich05)

I lead a six-person AI team in Rappi's Payments organization, building machine learning systems, AI agents, and process automation across nine Latin American countries. My work sits at the intersection of **engineering, mathematical reasoning, and real operational problems**—from deploying ML systems to solving constrained optimization problems.

Alongside industry work, I'm interested in **representation learning, dynamical systems, and the mathematical foundations of machine learning**. I have presented technical projects at **SCIAA in 2024 and 2025** and regularly speak about applied AI to academic and industry audiences.

---

## Featured work

### [Bonsai · Certified near-optimal packaging optimization](https://github.com/micmich05/bonsai-packaging-optimization)
**Mathematical optimization · OR-Tools CP-SAT · MILP · Python** | AlixPartners Data Challenge 2026

Redesigned a packaging catalog for **427 products across five plants**, jointly optimizing box dimensions, product assignments, freight, and volume discounts under physical and logistical constraints. Reduced the search to a finite candidate space without excluding an optimum, then solved the resulting integer optimization problem with CP-SAT.

**Outcome:** **55 box types instead of 204**, with **$21.2M in estimated annual savings (10.1%)** and a **certified 0.018% optimality gap**. Received special recognition in the AlixPartners challenge. The repository includes a solution validator, tests, and the full business report.

### [Oil & Gas · Production forecasting platform](https://github.com/tommycass/oil-production-forecasting-platform)
**Time-series ML · Data engineering · MLOps · FastAPI** | Collaborative engineering project, 2026

Co-developed an end-to-end platform for monthly, **well-level oil and gas production forecasting** using real Argentine energy data. Built around a Medallion data architecture with **Dagster, dbt, PostgreSQL, an offline feature store, MLflow model registry, automated retraining, and REST inference**. The ML pipeline uses time-aware validation, leakage-safe features, model selection, and recursive forecasts up to 12 months ahead.

**Outcome:** the selected Random Forest models outperformed persistence baselines on held-out data, achieving **test R² = 0.868 for oil** and **0.850 for gas**. The platform also includes BI, data quality checks, containerization, CI/CD, and monitoring.

### [Koopman-JEPA · Learning latent temporal dynamics](https://github.com/micmich05/koopman-jepa)
**Representation learning · Dynamical systems · Koopman operators · PyTorch** | Exploratory research, 2026

Investigating whether a temporal joint-embedding predictive architecture can learn **nontrivial linear dynamics in latent space**, rather than only invariant representations. Controlled synthetic experiments keep observation distributions fixed while changing the underlying temporal transition law.

**Finding so far:** the learned predictor distinguished static, cyclic, and independent dynamics across **10/10 seeds per condition** and recovered their characteristic active spectra. The repository documents assumptions, reproduction steps, results, and limitations; these are controlled experimental findings, **not a general claim of Koopman recovery**.

### Traffic signal optimization · San Nicolás, Argentina
**Computer vision · Simulation · Simulated annealing · SUMO · YOLOv8** | Municipality of San Nicolás, 2024–2025

Developed a traffic signal optimization workflow using vehicle counts extracted from real camera footage, a simulated corridor, and multi-objective search over traffic-light phases and offsets.

**Outcome:** **22% higher average vehicle speed** and **35% fewer stops in simulation**. The project was presented at **SCIAA 2025** and covered by local news outlets.

**Additional projects:** RGB–thermal wildlife detection with YOLO; autonomous TurtleBot4 navigation using SLAM, sensor fusion, A* and Pure Pursuit; used-SUV price prediction from marketplace listings (**test R² = 0.94**).

---

## Professional experience

**AI Lead — Rappi, Payments** · Oct 2025–present  
Lead a team of six delivering ML systems, AI agents, and automation for payment operations across nine Latin American countries. Own technical prioritization and execution, collaborate with Product and Operations, and support recruiting and mentoring.

**AI Engineer & Consultant — Municipality of San Nicolás** · Dec 2024–present  
Develop computer vision and optimization solutions for municipal workflows. Delivered ML-assisted labeling that reduced manual work by **over 90%** and advised on optimization initiatives that reduced service wait times by **over 40%**.

**Business Data Analyst — MSD (Merck Sharp & Dohme)** · Jan–Sep 2025  
Automated data validation and fuzzy record-matching workflows using Python, Pandas, and RapidFuzz, improving efficiency in previously manual processes.

---

## Education & research interests

**Universidad de San Andrés** — B.Eng. in Artificial Intelligence Engineering (2023–2027) · **GPA 9.66/10**  
Teaching Assistant, **Algorithms & Data Structures** and **Systems Dynamics**.

**Vrije Universiteit Amsterdam** — Exchange studies, 2026–2027  
Coursework in dynamical systems and stochastic processes.

Current technical interests: **applied mathematics, dynamical systems, representation learning, optimization, and interpretable latent dynamics**.

---

## Speaking & scientific presentations

### Scientific presentations

**SCIAA — Scientific Symposium on Artificial Intelligence and Applications** · **2024 & 2025**  
Selected as a speaker in two editions to present technical projects:
- **2025 — Traffic signal optimization:** computer vision, SUMO simulation, and simulated annealing for a city traffic corridor, with **22% higher mean speed and 35% fewer stops in simulation**.
- **2024 — Gomoku game-playing agent:** minimax, alpha-beta pruning, search optimizations, and benchmarking against Monte Carlo Tree Search under time constraints.

### Industry talks, webinars & panels

- **L’Oréal LATAM — Beauty Tech Month:** invited talk on language models and AI agents, covering how LLMs work, agent architectures, context, tools, and levels of autonomy.
- **University of Buenos Aires — Y-Hat:** talk on applied AI in Payments.
- **Data Science Research Perú — Machine Learning Webinar:** practical ML design, from feature engineering and leakage prevention to preprocessing and model selection.
- **Data Science Research Perú — AI Panel:** AI-first organizations, automation, emerging talent needs, and the future of work.
- **RedLazo — *dIA a dIA* podcast:** AI agents and practical perspectives on applied AI.

---

## Selected recognition

- **AlixPartners Data Challenge (2026)** — Special recognition for the packaging optimization solution, with **$21.2M in estimated annual savings** and a **certified 0.018% optimality gap**.
- **BCG ASPIRE (2026)** — Selected for BCG's international program for high-potential women.
- **Mensa Argentina (2026)** — Admitted after passing a supervised, in-person qualifying examination.
- **Santander Argentina Merit Award (2025)** — Recognized among 200 students with the country's highest university GPAs.
- **SCIAA Speaker (2024 & 2025)** — Twice selected to present projects at the Scientific Symposium on Artificial Intelligence and Applications.
- **ICPC Latin American Regional (2024 & 2025)** — Qualified twice through the Argentine Programming Contest.
- **National Parliamentary Debate (2022)** — National champion and best speaker.

---

## Technical toolkit

**Languages:** Python · C · Java · SQL · LaTeX  
**ML & scientific computing:** PyTorch · scikit-learn · XGBoost · NumPy · Pandas · SciPy  
**Optimization & computer vision:** OR-Tools CP-SAT · MILP · simulated annealing · YOLO · OpenCV  
**Data & deployment:** Dagster · dbt · MLflow · Airflow · FastAPI · Docker · PySpark · CI/CD · PostgreSQL · MongoDB · Neo4j

**Languages spoken:** Spanish (native) · English (professional)

---

Interested in collaborating on **applied ML, optimization, or research at the intersection of learning and dynamical systems**? [Get in touch](mailto:micolmichanie@gmail.com).
