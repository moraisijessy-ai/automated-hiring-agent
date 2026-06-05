# 🚀 Quick Start Guide

## Step 1: Get Claude
Go to https://claude.ai and sign up (free tier works)

## Step 2: Load the Prompt
Copy this URL:
https://raw.githubusercontent.com/moraisijessy-ai/automated-hiring-agent/main/prompts/system_prompt.md

Paste into Claude with:
"Please follow this system prompt: [paste text]"

## Step 3: Run a Query
Example:
"Find 10 researchers working on deceptive alignment at Anthropic from 2023-2026. Include email and LinkedIn."

## Step 4: Get Results
Receive a markdown table sorted by relevance score (0.0-1.0)

---

## Query Template
Find [NUMBER] researchers working on [TOPIC] at [SOURCES] from [TIMEFRAME].
Include [CONTACT FIELDS] when available.


### Examples:

**Basic:**
"Find 5 researchers working on AI scheming at DeepMind from 2024-2026."

**Conference:**
"List 15 authors of papers on reward hacking at NeurIPS 2024."

**Contact-focused:**
"Find 10 researchers at FAR AI working on AI safety. Prioritize email addresses."

---

## Tips

✅ Specify search limit (default: 10)
✅ Be specific about timeframe
✅ Add "Return ONLY the table" if Claude adds explanations
✅ Results include only researchers with score ≥ 0.30
