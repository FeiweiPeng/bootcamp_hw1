# Project Title
**Stage:** Problem Framing & Scoping (Stage 01)  

## Problem Statement
The project aims to design and evaluate an intraday momentum trading strategy for highly liquid U.S. equity ETFs, such as SPY and QQQ. The goal is to capture short-term price trends within the trading day by identifying periods of sustained directional movement. This strategy is intended to improve intraday returns while controlling for drawdowns and transaction costs. By systematically testing momentum signals and execution rules, the strategy will provide a robust framework for short-horizon trading decisions.

## Stakeholder & End User
**Primary Stakeholder (Decision Owner):** Portfolio Manager at a proprietary trading firm  
**End User(s):** Quantitative research team, execution traders  
**Decision Window:** Daily, with trades initiated and closed within market hours

## Useful Answer & Decision
**Answer Type:** Predictive  
**Form of Output:** Ranked list of ETFs with intraday momentum scores, recommended entry/exit times, and expected return bands  
**How It Will Be Used:** The research team will integrate the momentum signals into the daily trading plan, with execution traders acting on the entry/exit recommendations to capitalize on short-term price movements.

## Assumptions & Constraints
- Assumption: Liquidity in selected ETFs will remain high enough for low-slippage execution.
- Constraint: All trades must be closed before market close to avoid overnight risk.

## Known Unknowns / Risks
- Risk: Transaction costs and slippage could erode theoretical returns.

## Lifecycle Mapping
Goal → Stage → Deliverable  
- Identify viable intraday momentum signals → Problem Framing & Scoping (Stage 01) → Scoping paragraph, stakeholder memo, repo skeleton  
- Backtest momentum-based entry/exit rules → Research & Modeling (Stage 02) → Performance report and analysis notebook  
- Deploy real-time signal generation → Deployment (Stage 03) → Production-ready execution scripts

## Repo Plan
/data/ — store cleaned intraday price data  
/src/ — reusable functions for data processing
/notebooks/ — Jupyter notebooks for exploratory data analysis and performance testing  
/docs/ — stakeholder memo
