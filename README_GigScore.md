# GigScore — Behavioral & Graph-Based Credit Intelligence for Thin-File Borrowers

GigScore is an AI-driven credit risk assessment system that underwrites borrowers without formal credit history using transaction behavior, cash-flow dynamics, and network trust signals. The system generates an explainable credit score, risk tier, and structured loan offer in real time.

Unlike traditional bureau-based scoring, GigScore evaluates financial behavior, income stability, obligation discipline, and transaction network reliability to assess repayment capacity.

---

## System Architecture

GigScore is built as a multi-agent decision pipeline where each component contributes to the final credit decision:

| Agent | Function |
|------|---------|
| Agent 0 | Bank statement parsing, feature extraction, PII redaction |
| Agent 1 | Behavioral & financial feature engineering |
| Agent 2 | Default risk prediction using Gradient Boosting |
| Agent 3 | Social trust graph scoring + behavioral adjustment |
| Agent 4 | Final GigScore calculation + explainability |
| Agent 5 | Credit Story Chatbot (borrower-facing explanation) |
| Agent 6 | Loan structuring (amount, EMI, FOIR, interest rate) |

The pipeline produces a fully explainable credit decision, not just a risk score.

---

## Credit Scoring Methodology

The GigScore combines multiple layers of risk assessment:

- Default Risk Model – Predicts probability of default from behavioral and financial features.
- Cash-Flow Stability – Income consistency, inflow/outflow ratios, and financial discipline.
- Social Trust Graph – Transaction network reliability and stability of counterparties.
- Behavioral Signals – Streaks, obligation ratios, and financial habits relative to cohort baseline.
- Explainability Layer – SHAP-based feature attribution for transparent decision-making.

The final output is a 0–100 GigScore mapped to risk tiers and loan eligibility.

---

## Explainability & Borrower Interface

GigScore includes an explainability layer designed for financial inclusion:

- Credit Story Chatbot – Explains to borrowers why they received a certain score and how they can improve it.
- IVR Explainability – Voice-based explanation of loan decisions, EMI structure, and improvement actions in simple language.
- 90-Day Improvement Plan – Actionable steps to help borrowers move to a better risk tier.

This converts credit scoring from a black box decision into a transparent financial guidance system.

---

## Outputs Generated

- GigScore (0–100)
- Risk Tier Classification
- Approved Loan Amount
- Interest Rate
- EMI Structure
- FOIR (Fixed Obligation to Income Ratio)
- Explanation for Credit Decision
- Behavioral Improvement Plan

---

## Technology Stack

- Python
- XGBoost (Credit Risk Model)
- SHAP (Explainable AI)
- LangGraph (Multi-Agent Pipeline)
- PDF Parsing & Feature Extraction
- Graph-Based Trust Scoring
- LLM-based Chatbot Interface
- IVR Voice Interface

---

## Use Case

GigScore is designed for:
- Banks
- NBFCs
- Digital Lenders
- Embedded Finance Platforms

It enables underwriting for thin-file borrowers using behavioral and transaction data instead of traditional credit history.

---

## Key Idea

Creditworthiness is not just a function of past loans — it is a function of financial behavior, income stability, and network trust.

GigScore attempts to quantify this.

---

## Team
Barclays Hack-O-Hire 2026  
Team GigScore — Plaksha University
