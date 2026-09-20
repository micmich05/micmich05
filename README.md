# Micol Michanie

AI Engineering @ Universidad de San Andrés · AI Lead @ Rappi 

Buenos Aires, Argentina · [micolmichanie@gmail.com](mailto:micolmichanie@gmail.com) · [LinkedIn](https://www.linkedin.com/in/micol-michanie-2556bb23a/)

I lead a team of six inside Rappi's Payments vertical. We build ML models, agent pipelines and process automation for payins, refunds, reconciliation and treasury across 9 countries in Latin America. I own the technical roadmap, run execution alongside Product and Operations, and handle hiring and mentoring for the team.

Before Rappi I built AI systems for the Municipality of San Nicolás and data automation at MSD. I'm finishing a B.Eng. in AI Engineering and I TA Algorithms & Data Structures.

## Projects

### Redesigning a 204 box packaging catalog with a provably optimal solver
`OR-Tools CP-SAT` `MILP` `combinatorial optimization` `Python` · 2026
**[github.com/micmich05/bonsai-packaging-optimization](https://github.com/micmich05/bonsai-packaging-optimization)**

Bonsai Corp ships 427 products across 5 plants in 204 box types. The task, set by the AlixPartners Data Challenge, was to redesign that catalog to minimize annual packaging and freight cost under containment, dimensional fit, headspace, compression resistance and pallet stacking constraints.

Cost depends on box dimensions only through integer counts of boxes per pallet, so the continuous design space collapses. Enumerating exterior dimensions at the pallet thresholds and at each product's fit bounds yields 4,558 candidate boxes and 145,469 admissible pairings of product and box, with no loss of optimality. On that space a MILP with linearized volume discount tiers solves in exact integer arithmetic with CP-SAT, which returns the assignment and the lower bound that certifies it.

The proposed catalog of 55 box types on 14 base footprints costs USD 188.1M against USD 209.2M today, an annual saving of USD 21.2M or 10.1%. A proven lower bound of USD 188.05M puts the remaining gap at 0.018%. Pallet occupancy rises from 82.2% to 93.8%, shipped pallets drop by 119k per year, and inventory positions fall from 430 to 158.

The repo ships the frozen solution, a validator that checks every assignment row against the full rule set, 35 tests, a CLI that prices new product launches against the catalog, and a 25 page business report. Verifying the result does not require reoptimizing.

### Retiming a city corridor's traffic lights from real camera footage
`SUMO` `simulated annealing` `YOLOv8` `OpenCV` · Dec 2024 to Sep 2025

I processed footage of Av. Savio in San Nicolás de los Arroyos with YOLOv8 to extract vehicle counts and turn ratios, rebuilt the corridor in SUMO, and ran simulated annealing over the phase and offset space. The fitness function combines flow, queue length and stops, and is evaluated over separate time windows so the solution holds at rush hour and off peak rather than optimizing for an average that never occurs.

The resulting configuration raised average speed by 22% and cut stops by 35% in simulation. The municipality adopted it, and it was covered by Diario El Norte and Ramallo Informa. Presented at SCIAA 2025.

### Counting animals in drone footage with RGB and thermal fusion
`YOLOv8` `YOLOv11` `PyTorch` · Oct 2025 to Dec 2025

Detection and counting of wildlife from drone imagery, aimed at the cases where a single sensor fails: low light, camouflage, partial occlusion by canopy. I fused RGB and thermal streams into a YOLOv8 detector so the model has a signal to fall back on when either channel degrades.

The original dataset had systematic missing annotations, which inflates false positive counts and makes evaluation meaningless. I relabeled it with YOLOv11 assistance and manual review before measuring anything.

### Predicting used SUV prices from 18k messy marketplace listings
`XGBoost` `scikit-learn` `RapidFuzz` `Pandas` · May 2025 to Jul 2025

End to end regression pipeline over real Mercado Libre listings. Most of the work sat upstream of the model: regex extraction of specs from titles and descriptions written in free text, fuzzy token matching with RapidFuzz to collapse the long tail of inconsistent model names into canonical ones, currency normalization across ARS and USD listings, and one-hot encoding of categoricals.

I trained Ridge, Lasso, Random Forest and XGBoost, tuned with randomized search and 5-fold cross validation. The best model reached R² 0.94 on test data it had never seen.

### Searching deeper in Gomoku under a fixed time budget
`minimax` `alpha-beta pruning` `MCTS` `Python` · Jul 2024 to Nov 2024

Game playing agent built on minimax, with the search optimizations that actually move the needle when the clock is the binding constraint: alpha-beta pruning, move ordering, late move reduction, and quiescence search to avoid horizon effects on forced sequences. I also implemented and benchmarked a Monte Carlo tree search agent to compare how each approach degrades as the time limit tightens. Presented at SCIAA 2024.

## Experience

### AI Lead, Rappi · since Oct 2025
- Lead a team of six designing and shipping AI and automation for the Payments vertical across 9 countries, tying technical objectives to operational efficiency and decision making.
- Define the technical roadmap, prioritize initiatives, and own execution of data and ML projects from scoping through deployment, working across Product, Operations and Analytics.
- Run hiring for the team: design the technical assessments, interview candidates, and mentor engineers toward autonomy and good practice.

### AI Engineer & Consultant, Secretaría de Innovación, Municipality of San Nicolás · since Dec 2024
- Audited municipal operations to find where AI was actually the right tool, and scoped the projects that were.
- Built ML models that cut manual data labeling time by over 90%.
- Consulted on optimization problems using reinforcement learning and search methods, reducing citizen wait times by over 40%.

### Business Data Analyst, MSD (Merck Sharp & Dohme) · Jan 2025 to Sep 2025
- Automated data validation pipelines in Pandas, raising operational efficiency by 50%.
- Built a fuzzy database matching solution in Python with RapidFuzz, replacing manual reconciliation and raising efficiency on those tasks by 75%.

## Education

**B.Eng. in Artificial Intelligence Engineering** · Universidad de San Andrés · since Mar 2023 · GPA 9.66/10

Teaching assistant for Algorithms & Data Structures and Systems Dynamics at the School of Engineering: material preparation, exercise sessions and student tutoring.

Coursework includes LLMs and Transformers, Deep Learning and Neural Networks, VAEs, Computational Algebra, Graph Theory, applied statistics, clustering and tree based models.

## Recognition

**Special Recognition, AlixPartners Data Challenge** (2026)
First participant in the challenge to reach the optimal solution. The resulting catalog represented an estimated USD 21.2M in annual savings, a 10.1% reduction. Code and report above.

**BCG ASPIRE** (2026)
Selected for Boston Consulting Group's international program for high potential women, admitted through a multi stage selection process.

**Mensa Argentina** (2026)
Admitted after the supervised in person admission exam, the threshold being the top 2% of the population by standardized IQ.

**Banco Santander Argentina Merit Award** (2025)
Granted to the 200 highest university GPAs nationwide, across all institutions and fields of study.

**ICPC Latin American Regional Contest** (2024, 2025)
Qualified twice for the regional finals of the International Collegiate Programming Contest, based on team performance in the Argentine Programming Contest. Competitive programming is where I learned to reason about complexity under a clock, which is the habit I lean on most in production work.

**SCIAA Speaker** (2024, 2025)
Accepted twice to present research at the Scientific Symposium on Artificial Intelligence and Applications: the Gomoku search agent in 2024, the traffic signal optimizer in 2025.

**National Champion & Best Speaker, Parliamentary Debate** (2022)
Both titles in the same season in the national competitive league, certified by the Argentine Debate Association.

**ITBA Recognition** (2022)
For an academic essay on AI, Big Data and environmental sustainability, written and presented at the Buenos Aires Institute of Technology.

**ACOBI National Mathematics Champion** (2016, 2017)
First place nationally in consecutive editions.

## Stack

**Languages** Python · C · Java · SQL · LaTeX

**ML** PyTorch · scikit-learn · XGBoost · Pandas · NumPy · SciPy

**Optimization** OR-Tools CP-SAT · MILP · local search · reinforcement learning

**Computer vision** Ultralytics YOLOv8 · YOLOv11 · OpenCV

**Data & infra** PySpark · Airflow · FastAPI · Docker · n8n · CI/CD · MLOps

**Databases** MongoDB · Neo4j

Spanish (native) · English (professional)
