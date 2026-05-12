## Hi there 👋

- 🔭 I’m currently working on shaping and delivering core money‑management journeys across Upcoming Payments, Subscriptions, and Payday. My focus is on setting clear product direction, prioritising the right customer problems, and ensuring these experiences genuinely help customers feel in control of their money. I work closely with product, engineering, design, and analytics teams to turn insight into outcome, balancing customer needs, commercial impact, and regulatory expectations.

- 🌱 I’m currently learning how to deepen my impact as a leader through advanced data science and analytics, strengthening my ability to use evidence to influence decisions, set strategy, and measure success at scale. Alongside this, I’m continuing to build my capability in Python, Power BI, and analytics storytelling to support more confident, insight‑led leadership conversations.

- 👯 I’m looking to collaborate on complex, cross‑journey problems where clear ownership, strong alignment, and customer‑first thinking are essential — particularly initiatives that span payments, subscriptions, and financial wellbeing. I enjoy partnering with others to define strategy, challenge assumptions, and land change that makes a real difference for customers.

- 🤔 I’m looking for help with evolving how teams use insight to drive prioritisation, improving how we connect customer feedback to strategic roadmaps, and exploring better ways to test, learn, and scale what works across digital journeys.

- 💬 Ask me about leading customer‑centric product strategy, Upcoming Payments and Subscriptions journeys, payday experiences, turning customer insight into executive‑ready recommendations, or using data to support decision‑making and influence at senior levels.

- 📫 How to reach me: www.linkedin.com/in/amber-evans-363035177

- 😄 Pronouns: she/her

- ⚡ Fun fact: Outside work, I’m usually balancing running, Pilates or tennis with cooking something new — and planning my next travel adventure.





# PART 1 — DATA SCIENCE PROJECT
Analysis of Authorised Push Payment (APP) Fraud in the UK

---

## Executive Summary
This project investigates Authorised Push Payment (APP) fraud using publicly available UK datasets sourced from Action Fraud, UK Finance and Financial Conduct Authority (FCA) open‑data releases. The data reports aggregated APP fraud case volumes, financial losses, typology splits and limited victim segmentation. The aim of the project is to apply an end‑to‑end data science workflow to understand how APP fraud has evolved over time, which scam typologies pose the highest financial risk, and how analytical insights could inform more effective fraud‑prevention strategies within the banking sector.

The project consolidates multiple years of APP fraud data, applies feature engineering to quantify loss severity and growth trends, and conducts exploratory analysis across scam typologies. The findings highlight that financial losses are increasingly concentrated within fewer, higher‑value scams, rather than being evenly distributed across case volumes. This demonstrates the need to prioritise fraud prevention based on severity as well as frequency.

The outputs of the project are intended to support strategic decision‑making, regulatory alignment and targeted intervention design, rather than individual‑level fraud prediction.

---

## Data Infrastructure & Tools
Python is used as the primary analytical tool for data ingestion, transformation and analysis. Its data science ecosystem enables efficient manipulation of structured data and supports transparent feature engineering and exploratory analysis. Jupyter Notebook provides a reproducible environment in which code, outputs and explanatory commentary are combined, allowing assumptions and decisions to be clearly documented.

Power BI or Tableau is used for the conceptual design of dashboards that communicate key findings to non‑technical stakeholders. These tools are suitable for executive‑level audiences and allow long‑term fraud trends and typology‑level differences to be explored interactively.

GitHub is used to version‑control the project and to host analysis notebooks, data extracts and visual artefacts. This reflects standard industry practice and supports reproducibility, transparency and portfolio presentation.

---

## Data Engineering
The data engineering process follows an extract‑transform‑load (ETL) approach. Multiple annual APP fraud datasets are combined into a single analytical dataset. Because scam typology classifications differ across reporting years, typologies are harmonised where possible, with structural changes explicitly documented rather than imputed. For example, early reporting periods do not separately classify crypto‑related scams, which is flagged during transformation.

Several analytical features are engineered to support downstream analysis. These include total losses, total case volumes, average loss per case, typology‑level loss distributions, year‑on‑year growth metrics and categorical indicators of higher‑severity scams. Time‑based variables are introduced to enable trend analysis across reporting periods.

Data quality checks are conducted throughout, including validation against published totals, assessment of missing values, duplicate detection and review of anomalous values. Any limitations or anomalies are documented within the analysis notebooks.

---

## Data Visualisation & Dashboards
Visualisations are designed to illustrate how APP fraud has evolved over time and how financial harm differs across scam typologies. Planned outputs include trend charts showing total losses and case volumes, stacked charts illustrating typology composition across years, and comparative visuals highlighting differences in average loss per case.

Dashboard designs emphasise clarity, logical sequencing and alignment between written and visual findings. The intention is to support clear communication of insights to stakeholders such as fraud leaders, regulators and policy teams.

---

## Data Analytics
The analysis begins with descriptive statistics to establish baseline patterns in APP fraud volumes and losses. Comparisons are made across scam categories such as investment scams, impersonation scams, purchase scams and crypto‑related fraud where available. Longer‑term trends are examined to identify typologies exhibiting sustained growth, volatility or increasing loss severity.

Where appropriate, unsupervised analytical techniques may be applied to group scam typologies based on severity and growth characteristics. Any modelling choices are justified based on data structure and interpretability, with limitations clearly acknowledged.

Ethical considerations form part of the analytical discussion. The dataset is fully anonymised and aggregated, which reduces privacy risk but limits behavioural inference. The analysis avoids individual‑level prediction and acknowledges potential bias arising from under‑reporting of fraud incidents.

---

## Recommendations
The analysis indicates that APP fraud prevention strategies should prioritise loss severity in addition to case volume. Scam typologies with fewer incidents but significantly higher average losses contribute disproportionately to overall harm and warrant targeted intervention.

The findings support the use of typology‑specific customer warnings and preventative controls, particularly for high‑severity scams such as investment and impersonation fraud. Monitoring growth‑rate indicators is also recommended as an early‑warning mechanism to inform proactive control design.

Future iterations of the project could integrate public fraud data with internal transaction‑level datasets to enable more granular modelling and stronger measurement of intervention effectiveness.

---

## References
Action Fraud (2023). *Fraud and cyber crime statistics*.  
UK Finance (2024). *Fraud The Facts*.  
Financial Conduct Authority (2023). *APP reimbursement guidance*.  
Provost, F. and Fawcett, T. (2013). *Data Science for Business*.  
Few, S. (2012). *Show Me the Numbers*.  
