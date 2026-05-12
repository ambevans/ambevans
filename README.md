## Hi there 👋

- 🔭 I’m currently working on shaping and delivering core money‑management journeys across Upcoming Payments, Subscriptions, and Payday. My focus is on setting clear product direction, prioritising the right customer problems, and ensuring these experiences genuinely help customers feel in control of their money. I work closely with product, engineering, design, and analytics teams to turn insight into outcome, balancing customer needs, commercial impact, and regulatory expectations.

- 🌱 I’m currently learning how to deepen my impact as a leader through advanced data science and analytics, strengthening my ability to use evidence to influence decisions, set strategy, and measure success at scale. Alongside this, I’m continuing to build my capability in Python, Power BI, and analytics storytelling to support more confident, insight‑led leadership conversations.

- 👯 I’m looking to collaborate on complex, cross‑journey problems where clear ownership, strong alignment, and customer‑first thinking are essential — particularly initiatives that span payments, subscriptions, and financial wellbeing. I enjoy partnering with others to define strategy, challenge assumptions, and land change that makes a real difference for customers.

- 🤔 I’m looking for help with evolving how teams use insight to drive prioritisation, improving how we connect customer feedback to strategic roadmaps, and exploring better ways to test, learn, and scale what works across digital journeys.

- 💬 Ask me about leading customer‑centric product strategy, Upcoming Payments and Subscriptions journeys, payday experiences, turning customer insight into executive‑ready recommendations, or using data to support decision‑making and influence at senior levels.

- 📫 How to reach me: www.linkedin.com/in/amber-evans-363035177

- 😄 Pronouns: she/her

- ⚡ Fun fact: Outside work, I’m usually balancing running, Pilates or tennis with cooking something new — and planning my next travel adventure.


# Analysis of Authorised Push Payment (APP) Fraud in the UK

## Project Overview
This project applies an end-to-end data science workflow to analyse trends and risk patterns in Authorised Push Payment (APP) fraud in the United Kingdom. Using publicly available datasets from Action Fraud, UK Finance and the Financial Conduct Authority (FCA), the analysis explores how fraud volumes, financial losses and scam typologies have evolved over time.

The primary aim is to identify which APP fraud typologies pose the greatest financial risk and to demonstrate how analytical insights can support more effective fraud prevention strategies within the financial services sector.

---

## Executive Summary
Authorised Push Payment fraud represents a growing and complex challenge for UK financial institutions, with rising losses and increasing regulatory scrutiny. This project addresses the challenge of understanding how APP fraud risk is distributed across scam typologies and how this distribution has changed over time.

Multiple years of aggregated APP fraud data are consolidated and engineered to produce severity, growth and distribution metrics. Exploratory analysis reveals that financial losses are increasingly concentrated within fewer, higher-value scam types, particularly investment and impersonation-related frauds. This demonstrates that volume-based prioritisation alone is insufficient for managing APP fraud risk.

The findings provide strategic insight into how banks and regulators can better target interventions, prioritise investment, and support compliance with reimbursement obligations.

---

## Data Sources
All data used in this project is publicly available and fully anonymised.

- **Action Fraud** – National UK fraud and cybercrime statistics  
- **UK Finance** – Annual *Fraud The Facts* reports  
- **Financial Conduct Authority (FCA)** – Regulatory guidance and APP reimbursement reporting  

Data is aggregated at an annual level and includes:
- APP fraud case volumes  
- Total financial losses  
- Scam typology breakdowns  
- High-level victim segmentation  

---

## Data Infrastructure & Tools
The project uses a standard, industry-aligned data science toolchain:

- **Python** – Core analysis and data processing  
- **pandas / numpy** – Data manipulation and feature engineering  
- **matplotlib / seaborn** – Exploratory visualisation  
- **scikit-learn** – Unsupervised learning techniques  
- **Jupyter Notebook** – Reproducible and documented analysis workflow  
- **Power BI / Tableau** – Interactive dashboards (conceptual design)  
- **GitHub** – Version control and portfolio presentation  

This tooling supports transparency, reproducibility and effective communication with both technical and non-technical stakeholders.

---

## Data Engineering
An extract-transform-load (ETL) process is applied to combine multiple years of APP fraud statistics into a single analytical dataset.

Key steps include:
- Harmonising scam typology definitions across reporting years  
- Flagging structural changes where categories cannot be perfectly aligned (e.g. crypto scams)  
- Engineering analytical features such as:
  - Average loss per case  
  - Proportion of total losses by typology  
  - Year-on-year growth rates  
  - High-severity typology indicators  

Data quality checks are performed throughout, including validation against published totals, missing value analysis, and anomaly detection. All transformations are documented within the analysis notebooks.

---

## Analytical Approach
The analysis begins with descriptive statistics to establish baseline trends in APP fraud volumes and losses. The central hypothesis is that APP fraud risk is increasingly driven by loss severity rather than case volume alone.

Trend analysis is used to identify scam types with sustained growth or volatility. Where appropriate, unsupervised learning methods such as clustering are explored to group typologies based on severity, growth rate and loss concentration. Model choice is driven by interpretability and suitability for aggregated data.

The analysis explicitly avoids individual-level prediction and instead focuses on strategic, decision-relevant insights.

---

## Data Visualisation & Dashboards
Visual outputs are designed to communicate insights clearly to non-technical audiences, such as fraud leadership and policy stakeholders.

Planned visuals include:
- Time-series charts of total APP fraud losses and case volumes  
- Stacked charts illustrating shifts in scam typology composition  
- Comparative charts of average loss per case by typology  
- Optional geographic views where regional data permits  

Dashboard design follows established visualisation principles, prioritising clarity, consistency and narrative flow.

---

## Ethical, Legal & Governance Considerations
The project uses fully anonymised, aggregated data, eliminating risks associated with personal data processing. However, key limitations are acknowledged:

- Potential under-reporting of fraud incidents  
- Risk of ecological fallacy when interpreting aggregated trends  
- Inability to infer individual behaviour or causality  

Regulatory considerations are addressed through alignment with FCA guidance and APP reimbursement frameworks. Ethical implications are documented alongside analytical findings.

---

## Recommendations
Based on the analytical approach and anticipated findings, the project proposes the following strategic recommendations:

1. **Shift prioritisation from volume to severity**  
   Fraud prevention strategies should focus more heavily on scam types with high average losses rather than volume alone.

2. **Typology-specific customer interventions**  
   Warning messages and friction should be tailored to high-severity scams such as investment and impersonation fraud.

3. **Early-trend monitoring**  
   Growth-rate indicators should be used as early warning signals to inform proactive controls.

4. **Integration with internal data**  
   Future iterations could combine public data with bank-level transaction data to enable more granular risk modelling and evaluation.

---

## Future Work
Potential extensions of this project include:
- Automated data refresh pipelines  
- Integration with transaction-level datasets  
- Supervised modelling for risk scoring  
- Impact evaluation against reimbursement cost metrics  

---

## References
Action Fraud (2023). *Fraud and cyber crime statistics*.  
UK Finance (2024). *Fraud The Facts*.  
Financial Conduct Authority (2023). *APP reimbursement guidance*.  
Provost, F. & Fawcett, T. (2013). *Data Science for Business*.  
Few, S. (2012). *Show Me the Numbers*.  




<!--
**ambevans/ambevans** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:


-->
