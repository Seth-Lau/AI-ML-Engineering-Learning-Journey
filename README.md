# AI / ML Engineering — Learning Journey

Mechanical engineer (BEng, University of Warwick) transitioning into applied ML engineering. Currently at a London food manufacturer, splitting my time between new product development and building an internal sales platform as its sole developer, while working toward junior Applied ML Engineer / Data Scientist roles.

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

### B2B sales platform *(active, in production)*

Internal sales platform used daily by a commercial team. I inherited it from a previous developer in 2026 and now own its development, reliability and AI features. *Closed source; details kept deliberately general to respect confidentiality.*

**AI work**
- **LLM tool-calling assistant:** connected an existing voice-input LLM feature to structured business data through tool calls (search → lookup), so answers come from validated source data rather than the model's memory. Validated against known-correct answers before release.
- **Data controls for AI features:** admin-only data updates with staging, diff review and rollback; sensitive commercial fields excluded from the application database.

**Engineering**
- Ran a structured technical handover covering code, access, data and deployment
- Moved the production database onto company-owned infrastructure and added automated daily backups, resolving a recurring availability issue
- Built a scheduled data sync with defensive safeguards: no writes after a failed read, protection against unexpected data shrinkage, conflict reporting
- Redesigned a management dashboard: restructured the layout, corrected query-level ranking errors, reduced queries per page load
- Automated test suite and an isolated test environment containing no production data
- AI-assisted development with guardrails: manual approval of agent actions, production credentials isolated from the coding agent

**Skills used:** TypeScript · SQL · LLM tool calling · scheduled data pipelines · CI/CD · automated testing

**Next**
- [ ] Evaluation harness for the LLM assistant: known-answer test set, accuracy tracked per commit, regression gate in CI
- [ ] Similarity-based lead ranking using engineered features, replacing broad rule-based filtering

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

- [ ] **Duke — MLOps Tools: MLflow and Hugging Face** *(~3 weeks)* — experiment tracking and model registry, run against real forecasting experiments rather than course datasets

---

## Tools
Python, SQL, TypeScript, Git and scikit-learn.

---

## Background

New product developer, responsible for the full NPD cycle from concept through to approved production spec. Approved product development for major UK retailers and restaurant groups; menu creation for a high end independent London restaurant.

The relevance to ML work is direct: demand forecasting, yield and waste reduction, and process optimisation are problems I have worked on from the operations side before approaching them as modelling problems.

