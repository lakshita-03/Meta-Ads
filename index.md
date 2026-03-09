# Meta Ads Performance Analytics

<img src="pictures/fb-ad-format.png" alt="banner" width="35%"><img src="pictures/meta_ads.webp" alt="banner" width="35%">   

**Dark patterns** in e-commerce are deceptive user interface designs that manipulate shoppers into making unintended purchases or sharing more data, using tactics like false urgency (countdown timers), basket sneaking (adding items to cart), confirm shaming (guilt-tripping opt-outs), subscription traps (hard-to-cancel free trials), hidden costs (drip pricing), and disguised ads, all designed to boost company profits at consumer expense, leading to increased regulatory scrutiny and consumer awareness efforts. 

### Table of Contents (CHANGE)
Project Overview
Problem Statement & Business Objective
Dataset Description
Data Cleaning & Preprocessing
Exploratory Data Analysis (EDA)
Funnel & Behavioral Analysis
Dark Pattern Signal Identification
SQL-Based Analysis
Python-Based Behavioral Modeling
Machine Learning for Abandonment Prediction
Power BI Dashboards & Visualizations
Insights & Key Findings
Ethical UX Recommendations
Conclusion

### Problem Statement
- E-commerce platforms are heavily optimized for maximizing conversions and revenue. However, aggressive optimization strategies can unintentionally introduce user experience (UX) friction or manipulative design elements commonly referred to as **dark patterns** that influence user behavior in ways that may reduce trust and long-term customer value.
Such patterns often manifest as repeated cart interactions, prolonged decision-making without conversion, or frequent abandonment during checkout. While these behaviors do not explicitly prove unethical design, they act as **behavioral risk signals** that warrant investigation.

- This project aims to analyze user journey and session-level behavioral data to identify friction indicators that may suggest potential dark pattern risks in an e-commerce environment. By examining funnel drop-offs, cart interactions, session duration, and abandonment behavior, the analysis seeks to quantify how these signals impact conversion performance. The ultimate objective is not to accuse or label design practices, but to provide **data-driven insights** that help businesses balance conversion goals with ethical, user-centric design—supporting improved trust, retention, and sustainable growth.

DATASET,CLEAN,EDA,FUNNEL THEN SQL


### Funnel Definition & Metrics
#### Funnel Structure
To analyze user behavior and potential friction signals, the following e-commerce funnel is defined based on user interaction events:

| Funnel Stage      | Event Type         |
| ----------------- | ------------------ |
| Product Discovery | `view`             |
| Intent Formation  | `cart`             |
| Friction Signal   | `remove_from_cart` |
| Conversion        | `purchase`         |

The `remove_from_cart` event is treated as a **behavioral friction signal** rather than a funnel stage, as it reflects user hesitation or uncertainty during the decision-making process.

#### Core Metrics Tracked
**Conversion Metrics**

* View → Cart Conversion Rate
* Cart → Purchase Conversion Rate
* Overall Conversion Rate
* Funnel Drop-off Rates by Stage

**Friction & Dark Pattern Risk Indicators**

* Cart Abandonment Rate
* Average Cart Removals per Session
* Rapid Add-to-Cart and Abandonment Percentage
* Average Session Duration without Purchase

**Session-Level Behavioral Metrics**

* Session Duration
* Total Events per Session
* Cart Event Count
* Remove-from-Cart Event Count
* Purchase Flag (Binary)
* Abandonment Flag (Binary)

These metrics enable both high-level funnel analysis and granular session-level behavioral investigation, forming the foundation for SQL aggregation, Python-based pattern analysis, and optional predictive modeling.

------------------------------------------------------------------------------------------------------------------------------
Meta Ads Performance, Audience & Targeting Effectiveness Analysis
using SQL & Power BI
Digital marketing teams need more than surface-level metrics to optimize advertising performance. This project performs an in-depth analysis of Meta advertising data by combining campaign metadata, ad targeting information, user demographics, and event-level interaction data. The objective is to evaluate campaign effectiveness, user engagement patterns, targeting alignment, platform performance, and conversion behavior to identify optimization opportunities and reduce inefficient ad spend.
  
