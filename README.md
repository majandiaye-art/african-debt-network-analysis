# The Evolution of Africa's Bilateral Debt Network (2014–2024)

**Network Analysis · International Finance · R**

**Overview**

This project examines the structure and evolution of bilateral public and publicly guaranteed (PPG) external debt relationships between African countries and their creditors from 2014 to 2024. Inspired by Bhattacharya, Inekwe and Valenzuela (2018), it applies network analysis to a different financial instrument outstanding bilateral sovereign debt to explore connectivity, creditor concentration, and structural dependence.

The analysis models creditors and African borrowers as nodes in a **directed, weighted network**. A link runs from a creditor to a debtor, with its weight representing the outstanding bilateral debt stock.

 **Data and method**

The main data source is the **World Bank International Debt Statistics** (indicator `DT.DOD.BLAT.CD`), complemented by World Bank macroeconomic indicators and the **Boston University Chinese Loans to Africa** database. The observed dataset includes **50 African debtor countries**, **38 creditors**, and **4,897 positive creditor–debtor–year links**.

Methods include degree and strength centrality, the Herfindahl–Hirschman Index (HHI) for creditor concentration, weighted Louvain community detection, Ward hierarchical clustering of creditor-share profiles, pooled country/year OLS regressions, and hypothetical creditor-removal exercises.

**Selected finding**

- **Debt exposure changed more than connectivity:** observed bilateral debt stock rose from **USD 92.33 billion in 2014** to **USD 137.38 billion in 2024**, while the annual number of positive links remained relatively stable.
- **Intra-African exposure remained limited:** the share owed to African creditors fell from **6.2%** to **2.3%** over the period.
- **China was the largest observed bilateral creditor:** its average annual outstanding exposure was **USD 55.97 billion**, and it was connected to **46 African debtors in 2024**.
- **Creditor concentration increased:** mean debtor-level HHI rose from **0.363** in 2014 to **0.415** in 2024. Having several creditors does not necessarily imply a well-diversified debt portfolio.
- **Debt and creditor connectivity were positively associated:** the baseline pooled regression estimated a coefficient of **0.1485** for log bilateral debt in a model of log(1 + number of creditors), controlling for year effects. This is an association, not a causal estimate.
- **Chinese lending commitments slowed:** annual new commitments fell substantially from their 2016 peak, even as China remained prominent in *outstanding debt stocks*. Commitments (flows) and debt stocks are distinct measures.



The repository contains the full research report and supporting R analysis. **Read the full report for figures, detailed methodology, regression tables, references, and limitations.**

 **Scope and limitations**

The network covers **reported bilateral PPG external debt**, not all African public or external debt. It excludes multilateral and private liabilities. Missing observations are not treated as zero. The creditor-removal exercise measures structural exposure; it does not simulate defaults or financial contagion.

## Reference

Bhattacharya, M., Inekwe, J. N., & Valenzuela, M. R. (2018). *Financial integration in Africa: New evidence using network approach*. **Economic Modelling, 72**, 379–390. https://doi.org/10.1016/j.econmod.2018.02.013

**Author:** Mame Bousso Ndiaye
