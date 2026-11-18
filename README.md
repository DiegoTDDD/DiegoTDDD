# Hi, I'm Diego Alves 👋

**Data Engineer, Data Scientist & AI Engineer** building end-to-end data platforms, machine learning systems and LLM applications, from raw ingestion to deployed, tested and evaluated products.

📍 São Paulo state, Brazil · 🗣️ Portuguese (native), English (C2), Spanish (C1)

---

## 🧠 AI Engineering

| Project | What it does | Stack |
|---|---|---|
| [**LLM from Scratch**](https://github.com/DiegoTDDD/llm-from-scratch) | BPE tokenizer, causal attention, GPT-style decoder and KV-cache implemented in PyTorch and trained on SEC filings text | PyTorch |
| [**SEC Filings RAG**](https://github.com/DiegoTDDD/sec-filings-rag) | Question answering over 10-K/10-Q filings with cited sources, hybrid retrieval, re-ranking and RAGAS evaluation · [Demo](https://sec-filings-rag-demo.streamlit.app) | Qdrant, Ollama, sentence-transformers, FastAPI |
| [**SEC MCP Agent**](https://github.com/DiegoTDDD/sec-mcp-agent) | Tool-calling agent with custom MCP servers exposing the SEC RAG and the fraud model, with structured outputs | MCP, Pydantic, FastAPI |
| [**Fraud Investigation Agents**](https://github.com/DiegoTDDD/fraud-investigation-agents) | Multi-agent system (planner, researcher, critic, reporter) that investigates suspicious transactions end to end | LangGraph, MCP |
| [**LLM Evals & Observability**](https://github.com/DiegoTDDD/llm-evals-observability) | Evaluation harness with regression gates in CI, plus tracing, latency and cost monitoring | RAGAS, OpenTelemetry, Langfuse |
| [**LLM Guardrails & Red Team**](https://github.com/DiegoTDDD/llm-guardrails-redteam) | Threat model, input/output guardrails, PII redaction and an automated red-team suite running in CI | Presidio, pytest |
| [**Fine-Tune & Serve**](https://github.com/DiegoTDDD/finetune-and-serve) | QLoRA fine-tuning for structured extraction and self-hosted inference benchmarked against a hosted API | PEFT, vLLM |

## 🏗️ Data Engineering & Machine Learning

| Project | What it does | Stack | Live |
|---|---|---|---|
| [**LogiNexus — Freight Intelligence**](https://github.com/DiegoTDDD/freight-intelligence) | Freight analytics and forecasting platform: 97.6M-row medallion pipeline, forecasting evaluated on held-out years, truck-aware routing and a public API | Python, Polars, DuckDB, FastAPI, Docker | [Demo](https://loginexus-dashboard-preview.onrender.com/) |
| [**Real-Time Fraud Detection ML**](https://github.com/DiegoTDDD/realtime-fraud-detection-ml) | XGBoost model scoring a live Kafka stream in real time, with a precision/recall dashboard (PR-AUC 0.9925) | XGBoost, Spark Structured Streaming, Kafka | [Demo](https://realtime-fraud-detection-ml.streamlit.app) |
| [**Real-Time Fraud Streaming**](https://github.com/DiegoTDDD/realtime-fraud-streaming) | Streaming backbone with event-time windows and watermarking over ~10 transactions/second | Redpanda, Spark Structured Streaming | [Demo](https://realtime-fraud-streaming.streamlit.app) |
| [**Supply Chain Risk Intelligence**](https://github.com/DiegoTDDD/supply-chain-risk-intelligence) | Delivery-delay analysis from cause to decision: causal inference, survival analysis, forecasting, SHAP and optimization | statsmodels, lifelines, XGBoost, PuLP | [Demo](https://diego-supply-chain-risk.streamlit.app) |
| [**NYC Tip MLOps**](https://github.com/DiegoTDDD/nyc-tip-mlops) | End-to-end MLOps: training, model registry, API serving and drift monitoring | MLflow, FastAPI, Evidently, Docker | [Demo](https://nyc-tip-mlops.streamlit.app) |
| [**NYC Taxi Lakehouse**](https://github.com/DiegoTDDD/nyc-taxi-lakehouse) | Medallion lakehouse over 22M+ taxi trips with schema evolution and data quality checks | Delta Lake, DuckDB, Dagster | [Demo](https://nyc-taxi-lakehouse.streamlit.app) |
| [**Olist Analytics**](https://github.com/DiegoTDDD/olist-analytics) | Dimensional model, dbt tests and dashboard on Brazilian e-commerce data | dbt, DuckDB | [Demo](https://diegotddd-olist-analytics.streamlit.app) |
| [**Economic Data Platform**](https://github.com/DiegoTDDD/Economic-data-platform) | Containerized ELT pipeline for Brazilian macroeconomic and crypto market data, with quality checks and atomic Gold refresh | PostgreSQL, Docker, GitHub Actions | [Demo](https://diegotddd-economic-data-platform.streamlit.app) |

---

## ⚙️ How I build

Every project ships with automated tests and CI, documented architecture decisions, reproducible environments (Docker), dependency security audits and results measured on real data.

---

## 🛠️ Tech stack

- **Languages:** Python, SQL
- **Data engineering:** Spark, Kafka / Redpanda, Delta Lake, DuckDB, Polars, dbt, Dagster, PostgreSQL
- **Machine learning:** scikit-learn, XGBoost, MLflow, Evidently, SHAP, causal inference, survival analysis, time series
- **Deep learning & LLMs:** PyTorch, Transformers, RAG, MCP, LangGraph, QLoRA, vLLM, Qdrant, Ollama, RAGAS, Langfuse
- **Engineering:** Docker, FastAPI, GitHub Actions, pytest, OpenTelemetry
- **BI:** Power BI (DAX), Tableau, Streamlit

---

## 🎓 Education

- Postgraduate in Data Science & Big Data Analytics — Faculdade IMES (2026)
- BSc in Information Technology — UNIVESP (expected 2026)
- AI Technician — IFNMG (expected 2027)
- Technologist in Business Management — Fatec Catanduva (2023)

📚 Author of five published books (technical, business and literary).
