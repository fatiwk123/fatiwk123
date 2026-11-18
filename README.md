# Hi, I'm Fatima Ezzahra Wankida 👋

**Junior Data Engineer** · ENSEM Nancy engineering degree (Digital Systems, MSc-equivalent, 2026) · based in Paris  
I build data pipelines that are **incremental, tested and traceable**, and the RAG/LLM applications that sit on top of them.

🎯 **Open to full-time Data Engineer / Data & AI Engineer roles (CDI)** — [LinkedIn](https://www.linkedin.com/in/fatima-ezzahra-wankida)

---

## 🔧 Featured project

### [nhtsa-lakehouse-rag](https://github.com/fatiwk123/nhtsa-lakehouse-rag) — end-to-end incremental lakehouse + RAG assistant
Answers text and numeric questions about vehicle recalls and complaints (NHTSA public API + technical PDFs).

- **Lakehouse**: MinIO + Apache Iceberg, bronze → silver → gold, hash-based incremental ingestion (a re-run adds 0 rows)
- **Transformations & quality**: dbt-duckdb, dbt tests + Soda checks that **block publication** when quality fails
- **Orchestration**: Dagster assets, daily schedule, failure sensor with alerting
- **RAG**: pgvector + tsvector (BM25) hybrid retrieval with RRF, cross-encoder reranking, cited answers, "I don't know" threshold
- **Agent**: document search + read-only SQL tool over gold tables, served with FastAPI + Streamlit
- **CI**: GitHub Actions runs the full pipeline end-to-end on a small scope

`Python` `SQL` `dbt` `DuckDB` `Iceberg` `MinIO` `Dagster` `Soda` `PostgreSQL` `pgvector` `FastAPI` `Docker`

---

## 💼 Experience

**Data Engineer Intern — NgC GmbH, Diag2Go** (Wolfsburg, 04–10/2026) · *AI automotive diagnostics platform (RAG)*  
- Extended the knowledge base to multiple OEMs: **2,700 manuals from 24 manufacturers** collected and integrated
- Structured and loaded **2,047 OEM fault codes (DTC)** with validation and traceability
- Benchmarked multilingual embedding models: local model **18× faster** than a paid API at equivalent recall
- Audited the database (2 silent defects found), built a confidence guardrail (ROC) and a repair-cost estimator

**Data Engineer Intern — LORIA lab / ENSEM, HY2CAR project** (Nancy, 06–09/2025) · *hydrogen hybrid vehicle data platform*  
- Ingested and decoded real vehicle measurements (speed, current, voltage, SOC)
- Designed a bronze/silver/gold pipeline (**Parquet, DuckDB, dbt**): unit harmonisation, resampling, trip splitting, energy KPIs
- Automated data quality checks (physical ranges, gaps, timestamps) and defined the simulation's data contract

*(Company / lab code is private.)*

---

## 📂 Other projects

- **vehicle-telemetry-pipeline** *(in progress)* — streaming OBD-II telemetry: Kafka → Parquet data lake → BigQuery → dbt → Airflow → Streamlit
- **Hydrogen hybrid vehicle simulator (R&D, ENSEM)** — CARLA / FMU co-simulation, 5 Hz telemetry logging, eco-driving scoring engine
- **[twizzy](https://github.com/fatiwk123/twizzy)** — computer vision (OpenCV) traffic-sign detection and recognition, team project

---

## 🧰 Tech stack

**Data engineering**: Python, SQL, dbt, DuckDB, Parquet, Apache Iceberg, Dagster, Airflow, Kafka, Soda, ETL/ELT, web scraping  
**Databases & cloud**: PostgreSQL, pgvector, BigQuery, GCP, Docker, Terraform, GitHub Actions  
**AI**: RAG, embeddings, hybrid search & reranking, LLMs (Mistral), multilingual NLP, PyTorch

🗣️ French (fluent) · English (C1) · German (A2, learning)
