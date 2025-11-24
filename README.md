# DeFi-Liquidity-Risk-Dashboard
This document expands the previous plan into concrete, runnable steps with code snippets, GraphQL queries, SQL/duckDB examples, model skeletons, causal-analysis code, and a minimal Streamlit app.
It's organized by phase: ETL/backfill, storage & OLAP, baseline dashboard, forecasting models, causal analysis & shock simulator, and deployment/tests. Use this as a recipe — copy the code into your repo and adapt endpoints/keys.

Table of contents
Setup & config
ETL: backfill top pools (GraphQL + Python)
Building hourly pool_snapshot (DuckDB/Parquet)
Enrichment: token prices, exchange inflows
Baseline dashboard (Streamlit) — Sankey + heatmap
Forecasting: baseline LightGBM and TCN skeleton
Causality: Granger, Transfer Entropy, DoWhy example
Shock simulator (deterministic + causal-adjusted)
QA, tests, and monitoring
Next steps & where to run things
