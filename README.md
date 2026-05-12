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
## Topic: Analysis of Authorised Push Payment (APP) Fraud in the UK

---

## TL;DR
This project applies a full data science workflow to publicly available UK data on Authorised Push Payment (APP) fraud. By consolidating multiple years of aggregated fraud statistics, engineering severity‑based features, and conducting exploratory analysis, the project demonstrates that financial losses are increasingly concentrated within fewer, higher‑value scam types. The findings highlight the limitations of volume‑based prioritisation and illustrate how evidence‑led insights can support more targeted fraud‑prevention strategies, regulatory alignment, and strategic decision‑making within financial services.

---

## Executive Summary
This project investigates the evolution and impact of Authorised Push Payment (APP) fraud in the UK using publicly available datasets from Action Fraud, UK Finance and the Financial Conduct Authority (FCA). APP fraud presents a significant and growing challenge to the UK financial system, with increasing volumes, rising losses, and escalating regulatory expectations following the introduction of mandatory reimbursement requirements. The central data science challenge addressed in this project is to understand how APP fraud typologies are changing over time, which scam categories pose the greatest financial risk, and how evidence‑led insights can support more targeted fraud‑prevention strategies within financial institutions.

The project applies an end‑to‑end data science workflow, incorporating data sourcing, data engineering, exploratory and analytical techniques, and data visualisation. Multiple years of aggregated APP fraud statistics are consolidated into a single analytical dataset, with engineered features such as average loss per case, typology‑level loss concentration and year‑on‑year growth indicators. Exploratory analysis is used to quantify how losses are shifting towards fewer but higher‑value cases, particularly within investment and impersonation‑based scams.

The findings demonstrate that APP fraud risk is not evenly distributed across scam types. Certain typologies generate disproportionately high losses despite relatively lower case volumes, highlighting the limitations of volume‑based prioritisation approaches. These insights have direct business relevance for banks, enabling more effective allocation of fraud‑prevention investment, refinement of customer warning journeys, and improved compliance with regulatory expectations.

From an impact perspective, the project illustrates how aggregated external data can be transformed into decision‑useful intelligence. While the dataset does not allow individual‑level prediction, the analysis supports strategic prioritisation, cost‑benefit decision‑making and stakeholder engagement across fraud, product and compliance teams. Future iterations outline how similar methods could be integrated with internal transaction‑level data to deliver greater operational impact.

---

## Data Infrastructure & Tools
The project uses a modern, lightweight data science toolchain designed to support transparency, reproducibility and effective communication. Python is the core programming language, selected for its extensive data science ecosystem and strong support for data manipulation, statistical analysis and visualisation. Key libraries include **pandas**, **numpy**, **matplotlib**, **seaborn** and **scikit‑learn**.

Jupyter Notebook is used as the primary analytical environment. This enables a clear, documented workflow in which code, outputs and explanatory commentary are integrated, supporting auditability and alignment with best practice in applied data science. All assumptions, transformations and analytical decisions are recorded alongside outputs, which is particularly important in a regulatory‑adjacent domain such as fraud analytics.

For data communication, the project leverages Power BI (or Tableau) to design interactive dashboards. These tools are well‑suited to executive and stakeholder audiences, allowing users to explore trends over time, compare scam typologies, and understand changes in loss severity through intuitive visuals. Although dashboards are conceptual in early stages of the project, their structure has been deliberately designed to reflect real‑world fraud monitoring use cases within financial services.

GitHub is used for version control and project management, hosting datasets, notebooks, documentation and visual artefacts. This supports reproducibility, collaborative working, and alignment with industry practice for data science portfolio development.

---

## Data Engineering
The data engineering phase focuses on transforming fragmented public APP fraud statistics into a consistent and analysis‑ready dataset. Source data is published annually by multiple bodies, with variations in schema definitions, typology classifications and reporting granularity across years. An extract‑transform‑load (ETL) process is therefore applied to ensure temporal consistency and analytical validity.

During extraction, raw datasets are imported into Python and standardised to a common schema. Transformation steps include harmonising scam typology names, resolving category changes across reporting periods, and explicitly flagging typologies introduced part‑way through the time series (for example, crypto‑related scams). Where harmonisation is not possible, structural breaks are documented rather than imputed, preserving analytical integrity.

Feature engineering plays a central role in enabling meaningful analysis. Derived features include average loss per case, proportion of total losses attributable to each scam type, year‑on‑year growth rates, and categorical indicators of high‑severity typologies. Temporal features are added to support trend analysis and comparative evaluation across periods.

Data quality checks are embedded throughout the process, including validation of totals against published control figures, assessment of missing values, detection of duplicated records and review of extreme values. Any anomalies are documented within the analysis notebooks to ensure transparency.

Although the dataset is aggregated and does not require train‑test splitting or scaling, the engineering decisions are explicitly linked to downstream analytical objectives. This ensures that the data preparation stage directly supports robust analysis, visualisation and interpretation, consistent with established data engineering principles.

---

## Data Visualisation & Dashboards
Data visualisation is used as the primary mechanism for translating analytical findings into business‑relevant insights. The project employs trend charts to illustrate changes in total APP fraud losses and case volumes over time, highlighting divergence between volume growth and financial impact. Stacked bar and area charts are used to show how the composition of fraud losses has shifted across scam typologies, enabling rapid identification of emerging risks.

Comparative visuals, such as bar charts of average loss per case by typology, support prioritisation discussions by illustrating severity rather than frequency alone. Where available, geographic visualisation (for example, regional heatmaps) is proposed to support targeted intervention strategies.

Dashboard designs follow core data visualisation principles, including minimal cognitive load, consistent colour usage and clear annotation. Visuals are explicitly designed for a non‑technical audience, ensuring alignment between analytical outputs and decision‑making needs.

---

## Data Analytics
The analytical approach begins with descriptive and exploratory analysis to establish baseline patterns in APP fraud volumes, losses and typology distribution. The primary hypothesis is that APP fraud risk is increasingly concentrated in fewer, higher‑value scams rather than driven solely by growth in case volumes. This is tested through comparative analysis of average loss per case and typology‑level loss shares across time.

Trend analysis is used to identify scam categories exhibiting sustained growth or volatility. Where appropriate, unsupervised learning techniques such as clustering are explored to group scam typologies based on severity, growth and loss concentration. Model selection is justified based on data structure and interpretability, with clear explanation of limitations.

Given the aggregated nature of the dataset, the analysis explicitly avoids claims of individual‑level prediction or causality. Instead, outputs are positioned as strategic insights suitable for policy design, prioritisation and control optimisation. Evaluation focuses on interpretability and business relevance rather than predictive accuracy metrics.

Ethical considerations are central to the project. The data is fully anonymised and publicly released, eliminating privacy risks associated with personal data. However, aggregation introduces the risk of ecological fallacy, which is acknowledged in both analysis and conclusions. Bias arising from under‑reporting of fraud is also discussed, alongside the implications this has for interpreting trends.

Regulatory and legal considerations are addressed by aligning insights with FCA guidance and reimbursement obligations, ensuring that analytical recommendations are framed within a compliant and responsible governance context.

---

## Recommendations
The analysis indicates that APP fraud prevention strategies should move beyond volume‑based prioritisation and place greater emphasis on loss severity. Scam typologies with lower case volumes but significantly higher average losses, such as investment and impersonation scams, represent a disproportionate share of financial harm.

The findings also suggest a need for typology‑specific customer interventions. Tailoring messaging, friction and educational prompts to the behavioural characteristics of high‑severity scams could improve customer comprehension and reduce susceptibility at key decision points within the payment journey.

In addition, the use of growth‑rate metrics as early‑trend indicators is recommended. Monitoring sustained increases in loss severity or typology‑level growth could allow banks and regulators to introduce preventative controls earlier, rather than reacting once losses have materialised. Future iterations of this work should seek to integrate public APP fraud data with internal transaction‑level datasets to enable more granular modelling and improved impact measurement.

---

## References
- Action Fraud (2023). *Fraud and cyber crime statistics*  
- UK Finance (2024). *Fraud The Facts*  
- Financial Conduct Authority (2023). *APP reimbursement guidance*  
- Provost, F. and Fawcett, T. (2013). *Data Science for Business*  
- Few, S. (2012). *Show Me the Numbers*
``
