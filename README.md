# Hi, I'm Diego Alves 👋

**Data Engineer, Data Scientist & AI Engineer** building end-to-end data platforms, machine learning systems and LLM applications, from raw ingestion to deployed, tested and evaluated products.

📍 São Paulo state, Brazil · 🗣️ Portuguese (native), English (C2), Spanish (C1)

[![Portfolio](https://img.shields.io/badge/Portfolio-diegoalves.vercel.app-13233a?style=for-the-badge&logo=googlechrome&logoColor=white)](https://diegoalves.vercel.app/)

*Case studies and measured results for every project, in English and Portuguese.*

---

## 🧠 AI Engineering

| Project | What it does | Stack | CI |
|---|---|---|---|
| [**LLM from Scratch**](https://github.com/DiegoTDDD/llm-from-scratch) | GPT-style model written from scratch (byte-level BPE, causal attention, KV cache) and trained on 13M characters of 10-K filings on a free CPU runner: validation perplexity 32 vs 837 for a unigram baseline, KV cache up to 5.8× faster | PyTorch, GitHub Actions | [![ci](https://github.com/DiegoTDDD/llm-from-scratch/actions/workflows/tests.yml/badge.svg)](https://github.com/DiegoTDDD/llm-from-scratch/actions/workflows/tests.yml) |
| [**SEC Filings RAG**](https://github.com/DiegoTDDD/sec-filings-rag) | Question answering over 10-K/10-Q filings with cited sources, hybrid retrieval, re-ranking and RAGAS evaluation · [Demo](https://sec-filings-rag-demo.streamlit.app) | Qdrant, Ollama, sentence-transformers, FastAPI | [![ci](https://github.com/DiegoTDDD/sec-filings-rag/actions/workflows/tests.yml/badge.svg)](https://github.com/DiegoTDDD/sec-filings-rag/actions/workflows/tests.yml) |
| [**SEC MCP Agent**](https://github.com/DiegoTDDD/sec-mcp-agent) | MCP servers over SEC 10-K filings and the fraud model, and a local tool-calling agent whose citations are verified against the retrieved passages: 17 of 22 eval questions, up from 7 over six measured runs; works in Claude Desktop | MCP SDK, Pydantic, Ollama, XGBoost | [![ci](https://github.com/DiegoTDDD/sec-mcp-agent/actions/workflows/tests.yml/badge.svg)](https://github.com/DiegoTDDD/sec-mcp-agent/actions/workflows/tests.yml) |
| [**Olist AI Analyst**](https://github.com/DiegoTDDD/olist-ai-analyst) | A local-model analyst that turns a business question about the real Olist data into a decision memo; code checks the SQL (read-only, parser-validated), reads the trend and requires every number in the memo to be in the result: 68% execution accuracy on 25 questions in the last of three measured runs, 92% of memos fully grounded, the rest marked unverified | DuckDB, Ollama, Qwen2.5-Coder | [![ci](https://github.com/DiegoTDDD/olist-ai-analyst/actions/workflows/tests.yml/badge.svg)](https://github.com/DiegoTDDD/olist-ai-analyst/actions/workflows/tests.yml) |
| [**Fraud Investigation Agents**](https://github.com/DiegoTDDD/fraud-investigation-agents) | LangGraph team (planner, researcher, reporter, rule-based critic) that investigates fraud alerts through MCP tools; on 30 known cases the critic loop lifts pattern accuracy from 47% (single LLM call) to 77% | LangGraph, MCP, Ollama | [![ci](https://github.com/DiegoTDDD/fraud-investigation-agents/actions/workflows/tests.yml/badge.svg)](https://github.com/DiegoTDDD/fraud-investigation-agents/actions/workflows/tests.yml) |
| [**LLM Evals & Observability**](https://github.com/DiegoTDDD/llm-evals-observability) | Regression gate on every pull request (replays 162 real model tool calls; [blocked a regression](https://github.com/DiegoTDDD/llm-evals-observability/pull/1)), weekly live evals traced with OpenTelemetry into self-hosted Langfuse, and a [public dashboard](https://diegotddd.github.io/llm-evals-observability/) | OpenTelemetry, Langfuse, GitHub Actions | [![ci](https://github.com/DiegoTDDD/llm-evals-observability/actions/workflows/gate.yml/badge.svg)](https://github.com/DiegoTDDD/llm-evals-observability/actions/workflows/gate.yml) |
| [**LLM Guardrails & Red Team**](https://github.com/DiegoTDDD/llm-guardrails-redteam) | Six guardrail layers wrapped around both agents (injection quarantine, PII redaction, tool policy, output, critic, log redaction); a red-team suite runs in CI: 23 attacks that all work unguarded are all blocked, with 0 false positives on 283 real texts | MCP, LangGraph, OpenTelemetry, pytest | [![ci](https://github.com/DiegoTDDD/llm-guardrails-redteam/actions/workflows/redteam.yml/badge.svg)](https://github.com/DiegoTDDD/llm-guardrails-redteam/actions/workflows/redteam.yml) |
| [**Fine-Tune & Serve**](https://github.com/DiegoTDDD/finetune-and-serve) | LoRA fine-tune of a 0.5B model on a free CPU runner to tag XBRL facts in 10-K sentences: 0.82 F1 on auditor labels against 0.65 for a 3B model with examples, 3.7× the throughput, served with llama.cpp and costed against API list prices | PEFT, llama.cpp | [![ci](https://github.com/DiegoTDDD/finetune-and-serve/actions/workflows/ci.yml/badge.svg)](https://github.com/DiegoTDDD/finetune-and-serve/actions/workflows/ci.yml) |

## 🏗️ Data Engineering & Machine Learning

| Project | What it does | Stack | Live |
|---|---|---|---|
| [**LogiNexus — Freight Intelligence**](https://github.com/DiegoTDDD/freight-intelligence) | Freight analytics and forecasting platform: 97.6M-row medallion pipeline, forecasting evaluated on held-out years, truck-aware routing and a public API | Python, Polars, DuckDB, FastAPI, Docker | [Demo](https://loginexus-dashboard-preview.onrender.com/) |
| [**Real-Time Fraud Detection ML**](https://github.com/DiegoTDDD/realtime-fraud-detection-ml) | XGBoost model scoring a live Kafka stream in real time, with a precision/recall dashboard (PR-AUC 0.9925) | XGBoost, Spark Structured Streaming, Kafka | [Demo](https://realtime-fraud-detection-ml.streamlit.app) |
| [**Real-Time Fraud Streaming**](https://github.com/DiegoTDDD/realtime-fraud-streaming) | Streaming backbone with event-time windows and watermarking over ~10 transactions/second | Redpanda, Spark Structured Streaming | [Demo](https://realtime-fraud-streaming.streamlit.app) |
| [**Supply Chain Risk Intelligence**](https://github.com/DiegoTDDD/supply-chain-risk-intelligence) | Delivery-delay analysis from cause to decision: causal inference, survival analysis, forecasting, SHAP and optimization | statsmodels, lifelines, XGBoost, PuLP | [Demo](https://diego-supply-chain-risk.streamlit.app) |
| [**NYC Tip MLOps**](https://github.com/DiegoTDDD/nyc-tip-mlops) | End-to-end MLOps: training, model registry, API serving and drift monitoring | MLflow, FastAPI, Evidently, Docker | [Demo](https://nyc-tip-mlops.streamlit.app) |
| [**NYC Taxi Lakehouse**](https://github.com/DiegoTDDD/nyc-taxi-lakehouse) | Medallion lakehouse over 22M+ taxi trips with schema evolution and data quality checks | Delta Lake, DuckDB, Dagster | [Demo](https://nyc-taxi-lakehouse.streamlit.app) |
| [**Olist Cloud Warehouse**](https://github.com/DiegoTDDD/olist-cloud-warehouse) | BigQuery warehouse in São Paulo: Terraform, keyless CI through Workload Identity Federation, dbt with enforced contracts; partitioning cuts a one-month query by 92% | BigQuery, Terraform, dbt | [Project page](https://diegotddd.github.io/olist-cloud-warehouse/) |
| [**Olist Analytics**](https://github.com/DiegoTDDD/olist-analytics) | Dimensional model, dbt tests and dashboard on Brazilian e-commerce data | dbt, DuckDB | [Demo](https://diegotddd-olist-analytics.streamlit.app) |
| [**Economic Data Platform**](https://github.com/DiegoTDDD/Economic-data-platform) | Containerized ELT pipeline for Brazilian macroeconomic and crypto market data, with quality checks and atomic Gold refresh | PostgreSQL, Docker, GitHub Actions | [Demo](https://diegotddd-economic-data-platform.streamlit.app) |

---

## ⚙️ How I build

Every project ships with automated tests and CI, documented architecture decisions, reproducible environments (Docker), dependency security audits and results measured on real data.

---

## 🛠️ Tech stack

**Languages & data** ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-336791?style=flat-square&logo=postgresql&logoColor=white) ![PySpark](https://img.shields.io/badge/PySpark-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Polars](https://img.shields.io/badge/Polars-CD792C?style=flat-square&logo=polars&logoColor=white) ![DuckDB](https://img.shields.io/badge/DuckDB-FFF000?style=flat-square&logo=duckdb&logoColor=black) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![dbt](https://img.shields.io/badge/dbt-FF694B?style=flat-square&logo=dbt&logoColor=white)

**Data engineering** ![Spark Streaming](https://img.shields.io/badge/Spark_Streaming-E25A1C?style=flat-square&logo=apachespark&logoColor=white) ![Kafka / Redpanda](https://img.shields.io/badge/Kafka_%2F_Redpanda-231F20?style=flat-square&logo=apachekafka&logoColor=white) ![Delta Lake](https://img.shields.io/badge/Delta_Lake-00ADD4?style=flat-square) ![Dagster](https://img.shields.io/badge/Dagster-4F43DD?style=flat-square)

**Cloud & infrastructure** ![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=googlecloud&logoColor=white) ![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white) ![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=flat-square&logo=terraform&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)

**Machine learning** ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white) ![XGBoost](https://img.shields.io/badge/XGBoost-189AB4?style=flat-square) ![SHAP](https://img.shields.io/badge/SHAP-FF0D57?style=flat-square) ![MLflow](https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white) ![Evidently](https://img.shields.io/badge/Evidently-ED0400?style=flat-square) ![statsmodels](https://img.shields.io/badge/statsmodels-4051B5?style=flat-square)

**LLMs & agents** ![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white) ![Transformers](https://img.shields.io/badge/Transformers-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![LoRA (PEFT)](https://img.shields.io/badge/LoRA_(PEFT)-FF9D00?style=flat-square) ![llama.cpp](https://img.shields.io/badge/llama.cpp-000000?style=flat-square) ![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat-square&logo=ollama&logoColor=white) ![MCP](https://img.shields.io/badge/MCP-D97757?style=flat-square) ![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![Qdrant](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square) ![RAGAS](https://img.shields.io/badge/RAGAS-6A5ACD?style=flat-square) ![Langfuse](https://img.shields.io/badge/Langfuse-0A0A0A?style=flat-square) ![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white)

**Product & BI** ![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white) ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat-square&logo=powerbi&logoColor=black) ![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square)

---

## 🎓 Education

- Postgraduate in Data Science & Big Data Analytics — Faculdade IMES (2026)
- BSc in Information Technology — UNIVESP (expected 2026)
- AI Technician — IFNMG (expected 2027)
- Technologist in Business Management — Fatec Catanduva (2023)

📚 Five books written: the [Data-Driven Decisions trilogy](https://diegoalves.vercel.app/en/books.html) in English (SQL, Power BI and Python for decisions), plus a business book and a 1,042-page data science guide in Portuguese.
