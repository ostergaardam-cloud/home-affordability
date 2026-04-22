# 🏠 HomeReady — Home Affordability Assessment Tool

**A comprehensive, interactive tool that helps first-time home buyers understand if they're financially ready to purchase a home — and what it takes to get there.**

Unlike basic mortgage calculators, HomeReady builds a complete financial picture and gives you a **Readiness Score**, actionable guidance, and a personalized timeline to homeownership.

---

## ✨ Features

### Two Modes
- **⚡ Quick Check** — Answer 4–5 questions, get an instant affordability estimate using smart defaults
- **📋 Detailed Analysis** — Enter your full financial picture for a precise, personalized assessment

### Readiness Score (0–100)
A weighted score across four factors:

| Factor | Weight | Full Score When |
|--------|--------|-----------------|
| Housing-to-Income Ratio | 30 pts | ≤ 28% |
| Debt-to-Income Ratio | 30 pts | ≤ 36% |
| Down Payment % | 20 pts | ≥ 20% |
| Cash Flow Cushion | 20 pts | ≥ 15% of income remaining |

### Smart Financial Calculations
- **Purchase Verdict** — Clear recommendation: ✅ Affordable, ⚠️ Stretching, or 🚫 Not Recommended
- **"What Can I Afford?"** — Binary-search algorithm finds your maximum recommended home price
- **Income Tax Estimator** — Federal + state + FICA using real 2025/2026 brackets, standard or itemized deductions, child tax credits, and pre-tax retirement/HSA adjustments
- **County-Level Property Tax** — 2,700+ US counties with effective tax rates sourced from Census ACS data
- **State Insurance Rates** — Auto-suggests homeowner's insurance as a percentage of home value
- **PMI Calculation** — Automatically included when down payment is below 20%

### Planning & Scenario Tools
- **🎯 What Would Have to Be True?** — Five interactive sliders (income, down payment, expenses, debt, mortgage rate) with live score updates. Includes per-slider "Find Target" auto-solve and a multi-variable "Optimize All" button.
- **📅 When Will I Be Ready?** — Month-by-month simulation accounting for:
  - Savings growth with compound investment returns
  - Annual income growth (with marginal tax rate adjustments)
  - Home price appreciation
  - Expense inflation
  - Debt paydown
  - Configurable lending flexibility (Conservative / Moderate / Aggressive)

### Detailed Expense Tracking
- **Income Taxes** — Known amount ($ or %) or full estimator with filing status, state, dependents, and standard vs. itemized deductions
- **Retirement** — Pre-tax (401k/403b) and post-tax (Roth) contributions in $ or % of income
- **HSA Contributions** — Pre-tax health savings
- **Other Savings** — College funds, emergency fund, brokerage contributions
- **Living Expenses** — Customizable categories (groceries, transportation, utilities, subscriptions, etc.)
- **Debt Payments** — Itemized monthly obligations

### Quality of Life
- **Auto-save** — All inputs persist in localStorage automatically; never lose your work
- **Collapsible Accordions** — Sections expand/collapse to reduce scrolling
- **Marginal Tax Awareness** — WWHBT income slider accounts for taxes on incremental income
- **Print / PDF** — Clean print-friendly output via browser print dialog

---

## 📁 Project Structure

```
index.html              # The entire application
county-tax-data.js      # County-level property tax rates (~2,700 counties, all 50 states + DC)
README.md               # This file
```

---

## 🚀 Getting Started

No build tools, no frameworks, no dependencies. Just open the HTML file.

### Local Development
```bash
# Clone the repo
git clone https://github.com/YOUR-USERNAME/home-affordability.git
cd home-affordability

# Open in browser (Windows)
start index.html

# Open in browser (macOS)
open index.html
```

### Deploy to GitHub Pages
1. Push `index.html` and `county-tax-data.js` to a public GitHub repo
2. Go to **Settings → Pages → Source: Deploy from branch (main, / root)**
3. Your site will be live at `https://YOUR-USERNAME.github.io/home-affordability/`

---

## 🌐 Live Demo

[View on GitHub Pages →](https://ostergaardam-cloud.github.io/home-affordability/)

---

## 📊 Data Sources

| Data | Source |
|------|--------|
| Federal tax brackets | IRS Revenue Procedures (2025/2026) |
| State income tax rates | Tax Foundation |
| County property tax rates | US Census ACS (B25103 / B25077) |
| State insurance rates | Insurance Information Institute / NAIC |

---

## 🛠️ Tech Stack

- **Vanilla HTML, CSS, JavaScript** — zero dependencies
- **Single-file architecture** (+ one data file)
- **LocalStorage** for persistence
- **Fully client-side** — no server, no API keys, no data collection

---

## 🔒 Privacy

All data stays in your browser. Nothing is sent to any server. Your financial information is stored only in your browser's localStorage and can be cleared at any time by clearing your browser data.

---

## 📋 Roadmap

- [ ] Mobile responsiveness polish
- [ ] PWA support (offline use, installable to home screen)
- [ ] Zip-code-level property tax lookup
- [ ] Amortization schedule chart
- [ ] Rent vs. Buy comparison mode
- [ ] Closing costs estimator
- [ ] Multiple scenario save/compare
- [ ] Dark mode toggle

---

## 📄 License

© 2026 All rights reserved. This software is provided for personal, non-commercial use only. You may not copy, modify, distribute, or create derivative works without explicit written permission from the author.

---

*Built with care for first-time home buyers navigating one of life's biggest financial decisions.*
