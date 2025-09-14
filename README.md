# Marketing Mix Model
Scalable Bayesian MMM using Google's LightweightMMM framework in Python to measure media effectiveness &amp; optimize marketing ROI. Built on AMASS-simulated realistic marketing data, delivering interpretable insights for strategic budget allocation decisions across channels.

# Executive Summary

### **Optimization Results: 6.3% Brand Sales Improvement Through Strategic Budget Reallocation**

The media mix optimization analysis reveals a meaningful opportunity to improve performance by reallocating budget across channels. The model simulation predicts a 6.28% increase in target variable through strategic budget reallocation. 
### Key Budget Reallocation Recommendations

#### Increase Investment:
* TV: +2% budget increase (maintaining dominance as top performer)
* Direct Mail: +1% budget boost to capitalize on proven mid-tier performance

#### Decrease Investment:

* Online Video: -3% reduction (17% → 14%) despite strong historical performance
* Social Media: -2% reduction, suggesting saturation at current spend levels
* Digital Out of Home & Billboard: Minor adjustments reflecting optimization at the margins


## Business Impact
This is expected to result in 1,496,524 more brand sales over two years, from 22,358,139 to 23,854,663.

The 6.3% performance lift represents meaningful incremental value with minimal risk, as all changes stay within ±20% bounds of historical spending patterns. This conservative optimization approach ensures implementable recommendations while capturing measurable improvement opportunities across the media portfolio.

<img width="2984" height="984" alt="MMM-Optimal-Budget-Simulation" src="https://github.com/user-attachments/assets/7b72d2c6-f5d9-4d31-ad49-71039d743477" />
<img width="2421" height="885" alt="Unknown" src="https://github.com/user-attachments/assets/3c6c95e0-a19b-4b0f-9c68-51521cfe59a6" />


## Project Overview

Marketing Mix Modeling (MMM) has become an essential tool for understanding the incremental impact of marketing channels on business outcomes, enabling data-driven budget allocation and strategic decision-making. For this analysis, I implemented a Bayesian MMM approach using Google's LightweightMMM framework [1], leveraging the comprehensive API documentation provided in the repository [2]. The model provides a scalable and interpretable solution for measuring media effectiveness and optimizing marketing investments. 

This analysis represents a foundational implementation of Google's LightweightMMM framework using simulated data. While the underlying Bayesian approach remains robust, readers should note that this model reflects techniques and data structures from 2022 and serves as a methodological reference point.. For production implementations, consider utilizing Google's Meridian model. 

**Dataset Details:**

This model utilizes a dataset generated with the Aggregate Marketing System Simulator (AMASS), an open-source R package provided by Google for research purposes [3]. The AMASS tool simulates realistic marketing datasets. The source code for the AMASS package was obtained from the Google GitHub repository.

*   Initial Data: AMASS generated 228 rows of weekly data, representing 4 years.
Normalization Period: The first 104 rows were removed to allow the simulator time to normalize.
*   Final Dataset: The resulting dataset contains 104 rows, representing 2 years of weekly data.

This final dataset captures a balanced media budget allocation across traditional media, social media, search engine marketing (SEM), programmatic display advertising, direct mail, digital out-of-home (DOOH), and billboards.

**Media Variables Used:**

The dataset includes the following media variables:

*   dsp_tv
*   dsp_search
*   dsp_programmatic
*   dsp_social
*   dsp_ctv
*   dsp_directmail
*   dsp_dooh
*   dsp_billboard

**Holiday Variables Used:**

Merge weekly records with Canadian national holidays across the 52 weeks of the year. The holidays included are:

* New Year's Day (Week 1)
* Family Day (Week 7)
* Good Friday (Week 14)
* Victoria Day (Week 20)
* Canada Day (Week 26)
* Civic Holiday (Week 31)
* Labour Day (Week 36)
* Thanksgiving (Week 40)
* Remembrance Day (Week 45)
* Christmas Day (Week 51)
* Boxing Day (Week 51)

**References**

[1] Duque, P., Nachbar, D., Abe, Y., Ahlheim, C., Anderson, M., Sun, Y., Goldstein, O. and Eck, T. (2022) LightweightMMM: Lightweight (Bayesian) Marketing Mix Modeling. https://github.com/google/lightweight_mmm

[2] Duque, P., Nachbar, D., Abe, Y., Ahlheim, C., Anderson, M., Sun, Y., Goldstein, O. and Eck, T. (2022) LightweightMMM Models API Documentation. https://lightweight-mmm.readthedocs.io/en/latest/api.html

[3] Zhang, S. and Vaver, J. (2017) Introduction to the Aggregate Marketing System Simulator. https://research.google/pubs/introduction-to-the-aggregate-marketing-system-simulator/



