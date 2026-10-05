# Rachana Nijalingappa

AI Engineer and Backend Engineer. I build LLM and RAG applications in Python, on top of 5+ years of production backend work in C#, .NET and Azure for banking and healthcare. MSc Artificial Intelligence, Brunel University London (2026).

Based in Birmingham, open to AI Engineer and Backend Engineer roles across the UK.

**Portfolio:** [rachananijalingappa.github.io/rachana-n.github.io](https://rachananijalingappa.github.io/rachana-n.github.io/)

---

## Projects

### Agentic RAG for Multi-Source Financial QA (MSc dissertation)
- Built and compared five QA methods in LangGraph with GPT-4o-mini over 10-Q filings and yfinance market data.
- Static routing raised answer correctness from 56.7% (single-source RAG) to 91.8% on 97 scorable questions, with 97.6% exact-match source selection on 125 routable questions.
- **Stack:** Python, LangGraph, ChromaDB, GPT-4o-mini, RAGAS, BERTScore, yfinance

### [DocChat: Routed RAG Service](https://github.com/rachananijalingappa/DocChat_RAG) ([live demo](https://huggingface.co/spaces/rachana28/DocChat-Advanced-RAG))
- LangGraph router sends each query to document retrieval or a web-search fallback, replacing a single-path RAG pipeline.
- Retrieval with ChromaDB, contextual compression and Cohere re-ranking; LLM-as-a-judge scoring for faithfulness and relevance; prompt-injection screening; LangSmith tracing.
- Pilot evaluation on 15 synthetic questions: re-ranking raised mean faithfulness from 0.92 to 0.99. The LLM-based injection pre-check flagged all 20 standard injection templates tested [and 0 of N benign questions].
- **Stack:** Python, LangGraph, LangChain, FastAPI, Streamlit, OpenAI API, Cohere API, ChromaDB, LangSmith, Docker

### [Credit Card Fraud Detection](https://github.com/rachananijalingappa/CreditCard_Fraud_Detection)
- Compared 13 models on 283,726 transactions with 0.17% fraud; SMOTE applied inside CV folds only.
- Optuna-tuned LightGBM (30 trials, 3-fold stratified CV) reached PR-AUC 0.817 and F1 0.859 (precision 0.973, recall 0.768) on a held-out test set.
- **Stack:** Python, scikit-learn, LightGBM, TensorFlow, Optuna, SHAP, pandas

### [ShopNova: .NET Modular Monolith](https://github.com/rachananijalingappa/E-Commerce-Monolith)
- Three bounded contexts (Catalog, Orders, Basket) with 13 REST endpoints, CQRS via MediatR and cross-module domain events (OrderPlacedEvent clears the basket).
- Ocelot API gateway, FluentValidation pipeline, JWT authentication, Serilog correlation IDs, NUnit and Moq tests. Each module's DbContext has its own schema configured; the repo runs on EF Core InMemory so it starts with `dotnet run` and no database setup.
- **Stack:** C#, .NET 8, EF Core, MediatR, Ocelot, Serilog, NUnit, Moq

---

## Tech

- **AI and ML:** Python, LLMs, RAG, LangGraph, LangChain, ChromaDB, OpenAI API, RAGAS, scikit-learn, LightGBM, TensorFlow, SHAP, pandas, R
- **Backend:** C#, .NET 8, ASP.NET Core, FastAPI, REST APIs, CQRS, SQL Server
- **Cloud and tooling:** Azure (Key Vault, Storage, Functions, Service Bus), Docker, CI/CD, Git, NUnit, Moq

---

[LinkedIn](https://www.linkedin.com/in/n-rachana) · [Email](mailto:nrachananijalingappa@gmail.com)