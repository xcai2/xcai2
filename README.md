# Xin Cai

MSIS @ Santa Clara University. I build AI-powered analytical systems that turn messy filings, news, and operational data into something a decision-maker can actually act on.

## What I'm Building

### 🎯 Flex Competitive Intelligence Platform — *Practicum capstone*
**[Flex-Practicum-Project-2026](https://github.com/xcai2/Flex-Practicum-Project-2026)**

An AI-powered competitive intelligence tool built for Flex to monitor its five closest competitors in contract manufacturing — Jabil, Celestica, Benchmark, Sanmina, and Plexus. Team of four over 12 weeks as our SCU practicum project.

**What it does.** Ingests ~405 SEC filings (10-K, 10-Q, earnings calls), USPTO patents, job postings, and real-time news across all six companies, embeds everything into ChromaDB (768-dim sentence transformers), and answers natural-language questions by retrieving relevant chunks and running them through Claude with citations. Hybrid mode merges document retrieval with live Brave Search so answers stay current past the filing date.

**Beyond chat.** A Claude-powered sentiment analyzer tracks management tone across quarters, CapEx anomaly detection surfaces unusual spending, an AI-vs-traditional investment classifier tags where the money is going, and a Leaflet-based heatmap plots **221 facilities** extracted from filings. Financial data and news for all six companies update continuously. Any view exports to Excel, PowerPoint, or PDF; alerts push to email/Slack when anomalies trigger.

**My role.** I led two end-to-end modules — the **Geographic Map** (facility extraction from unstructured filings into the 221-point map) and the **Earnings Calendar** (dynamic scheduling across six companies). Across the wider system my focus was **RAG accuracy**: iterating on extraction logic and parameter choices to push retrieval precision upward so the chat answers would actually hold up to scrutiny.

**Stack.** Python · FastAPI · ChromaDB · Sentence Transformers · Claude API · Next.js 16 · Tailwind · shadcn/ui · Recharts · Leaflet · APScheduler.

**Team.** Xin Cai · Srinidhi Jagannathan · Heliang Gao · Xinyi Liu · with Lucas as external contributor.

---

### [Instacart Market Basket Analysis](https://github.com/xcai2/Instacart-Market-Basket-Analysis) — *Next-order product prediction*
Framed next-basket prediction as a per-user, per-product binary classification problem on 3M+ Instacart orders. Engineered features at six levels (product, aisle, department, user, user×aisle/department, user×product) and compared a recent-purchase baseline against logistic regression, LightGBM, and XGBoost. Evaluation by F1@K, precision, recall, and ROC-AUC. Includes a full case-study walkthrough for a single user — predicted basket, error analysis, what the model got wrong and why.

### [Hotel Booking Analysis](https://github.com/xcai2/hotel-booking-analysis) — *Marketing analytics on 119K bookings*
EDA on a 2015–2017 hotel bookings dataset (City Hotel + Resort Hotel, 32 variables), enriched with FRED CPI, INE Portugal tourism stats, Eurostat European tourism, and seasonal indices to place findings in macro context. Three things worth acting on: a **37% overall cancellation rate** driven mostly by City Hotel long-lead bookings, a **3.2% repeat-customer rate** flagging a real loyalty gap, and an **80%+ dependency on travel-agent channels**. Each translates into a concrete marketing question — deposit policy, loyalty program design, channel mix and dynamic pricing.

## How I Work

I care less about squeezing the last point of accuracy out of a model and more about whether the answer survives contact with a real user. On the Flex project that meant treating RAG accuracy as a product metric, not a benchmark — if a Flex analyst wouldn't trust the citation, the retrieval logic had to change regardless of what offline metrics said. Most of my projects go the same way: start from a decision someone has to make, work backward to what the data can and can't answer, iterate until the answer holds up.

## Tech Stack

**Languages** Python · SQL · R
**ML & Analysis** pandas · scikit-learn · LightGBM · XGBoost · Sentence Transformers
**AI Systems** Claude API · ChromaDB · RAG pipelines · FastAPI
**Frontend** Next.js · Tailwind · shadcn/ui · Recharts · Leaflet
**Tools** Jupyter · Tableau · Git

## Connect

📧 xcai2@scu.edu
💼 [LinkedIn](https://www.linkedin.com/in/celia-cai-96a887383/)
🎓 Santa Clara University · MSIS
