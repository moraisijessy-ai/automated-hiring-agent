# 🤖 AI Safety Talent Sourcing Agent

> Find and rank AI safety researchers globally — with comprehensive coverage of alignment, scheming, interpretability, and 40+ related topics. Returns structured results with relevance scores and public contact information.
---

## 🎯 What This Does

This project provides a prompt template for an AI agent (e.g., Claude) that:

- 🔍 **Searches for researchers** working on 40+ AI safety topics
- 🌍 **Global scope** — Not limited to specific countries
- 📊 **Numerical scoring** — Relevance score (0.0-1.0) for ranking
- 📧 **Contact extraction** — Email, LinkedIn, Twitter, website (public only)
- 📋 **Structured output** — Markdown table sorted by score
- 🎯 **Quality-first** — Precision over recall, minimum score threshold
- ❓ **Interactive** — Asks clarifying questions if request is underspecified

---

## 📁 Repository Structure
automated-hiring-agent/
├── prompts/
│ └── system_prompt.md # Main instructions for the AI agent
├── config/
│ └── scoring_rules.txt # Detailed scoring calculation guide
├── tests/
│ └── example_query.txt # Sample queries for testing
└── README.md # You are here

## 📐 Output Format

Results are returned as a **markdown table** with these fields:

| Field | Description |
|-------|-------------|
| **Score** | Relevance score (0.0-1.0) |
| **Name** | Researcher's full name |
| **Organization** | Current institution/lab |
| **Paper** | Relevant publication title |
| **Link** | URL to paper or profile |
| **Email** | Public email address (if available) |
| **LinkedIn** | LinkedIn profile URL (if public) |
| **Twitter** | Twitter/X profile URL (if public) |
| **Website** | Personal/institutional website |

**Requirements:**
- Relevance score ≥ 0.30
- At least 3 of the 8 fields (excluding Score) must be populated with verified information
- Results sorted by Score (highest first)

### Score Interpretation
- **0.80-1.00**: Excellent match, strong evidence, recent work
- **0.60-0.79**: Strong match, good evidence
- **0.40-0.59**: Moderate match, some evidence
- **0.30-0.39**: Minimum threshold, borderline inclusion


## 🔑 Key Features

✅ **Comprehensive topic coverage** — 40+ alignment terms from glossary  
✅ **Flexible timeframe** — User-defined (not fixed to 5 years)  
✅ **Contact extraction** — Email, LinkedIn, Twitter, website when public  
✅ **Source specificity** — Default: AISafety.com/map orgs + major venues  
✅ **Numerical scoring** — Relevance score (0.0-1.0) for ranking  
✅ **Quality-first** — Precision over recall, minimum score threshold 0.30  
✅ **Clarification mode** — Asks questions if request is underspecified  
