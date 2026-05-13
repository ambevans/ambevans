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

## PART 1 — DATA SCIENCE PROJECT

---

## Executive Summary, Documentation, Project Report & Impact Evaluation

This project investigates the evolution and impact of Authorised Push Payment (APP) fraud in the UK using publicly available datasets from Action Fraud, UK Finance and the Financial Conduct Authority (FCA). APP fraud represents a rapidly evolving and systemically significant form of financial crime that has prompted a major regulatory response, including the introduction of mandatory reimbursement requirements. These developments reflect growing recognition that APP fraud poses material risks to consumer protection and financial stability rather than being an isolated operational issue (Braithwaite, 2024).

The central business challenge addressed is how financial institutions can prioritise fraud‑prevention effort more effectively in a context where reimbursement obligations increase the cost of inaction. The project tests the hypothesis that APP fraud harm is increasingly driven by loss severity within specific scam typologies rather than by overall growth in case volumes. From a data science perspective, the objective is to determine how aggregated external data can be transformed into insights that support smarter prioritisation and earlier intervention.

An end‑to‑end data science workflow is applied, focused on exploratory, comparative and descriptive analysis rather than individual‑level prediction. This aligns with established data science principles, which emphasise that analytical value is realised when insights directly support strategic decision‑making (Provost and Fawcett, 2013). Multiple years of aggregated APP fraud statistics are consolidated into a single analysis‑ready dataset, with engineered features including average loss per case, typology‑level loss concentration and year‑on‑year growth indicators.

The analysis shows that APP fraud risk is not evenly distributed: a small number of scam types generate disproportionately high financial harm despite relatively lower volumes. This exposes the limitations of volume‑based prioritisation commonly used in operational reporting. From a business perspective, these insights support severity‑based prioritisation that can reduce financial losses, improve reimbursement outcomes and inform earlier regulatory intervention. The project concludes by outlining how similar methods could be extended using internal transaction‑level data to measure and increase operational impact.

---

## Data Infrastructure & Tools

The project uses a lightweight data science toolchain designed to support transparency, reproducibility and effective communication. Python is selected as the core programming language due to its strong support for data manipulation, aggregation and exploratory analysis. Core libraries include `pandas` and `numpy` for structured data processing and feature engineering, alongside `matplotlib` and `seaborn` for exploring trends, distributions and typology‑level comparisons. These tools are well‑suited to working with aggregated public data and enable rapid iteration during exploratory analysis.

Jupyter Notebook is used as the primary analytical environment, allowing code, outputs and explanatory commentary to be documented side by side. This supports auditability and reproducibility by ensuring that assumptions, transformations and analytical decisions are visible and reviewable. Such transparency is particularly important in regulatory‑adjacent domains such as financial crime analytics, where analytical reasoning must be explainable and defensible.

For insight communication, the project leverages business intelligence tools such as Power BI (or Tableau) to design interactive dashboards. These tools are selected for their effectiveness in conveying analytical insights to non‑technical stakeholders, enabling exploration of trends over time, comparison of scam typologies and assessment of loss severity. Dashboard design follows established visual communication principles that prioritise clarity and decision support (Few, 2012).

The supporting infrastructure is intentionally lightweight and file‑based, reflecting the constraints of working with externally published datasets rather than live internal transaction feeds. In a production environment, similar analyses could be supported by automated pipelines and governed analytics platforms; however, such infrastructure is neither required nor appropriate for the exploratory and strategic aims of this project. GitHub is used for version control and documentation, supporting reproducibility and alignment with professional data science practice.

---

## Data Engineering

The data engineering phase focuses on transforming fragmented public APP fraud statistics into a consistent and analysis‑ready dataset. Source data is published annually by multiple organisations, with variation in schema design, typology classification and reporting granularity. An extract‑transform‑load (ETL) approach is therefore applied to ensure temporal consistency and analytical validity.

During extraction, raw datasets are imported into Python and standardised to a common schema. Transformation steps include harmonising scam typology names, resolving category changes across reporting periods and explicitly flagging typologies introduced part‑way through the time series. Where harmonisation is not possible, structural breaks are documented rather than imputed to preserve analytical integrity and avoid misleading trend analysis.

Feature engineering is used to support the project’s core analytical questions. Derived features include average loss per case, typology‑level contribution to total losses, year‑on‑year growth rates and categorical indicators of high‑severity scam types. Temporal fields are added to support trend identification and comparison across periods.

Data quality checks are embedded throughout the process, including validation of totals against published control figures, checks for missing values and review of extreme values. Any anomalies are documented within the analysis notebooks to maintain transparency. As the dataset is fully aggregated and population‑level, standard practices such as train‑test splits, scaling or normalisation are neither methodologically valid nor analytically meaningful in this context. Engineering decisions are therefore explicitly aligned to downstream exploratory and comparative analysis rather than predictive modelling.

---

## Data Visualisation & Dashboards

Data visualisation is the primary mechanism for translating analytical findings into business‑relevant insights. Trend charts illustrate changes in total APP fraud losses and case volumes over time, highlighting divergence between incident frequency and financial impact. This allows stakeholders to observe that rising harm is driven by severity rather than volume alone.

Stacked bar and area charts show how the composition of fraud losses has shifted across scam typologies, enabling rapid identification of high‑impact categories. Comparative visuals, such as average loss per case by typology, reinforce prioritisation discussions by focusing attention on financial harm rather than reported incidents.

Visuals are designed not as descriptive outputs but as decision‑support artefacts, enabling stakeholders to distinguish high‑volume scams from high‑impact scams at a glance. Designs prioritise accessibility for non‑technical audiences, using consistent colour, clear annotation and minimal cognitive load to support interpretation. Together, the visual and written elements form a coherent analytical narrative that links trends, drivers and implications for decision‑making.

---

## Data Analytics, Ethics & Governance

The analytical approach begins with descriptive and exploratory analysis to establish baseline patterns in APP fraud volumes, losses and typology distribution, consistent with the principles of exploratory data analysis (Tukey, 1977). The primary hypothesis is that APP fraud harm is increasingly concentrated within fewer, higher‑value scam types rather than being driven solely by case growth.

Comparative analysis of average loss per case and typology‑level loss shares supports this hypothesis, showing that certain scams generate disproportionate financial harm. Trend analysis is used to identify scam categories exhibiting sustained growth or volatility, enabling early‑warning insight. Where appropriate, unsupervised techniques such as clustering are explored to group scam types based on shared characteristics of severity and growth.

Exploratory and comparative approaches are particularly suitable for fraud analysis, as losses are typically skewed and dominated by extreme values. Effective fraud analytics therefore prioritise interpretability and robustness over predictive accuracy, particularly where outputs inform strategic rather than operational decisions (Bolton and Hand, 2002). While predictive modelling could be applied where individual‑level data is available, an exploratory analytical approach is more appropriate here given the aggregated structure of the data and the strategic nature of the research questions.

Ethical considerations are central to the project. The data is publicly released and anonymised, minimising privacy risk. However, aggregation introduces risk of ecological fallacy and masking of sub‑population effects, which is acknowledged. Bias arising from under‑reporting of fraud is also considered when interpreting trends. Regulatory framing aligns insights with FCA reimbursement obligations and established principles for responsible analytics, emphasising transparency, proportionality and consumer protection (UK Finance, 2020).

---

## Recommendations

Based on the findings, APP fraud prevention strategies should move beyond volume‑based prioritisation and place greater emphasis on loss severity. Scam typologies with lower reported volumes but high average losses represent a disproportionate share of financial harm. Aligning controls, monitoring thresholds and reimbursement strategies with severity‑based indicators would enable more effective use of fraud‑prevention investment and reduce downstream reimbursement costs.

The analysis also supports development of typology‑specific customer interventions. Generic fraud warnings are unlikely to be equally effective across all scam types. Tailoring messaging and friction to the behavioural characteristics of high‑severity scams, such as impersonation or investment fraud, could improve customer comprehension and reduce susceptibility at critical decision points.

From a data science perspective, severity‑weighted growth metrics should be adopted as early‑warning indicators. Monitoring increases in average loss per case or typology‑level loss concentration would allow institutions to act proactively rather than reacting once total losses escalate. This is particularly relevant in a regulatory environment where earlier intervention reduces both consumer harm and reimbursement exposure.

Future iterations of this work should integrate aggregated external fraud statistics with internal transaction‑level and behavioural data. While the current project is necessarily strategic, combining these data sources would enable more granular modelling, clearer evaluation of intervention effectiveness and stronger measurement of business value.

---

## References

- Action Fraud (2023). *Fraud and cyber crime statistics*  
- Bolton, R.J. and Hand, D.J. (2002). *Statistical fraud detection: A review*  
- Braithwaite, J. (2024). *Authorised push payment fraud and regulatory response*  
- Few, S. (2012). *Show Me the Numbers*  
- Provost, F. and Fawcett, T. (2013). *Data Science for Business*  
- Tukey, J.W. (1977). *Exploratory Data Analysis*  
- UK Finance (2020). *Ethical principles for advanced analytics and AI*

---
