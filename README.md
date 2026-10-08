<h1 align="center">Hi, I'm Krishna Sharma 👋</h1>

<p align="center">
  <b>AI Data Engineer</b> · Databricks · PySpark · GenAI &amp; Agents<br>
  📍 Bengaluru, India
</p>

<p align="center">
  <a href="https://linkedin.com/in/krishnasharma18"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge" alt="LinkedIn"></a>
  <a href="mailto:1212.krishnasharma@gmail.com"><img src="https://img.shields.io/badge/Email-Say%20hi-EA4335?style=for-the-badge" alt="Email"></a>
</p>

---

I'm a data engineer who builds the pipelines **and** the AI that runs on top of them. I work with Spark and Microsoft Fabric pipelines day to day, and I build lakehouse platforms and LLM agents on Databricks in my own time.

My one rule: **if you can't measure it, it isn't done.** Pipelines get data-quality checks. AI features get evals, written before the code.

## 🔭 What I'm working on right now

- 🏗️ A medallion **lakehouse** on Databricks: Auto Loader → Delta → Lakeflow Jobs, with before/after Spark optimization numbers
- 🤖 A **Lakehouse Copilot**: RAG + text-to-SQL agent + MCP server, evaluated with MLflow
- 🔬 Spark internals: skew, shuffles, AQE, spill, small files, learned by breaking things and reading the Spark UI
- 🎓 Databricks certifications (see below)

## 🚀 Featured projects

### 🏗️ Lakehouse Medallion Platform
![Status](https://img.shields.io/badge/status-in%20progress-orange)
<!-- After shipping (Nov 15): replace the badge above with
![Status](https://img.shields.io/badge/status-shipped-brightgreen)
and add one line with real optimization numbers, e.g. "Cut gold build from X min to Y min (skew fix + broadcast join)". -->

End-to-end batch lakehouse on Databricks: raw files to analytics-ready star schema, with quality gates and orchestration.

- **Bronze:** Auto Loader ingestion with lineage columns and rescued-data handling
- **Silver:** dedup, typing, quarantine table for bad records, **SCD Type 2** dimension via `MERGE`
- **Gold:** star schema (`fact_events`, `dim_user`, `dim_product`, `dim_date`) plus aggregate tables
- **Reliability:** data-quality checks, Lakeflow Job running bronze → silver → gold → DQ

`Databricks` `PySpark` `Delta Lake` `Lakeflow` `Unity Catalog` `SQL`
👉 [View repo](https://github.com/YOUR_USERNAME/lakehouse-medallion)

### 🤖 Lakehouse Copilot (agentic RAG + text-to-SQL)
![Status](https://img.shields.io/badge/status-in%20progress-orange)
<!-- After shipping (Dec 13): swap badge to "shipped" and add your eval table summary,
e.g. "Faithfulness 0.__ → 0.__ after adding hybrid search + reranking". -->

A copilot that answers questions over both documents and warehouse tables, and can tell which one a question needs.

- **RAG:** hybrid search (BM25 + vector) with reranking, citations, and refusal when the answer isn't in the docs
- **Text-to-SQL tool** over the gold tables from the lakehouse project
- **LangGraph agent** routing between docs, SQL, or both, exposed through an **MCP server**
- **Evals first:** a 40-question eval set built before the code; every change tracked in **MLflow**

`Python` `FastAPI` `LangGraph` `MCP` `MLflow` `Databricks AI Search`
👉 [View repo](https://github.com/YOUR_USERNAME/lakehouse-copilot)

## 📜 Certifications

| Certification | Status |
|---|---|
| Databricks Certified Data Engineer Associate | 🎯 In progress · exam Nov 2026 |
| Databricks Certified Generative AI Engineer Associate | 🎯 In progress · exam Dec 2026 |

<!-- After passing: change the status to "✅ Certified · Month 2026" and link the credential. -->

## 🛠️ Tech stack

| Area | What I use |
|---|---|
| **Data engineering** | PySpark · Spark SQL · Delta Lake · Databricks (Lakeflow, Unity Catalog) · Microsoft Fabric · dimensional modeling |
| **AI engineering** | RAG (hybrid search, reranking) · LLM tool calling · LangGraph · MCP · MLflow evals · Databricks AI Search |
| **Languages & tools** | Python · SQL · FastAPI · Git/GitHub · pytest |

## 💼 Experience in brief

- Build and maintain **Spark and Microsoft Fabric data pipelines** for a large enterprise automotive client (~1.5 years).
- Fluent in both worlds: I can map **Fabric → Databricks** (OneLake and Lakehouse to Delta and Unity Catalog, Data Pipelines to Lakeflow Jobs) and redesign a pipeline on either.
<!-- Add real numbers once you've done your metric mining, e.g. "X pipelines, ~Y GB/day, runtime A → B min, Z downstream consumers". Only add numbers you can defend in an interview. -->

## 🧭 How I work

- **Grain first** in data models, **evals first** in AI systems.
- **Ship weekly.** Commits are small and frequent, and every project README has real numbers.
- **Debug with evidence:** Spark UI signals, query plans, traces. Not guesses.

---

<p align="center">
  Questions about lakehouses, Spark performance, or RAG evals? Reach out on <a href="https://linkedin.com/in/krishnasharma18">LinkedIn</a> or <a href="mailto:1212.krishnasharma@gmail.com">email</a>.
</p>
