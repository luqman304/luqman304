# Luqman Abdulwahab

**AI master's student in Paris, building LLM and machine-learning systems that are measured, not just demoed.**

I work on retrieval-augmented generation, LLM evaluation and production ML services: Python back ends, vector
search, model APIs and the test harnesses that show whether a change actually helped.
Open to **AI / ML engineering internships**.

[LinkedIn](https://www.linkedin.com/in/luqman-abdulwahab-7b421b217) · [Email](mailto:luqmanabdulwahab108@gmail.com)

---

### Featured projects

| project | what it is | stack |
|---|---|---|
| [**ap-copilot**](https://github.com/luqman304/ap-copilot) | Accounts-payable agent for Dynamics 365 Business Central: reads supplier invoices, runs a 3-way match against POs and goods receipts, flags duplicates, overcharges and bank-detail changes, and drafts the invoice for human approval in Teams. Draft-only by design — posting is blocked in code, in BC permissions and in the AL extension. Hash-chained audit log, ADRs for every decision. | Python · FastAPI · Claude API · Business Central (AL) · Power Automate |
| [**eu-ai-act-rag**](https://github.com/luqman304/eu-ai-act-rag) | Cited Q&A over the EU AI Act with an evaluation harness. Structure-aware chunking and hybrid search raised recall@5 from 69.6 to 89.9 and answer correctness from 0.68 to 0.85, with bootstrap confidence intervals. | FastAPI · Qdrant · Claude API · Docker · CI |
| [**velib-forecasting**](https://github.com/luqman304/velib-forecasting) | Forecasts Paris Vélib' bike availability 30 minutes to 24 hours ahead from 11 M messy open-data snapshots, cleaned with 10 documented rules. Walk-forward validation over 8 weekly folds and 864 k scored points: MAE 2.26 bikes against 2.89 for persistence and 4.39 for seasonal naive, with block-bootstrap CIs. Streamlit map app. | LightGBM · pandas · Streamlit · GitHub Actions |
| [**gnn-fraud-detection**](https://github.com/luqman304/gnn-fraud-detection) | Illicit-Bitcoin detection on the Elliptic dataset (204 k transactions), with a temporal split that never lets a model see the future. Benchmarks GCN and GraphSAGE against feature baselines over 5 seeds: the random forest wins at F1 0.815, and the honest negative result is written up rather than hidden. Scoring API explains a prediction through the transaction's neighbourhood. | PyTorch Geometric · scikit-learn · FastAPI |
| [**lora-finetuning**](https://github.com/luqman304/lora-finetuning) | LoRA fine-tuning of Qwen2.5-0.5B for Banking77 intent classification: 92.9 % accuracy against 76.2 % few-shot, with bootstrap confidence intervals, tests, CI and Docker. | PyTorch · Hugging Face PEFT · Docker |
| [**road-damage-detection**](https://github.com/luqman304/road-damage-detection) | YOLO11 road-defect detector trained on RDD2022 across six countries: mAP@0.5 0.595, with per-class and per-country breakdowns and severity scoring. Served as a Dockerised FastAPI app, [live on Render](https://road-damage-detection-le7h.onrender.com). | YOLO11 · PyTorch · FastAPI · Docker · Render |

Also worth a look: [**earthquake-dq-pipeline**](https://github.com/luqman304/earthquake-dq-pipeline) — a dbt + DuckDB
pipeline over live USGS data with 38 data-quality tests, a CI gate that proves the checks fire, and
[published lineage docs](https://luqman304.github.io/earthquake-dq-pipeline/) — and
[**guarded-text-to-sql-agent**](https://github.com/luqman304/guarded-text-to-sql-agent), a read-only SQL agent
with code-enforced guardrails: 98 % on a 50-question eval and 49/49 red-team attacks blocked.

---

### Tech

**Languages:** Python, SQL, TypeScript
**ML / LLM:** PyTorch, Hugging Face Transformers, scikit-learn, LightGBM, PyTorch Geometric, YOLO, LoRA / PEFT, RAG, LLM-as-judge evaluation
**Retrieval:** Qdrant, ChromaDB, hybrid dense + BM25 search, cross-encoder reranking
**Data:** dbt, DuckDB, pandas, data-quality testing and lineage
**Back end:** FastAPI, Django, Streamlit
**Ops:** Docker, Docker Compose, GitHub Actions, pytest

**Evaluation first:** every project above is scored against a baseline with confidence intervals, and the
result is reported even when the simpler method wins.
