# Shivam Mishra

**AI Engineer** | LLMs (**RAG**, agents) | NLP | Python

**Open to:** AI Engineer / LLM Engineer / ML Engineer (internship/full-time)| 
**LinkedIn:** https://linkedin.com/in/shivam-mishra-3b354023a | **Email:** mshivam3003@gmail.com | **Phone:** +91 75685 55487

## Recruiter Quick Scan

- **Experience:** AI Engineer Intern @ MySellerCentre (Sep 2025 - Present)
- **Domain:** e-commerce / marketplaces (support automation, listings, catalog content)
- **Core strengths:** **embeddings**, **retrieval**, **RAG**, structured outputs, Python backend
- **Primary stack:** **Python**, **FastAPI**, **Streamlit**, **PostgreSQL**, **MongoDB**
- **Education:** M.Tech (Data Science), NIT Patna (Expected Jun 2026) | **GPA: 8.14/10**

## What I Build

- **LLM apps**: assistants/tools using **RAG** + structured outputs
- **Data pipelines**: scraping -> cleaning/normalization -> enrichment -> storage -> retrieval
- **APIs + demos** for fast iteration with product/business stakeholders

## Skills Snapshot (Keyword-Friendly)

| Category | Skills |
| --- | --- |
| Languages | Python, SQL |
| LLM / GenAI | LLMs, prompt engineering, Retrieval-Augmented Generation (RAG), embeddings, vector search, agentic workflows |
| Frameworks | FastAPI, Streamlit, LangChain, LangGraph |
| LLM Observability | LangSmith, Langfuse |
| Data / Storage | PostgreSQL, MongoDB, Microsoft SQL Server, DuckDB, AWS S3 |
| Web scraping | web scraping, BeautifulSoup, lxml, requests, Zyte API |
| ML / NLP | Transformers, evaluation, feature engineering, spaCy, NLTK |
| Libraries | NumPy, Pandas, SciPy, scikit-learn, XGBoost, LightGBM, CatBoost, PyTorch, TensorFlow/Keras, OpenCV |
| Analytics | EDA, data cleaning, Matplotlib/Seaborn, Power BI, Excel, Google Sheets |

## Featured Projects

### 🚀 ResumeRise AI (Resume Builder + ATS Scoring + Job Scout)
🔗 [View Project](https://github.com/mshivam3003/ats_score)
**Goal:** help candidates tailor resumes to a job description and discover fresh roles (with optional email alerts).

- **Built:** a local **Streamlit** app to (1) **score ATS compatibility** against a JD, (2) **improve the resume with an LLM** while preserving original content, and (3) **find job links** and generate a daily-style job email.
- **Designed:** a hybrid ATS pipeline (**LLM JSON extraction** of signals + **deterministic rule engine**) for consistent scoring and actionable recommendations.
- **Implemented:** resume parsing + exports (PDF/DOCX) and a best-effort job discovery workflow (HTTP fetch + HTML/JSON-LD extraction) with SMTP/Outlook fallback for sending.

**Demo:** https://conversational-ai-147.preview.emergentagent.com/

**Tech:** Python, Streamlit, OpenRouter (via `openai` SDK), PyPDF2, python-docx, requests, lxml, SMTP, (optional) Outlook/pywin32

### Mixed-Infection Sugarcane Leaf Disease Classification (GenAI Synthetic Data + Multi-Level Transformer)
**Project Status**
- **Stage:** prompt bank + initial generation experiments completed; training the upgraded classifier is ongoing.

**Resume/Recruiter Summary (Copy-Paste Friendly)**
- Built a **prompt-engineered synthetic dataset plan** to address **mixed infection** gaps in sugarcane leaf disease classification (MLTSDC extension).
- Curated **48 structured prompts** covering **4 overlapping disease pairs**, **3 severity levels**, and **4 climate conditions** to improve real-field generalization.
- Evaluated baseline training sensitivity to optimizer/learning-rate choices; identified **data coverage** (not hyperparameters) as the primary bottleneck.
- Achieved **85.30% overall testing accuracy (preliminary)** with the proposed multi-level model vs **65.23%** with baseline MLTSDC on the current split (per `Research work.pptx`).
- Prototyped a workflow to generate realistic leaf images using **GenAI models** (open/free options when paid APIs are restrictive).

**Concise (1–2 lines)**
Using GenAI (LLM-driven prompt engineering) to extend the MLTSDC transformer pipeline for sugarcane leaf disease detection by addressing the real-world gap of mixed/co-occurring infections via a structured synthetic-data workflow (48 prompts across disease pairs × severity × climate), improving preliminary overall test accuracy from **65.23%** (baseline MLTSDC) to **85.30%** (proposed multi-level model).

**Detailed (resume-ready bullets)**
- **Problem:** baseline sugarcane disease classifiers (including MLTSDC) perform well on single-disease labels but degrade in farm conditions due to mixed infections (symptom overlap) and environmental variability (lighting/climate).
- **Proposed solution:** designed a hierarchical multi-level transformer-based pipeline (Patch Encoder + AI Blocks) with staged decisions: Level-1 Healthy/Unhealthy → Level-2 Single/Mixed → Level-3 single-disease class → Level-4 mixed-disease class.
- **Synthetic data strategy:** built a prompt bank (`prompt.csv`) of **48 high-constraint prompts** covering **4 overlapping disease pairs** (A: Mosaic+Red Rot, B: Mosaic+Yellow, C: Mosaic+Rust, D: Red Rot+Rust) × **3 severities** (Early/Mid/Severe) × **4 conditions** (Natural light/Humid/Dry/Rainy) to generate realistic **256×256** field-like leaf images.
- **Experiments:** ran optimizer sweep on baseline MLTSDC (LR=0.001, 10 epochs) showing limited gains from hyperparameter changes, indicating **data coverage** as the key bottleneck.
- **Results (from `Research work.pptx`):** achieved **85.30%** preliminary overall testing accuracy with the proposed model vs **65.23%** with baseline MLTSDC; Level-2 improved substantially (**91.15%** test) for single/mixed discrimination, while deeper mixed-class levels remain an ongoing improvement area.
- **Engineering:** implemented a post-processing pipeline (`post_process.py`) to standardize generated images (RGB, crop/resize to 256×256, JPEG quality 90), enforce ID→prompt mapping, and export a manifest for dataset QA and reproducibility.
- **Tools/stack:** Python, TensorFlow/Keras (transformer/CV), prompt engineering, GenAI image generation workflow (Stable Diffusion/FLUX/Gemini-style models), dataset structuring + experiment tracking.

## Experience

### AI Engineer Intern - MySellerCentre (Sep 2025 - Present)
- Built **LLM/NLP** solutions using Python, embeddings, and retrieval workflows to automate marketplace operations.
- Developed **data pipelines** for scraping, processing, and analyzing product/catalog data.
- Delivered internal tools and prototypes to improve product listings and seller support workflows.

#### Selected Work Projects

**Multi-Marketplace Seller Support Chatbot (RAG) (Jan 2026 - Feb 2026)**
- Built a seller support chatbot that answers **policy/refund/compliance** questions using **RAG** over internal documents.
- Worked on knowledge organization, chunking strategy, and retrieval quality to keep answers grounded and consistent.
- Shipped a demo-ready **FastAPI + Streamlit** experience to validate end-to-end flows with stakeholders.

**Cross-Marketplace ONDC Listing Generator (Dec 2025 - Jan 2026)**
- Built an agent-style workflow to extract product info, map categories via **embeddings**, and generate **ONDC-compliant** listings using an LLM.
- Created a review UI to verify extracted/enriched fields and reduce errors before final listing export.
- Designed a structured pipeline from **raw HTML -> normalized fields -> enriched attributes -> compliant output**.

**Product Content Enhancer for E-commerce (Oct 2025 - Dec 2025)**
- Built an LLM-powered tool to improve **titles**, **bullets**, and **descriptions** with structured prompts and validation rules.
- Implemented batch processing (queue + workers) to handle larger catalogs reliably.
- Standardized output format to improve readability and reduce manual edits.

## Education

- M.Tech (Data Science) - **National Institute of Technology**, Patna (Expected Jun 2026) | **GPA: 8.14/10**
- B.Tech (Computer Science) - **Gurukula Kangri University (Jun 2024)** | **GPA: 8.51/10**

## Certifications

- The Joy of Computing Using Python - NPTEL (May 2025)
- Data Analytics - Udemy (Jul 2025)
- Data Science - Devtown (Jul 2025)

## Contact
- LinkedIn: https://linkedin.com/in/shivam-mishra-3b354023a
- Email: mshivam3003@gmail.com
- Phone: +91 75685 55487


