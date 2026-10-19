# RWE Insight Copilot

Ask a real-world evidence question in plain English, such as
"Compare 12-month persistence on sitagliptin vs. sulfonylureas in patients 65+
with type 2 diabetes," and get a validated cohort analysis back: attrition,
propensity-score-matched Kaplan-Meier curves, a hazard ratio, and a
plain-English summary with its assumptions.

**Status:** in progress

**Data:** CMS 2008–2010 DE-SynPUF (synthetic Medicare claims). Results
demonstrate the method and are not clinical findings.

**Stack:** Python · DuckDB · Claude API · lifelines · Streamlit

## Setup
1. `python -m venv .venv`, activate it, then `pip install -r requirements.txt`
2. Copy `.env.example` to `.env` and add your Anthropic API key
3. Download DE-SynPUF Sample 1 into `data/raw/`
