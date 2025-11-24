# DeFi-Liquidity-Risk-Dashboard
This document expands the previous plan into concrete, runnable steps with code snippets, GraphQL queries, SQL/duckDB examples, model skeletons, causal-analysis code, and a minimal Streamlit app.
It's organized by phase: ETL/backfill, storage & OLAP, baseline dashboard, forecasting models, causal analysis & shock simulator, and deployment/tests. Use this as a recipe — copy the code into your repo and adapt endpoints/keys.

Table of contents
Setup & config
1. ETL: backfill top pools (GraphQL + Python)
2. Building hourly pool_snapshot (DuckDB/Parquet)
3. Enrichment: token prices, exchange inflows
4. Baseline dashboard (Streamlit) — Sankey + heatmap
5. Forecasting: baseline LightGBM and TCN skeleton
6. Causality: Granger, Transfer Entropy, DoWhy example
7. Shock simulator (deterministic + causal-adjusted)
8. QA, tests, and monitoring
9. Next steps & where to run things
