# AI / ML Engineering — Learning Journey

Mechanical engineer (BEng, University of Warwick) transitioning into applied ML engineering. Currently at a London fresh pasta manufacturer, splitting my time between new product development and building an internal sales platform as its sole developer, while working toward junior Applied ML Engineer / Data Scientist roles.

**Working principles:** portfolio over certificates · from-scratch before frameworks · ship real things

---

## Current focus
| | |
|---|---|
| **Active project** | Internal B2B sales prospecting platform |
| **Active course** | DeepLearning.AI — Machine Learning in Production |
| **Next milestone** | MLOps course sequence completion |

---

## Projects

### B2B prospecting platform *(active)*

Internal web application for discovering, qualifying and contacting trade customers in the food service sector. Originally built by a previous developer; I took over the codebase and now own its development.

**Stack**

| Layer | Technology |
|---|---|
| Frontend | Next.js 14 (App Router), TypeScript, Tailwind |
| Mapping | Leaflet + OpenStreetMap — clustered geospatial search across ~135k UK venues |
| Data source | Public food-safety venue dataset, refreshed daily via a scheduled GitHub Actions pipeline into object storage |
| LLM layer | Anthropic Claude — filtering, record entry, email drafting, opportunity detection |
| Database | PostgreSQL |
| Integration | Business intelligence platform for live customer and sales data |
| Auth | Role-based access control |

**What I'm working on**

- [ ] **Look-alike lead ranking** — ranking the venue dataset by similarity to existing customer accounts across engineered features (venue type, hygiene rating, local density of comparable venues, proximity to existing accounts), replacing broad criteria filtering that currently returns high volume at low precision
- [ ] **Geospatial lead discovery** — clustered map visualisation across a national venue dataset
- [ ] **Evaluation harness** — question/known-answer pairs tracked over time, so changes to prompts and schema produce a measurable accuracy delta rather than a guess

**Engineering and reliability**

- [ ] Codebase read-through and documentation following handover
- [ ] Test coverage and CI
- [ ] Pipeline observability — refresh failure alerting and upstream schema drift detection
- [ ] Production audit: failure modes, monitoring gaps, drift exposure

*Closed source — internal company project*

### Time series forecasting *(active)*

Demand forecasting project applying the time series techniques below to real operational data.

---

## Learning roadmap

### Completed

- [x] IBM — Python for Data Science
- [x] Mathematics for Machine Learning
- [x] SQL for Data Science with Python *(Modules 1–5)*
- [x] DeepLearning.AI / Stanford — Machine Learning Specialization *(all three courses)*
- [x] Kaggle — Time Series micro-course
- [x] Course 1 study reference notebook — from-scratch NumPy implementations alongside scikit-learn equivalents, worked on manufacturing and predictive maintenance data

### In progress

- [ ] **DeepLearning.AI — Machine Learning in Production** *(~2 weeks)*
  ML project lifecycle, deployment and monitoring patterns, concept drift, error analysis, data definition and baselines. Taken standalone; the remaining TFX-heavy courses in the specialization are deliberately skipped.

### Next — MLOps sequence

- [ ] **Duke — Python Essentials for MLOps** *(~3 weeks)* — packaging, testing, CLI tooling, project structure
- [ ] **Duke — DevOps, DataOps, MLOps** *(~4 weeks)* — CI/CD, reproducibility, observability
- [ ] **Duke — MLOps Tools: MLflow and Hugging Face** *(~3 weeks)* — experiment tracking and model registry, run against real forecasting experiments rather than course datasets
- [ ] **Duke — MLOps Platforms: SageMaker and Azure ML** *(~4 weeks)* — cloud deployment, SageMaker prioritised

### Later

- [ ] PyTorch
- [ ] Hugging Face ecosystem
- [ ] LoRA / QLoRA fine-tuning
- [ ] fast.ai — Practical Deep Learning for Coders
- [ ] Karpathy — Neural Networks: Zero to Hero
- [ ] AWS certification path: AI Practitioner → ML Engineer Associate → Generative AI Developer Professional

---

## Tools

**Development** VS Code · Claude Code · Jupyter
**Version control** Git · GitHub · GitHub Actions
**Python** pandas · NumPy · scikit-learn · sqlite3
**Web** TypeScript · Next.js · Tailwind · Leaflet
**Data** SQL · PostgreSQL · SQLite

---

## Background

New product developer, responsible for the full NPD cycle from concept through to approved production spec. Approved product development for a major UK retailer and for restaurant groups including Gordon Ramsay Restaurants and the Marco Pierre White group; menu design for a high end independent London restaurant.

The relevance to ML work is direct: demand forecasting, yield and waste reduction, and process optimisation are problems I have worked on from the operations side before approaching them as modelling problems.

