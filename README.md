# ✈️ Customer Loyalty Program Analytics

> **Power BI dashboard analysing customer lifetime value and promotional cohort effectiveness for an airline loyalty program**

---

## 🎯 Business Problem

Northern Lights Air wanted to evaluate their loyalty program promotion. The key question: **Do customers acquired through promotional offers deliver higher lifetime value than standard enrollees?**

The challenge: Raw data showed misleading results due to time bias — promotional members (enrolled 2018) had less time to accumulate value compared to standard members (enrolled earlier).

---

## 📊 Key Findings

| Metric | Promotion Members | Standard Members | Insight |
|--------|-------------------|------------------|---------|
| **Average CLV** | £8,047 | £7,435 | +8.2% higher for promotion cohort |
| **Cancellation Rate** | 11.8% | 14.8% | Lower churn for promotion members |

### Critical Discovery

Initial analysis showed standard members with higher CLV — but this was **time bias**. By implementing controlled cohort comparison (Feb-Apr 2017 vs Feb-Apr 2018 enrollees), the true picture emerged: **promotion members are more valuable and more loyal**.

---

## 📈 Dashboard Pages

### Page 1: Customer Value Analysis
![Customer Value Analysis](Customer%20Value.jpg)

Compares CLV distribution and cancellation rates between promotion and standard cohorts, controlling for enrollment timing.

### Page 2: Flight Activity
![Flight Activity](Flight%20Activity.jpg)

Analyses booking patterns, flight frequency, and travel behaviour across member segments.

### Page 3: Promotion Impact
![Promotion Impact](Promotion%20Impact.jpg)

Evaluates the overall effectiveness of the promotional campaign on member acquisition and retention.

---

## 🛠️ Technical Implementation

### DAX Measures (19 total)
Organised in display folders for maintainability:
- **CLV Calculations** — Customer lifetime value by segment
- **Cohort Metrics** — Controlled comparisons with time-period filters
- **Cancellation Analysis** — Churn rates by enrollment type

### Key Technical Challenges Solved
- **Time Bias Correction**: Implemented page-level filters to ensure fair cohort comparison (Feb-Apr enrollment windows)
- **Filter Context Management**: Resolved nested CALCULATE/USERELATIONSHIP conflicts causing negative running totals
- **Data Modelling**: Calculated columns for derived metrics, proper relationship handling

---

## 🏦 Banking & Fintech Applications

This methodology directly transfers to financial services:

| Loyalty Program Analysis | Banking Equivalent |
|--------------------------|-------------------|
| Promotion vs standard member CLV | Credit card reward tier effectiveness |
| Enrollment cohort comparison | Product launch performance by vintage |
| Cancellation rate by segment | Deposit account churn by acquisition channel |
| Booking frequency patterns | Transaction frequency by customer tier |

---

## 💡 Skills Demonstrated

- **Customer Lifetime Value (CLV)** — Core metric for banking customer analytics
- **Cohort Analysis** — Controlled comparison methodology for fair evaluation
- **Bias Detection** — Identifying and correcting time-based comparison errors
- **DAX** — Complex measures, filter context, display folders
- **Business Storytelling** — Three-page narrative structure for stakeholders

---

## 📁 Files

| File | Description |
|------|-------------|
| `airline_loyalty_program.pbix` | Power BI dashboard (requires [Power BI Desktop](https://powerbi.microsoft.com/desktop/)) |
| `Customer Value.jpg` | Dashboard screenshot — CLV analysis |
| `Flight Activity.jpg` | Dashboard screenshot — Booking patterns |
| `Promotion Impact.jpg` | Dashboard screenshot — Campaign effectiveness |

---

## 🚀 How to View

1. Download [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free)
2. Download the `.pbix` file from this repository
3. Open in Power BI Desktop
4. Explore the three dashboard pages

---

**Built to demonstrate fintech-transferable customer analytics skills**
