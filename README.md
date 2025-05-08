# Evaluating Twitter’s Deplatforming Policy on Misinformation (Replication Study)

This project replicates and extends the findings from the 2024 study, [**"Post-January 6th deplatforming reduced the reach of misinformation on Twitter"**](https://www.nature.com/articles/s41586-024-07524-8) by McCabe et al., published in *Nature*.  
Using the original dataset and Difference-in-Differences (DiD) methodology, this analysis investigates the causal impact of Twitter’s deplatforming intervention on misinformation sharing, user behavior, and content landscape.

## Overview

Following the January 6th Capitol riots, Twitter suspended major accounts, including then-President Donald Trump and high-profile misinformation spreaders. This study explores whether this action effectively reduced misinformation on the platform and reshaped user behavior.

The project replicates the main DiD analysis of McCabe et al. and further explores subgroup impacts (e.g., QAnon and Trump followers), robustness (parallel trends), and behavioral changes across the Twitter user base.

## Data

- **Original dataset provided by McCabe et al. (2024)**  
  - 1.5 million Twitter users (Dec 2020 — Jan 2021)
  - User activity logs (retweets, URLs shared)
  - Flags for misinformation sharers and suspended accounts

## Methodology

### 1️⃣ Difference-in-Differences (DiD) Analysis
- Treatment group: Followers of deplatformed users
- Control group: Non-followers
- Pre, Intervention, and Post-treatment periods defined
- Modeled misinformation retweet counts using DiD to estimate causal impact

### 2️⃣ Subgroup Analysis
- Examined QAnon and Trump followers separately
- Focused on high-activity users to test heterogeneous treatment effects

### 3️⃣ Robustness Checks
- Tested the parallel trends assumption
- Extended post-treatment window to validate robustness of results

## Key Findings

- **Significant reduction in misinformation** among both suspended users and their followers after the deplatforming.
- **64% drop** in misinformation retweets from followers of suspended users, compared to a 55% decline among non-followers.
- **QAnon and high-activity users** showed particularly sharp declines in misinformation sharing.
- Results suggest deplatforming not only curbed misinformation at its source but also influenced broader user behavior.

## Policy Implications

- **Content moderation interventions can be effective** in reducing misinformation and reshaping online discourse.
- Deplatforming, while effective, may also drive migration to alternative platforms → broader ecosystem monitoring is needed.
- Replication and transparency in research help validate policy effectiveness and support evidence-based decision making.

## Files

- `Twitter_misinfo_project.ipynb`: Main analysis notebook (Replication, DiD model, subgroup and robustness analyses)
- `mccabe-public-data.csv`: Original dataset
- `codebook`: codebook for the dataset

## Related Work

Please also check out my Medium post where I summarize this project and discuss its policy relevance in more detail.  
[Medium Post](https://medium.com/@sangmin.lee.ir/evaluating-the-effectiveness-of-twitters-deplatforming-as-a-content-moderation-strategy-1066dea05a46)

## License

This project is for educational and research purposes only.
