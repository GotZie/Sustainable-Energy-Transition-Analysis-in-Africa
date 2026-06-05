# Sustainable Energy Transition Analysis in Africa (2000–2019)

## Overview

This project investigates the state of sustainable energy transition across African countries between 2000 and 2019 using a multi-dimensional data analysis approach. The analysis explores the relationships between energy access, renewable energy adoption, economic development, CO₂ emissions, and international financial assistance across African countries between 2000 and 2020.  
The project combines exploratory data analysis, comparative visualizations, trend analysis, and correlation-based evaluations to uncover structural patterns influencing Africa’s transition toward sustainable and low-carbon energy systems.



## Problem Statement

Africa faces a complex energy transition challenge. While many countries possess large renewable energy resources, the continent still experiences:

* limited electricity access,
* low clean cooking fuel adoption,
* high dependence on traditional biomass,
* uneven industrial development,
* fossil-fuel-driven emissions in industrialized regions,
* and heavy reliance on foreign financial assistance for infrastructure expansion.

The **objective** of this project is to evaluate:

* how energy development differs across African regions,
* whether renewable energy adoption translates into broader sustainability outcomes,
* the relationship between economic growth and emissions,
* and whether foreign financial assistance meaningfully supports renewable energy transition.


#### Key Challenges

Several structural and analytical challenges emerged throughout the project:

* Missing values across multiple sustainability indicators
* Strong regional inequalities in development and infrastructure
* Presence of major outliers (e.g., South Africa)
* Interpreting renewable energy shares correctly, especially where traditional biomass dominates


## Dataset Summary

The dataset contains African country-level sustainability indicators spanning 2000–2020.

*Dataset Name:* Global Data on Sustainable Energy (2000-2020)  

*Domain:* Semiconductor Manufacturing

*Dataset Source:*
[Global Data on Sustainable Energy](https://www.kaggle.com/datasets/anshtanwar/global-data-on-sustainable-energy)  

*Scope*: 50 African countries · 2000–2019    

*Number of Features:* 21

### Major Variables

| Category               | Variables                                                                 |
| ---------------------- | ------------------------------------------------------------------------- |
| Energy Access          | `elec_access_pct`, `clean_fuels_pct`                                      |
| Renewable Energy       | `renew_share_pct`, `renew_cap_per_capita_W`, `low_carbon_elec_pct`        |
| Electricity Generation | `elec_fossil_TWh`, `elec_renew_TWh`, `elec_nuclear_TWh`, `elec_total_TWh` |
| Economic Indicators    | `gdp_per_capita_usd`, `financial_flows_bn_usd`                            |
| Emissions              | `co2_Mt`                                                                  |
| Energy Consumption     | `primary_energy_kWh_per_capita`, `energy_intensity_MJ_per_USD`            |
| Geographic Variables   | `sub_region`, `latitude`, `longitude`                                     |

### Geographic Coverage

 African countries only Grouped into:

  * North Africa
  * West Africa
  * East Africa
  * Central Africa
  * Southern Africa


## Repository Structure

```bash
├── data/
│   ├── raw/   # unprocessed dataset
│   ├── processed/ # clean dataset
│
├── notebooks/
│   ├── Global Data on Sustainable Energy.ipynb
│
├── visuals/ # folder containing all analytical visualisations
│   ├── comparative_analysis/
│   ├── economic_analysis/
│   ├── electricity_mix/
│   ├── energy_access/
│   ├── renewable_transition/
│
├── README.md
│
├── requirements.txt
│
└── LICENSE
```


## Approach

The analysis was conducted in multiple stages:

#### 1. Data Cleaning & Preparation

* Handling missing values
* Feature standardization
* Regional grouping
* Unit conversions
* Weighted regional calculations


#### 2. Exploratory Data Analysis

Evaluation of:

* Missingness Analysis
* Structured Data Imputation

#### 3. Statistical Analysis

Applied:

* Pearson correlation analysis
* Trend analysis
* Comparative regional analysis
* Growth comparisons
* Weighted electricity mix analysis


#### 4. Visualization

Generated:

* Scatter plots
* Bubble charts
* Heatmaps
* Line charts
* Stacked area charts
* Comparative bar charts


## Key Assumptions

The project assumes that:

* Renewable electricity share reflects national electricity generation structure
* Financial assistance contributes to sustainable energy development
* Regional averages reasonably represent sub-regional energy patterns
* CO₂ emissions partially reflect fossil-fuel dependence
* Weighted electricity generation provides more realistic regional grid composition analysis


## Key Findings & Observations

#### 1. Renewable Energy Share Does Not Always Mean Energy Modernization

Many African countries exhibit high renewable energy shares because of:

* hydropower dominance,
* traditional biomass use,
* and low industrialization levels.

High renewable share did not necessarily imply:

* high electricity access,
* clean cooking adoption,
* or advanced infrastructure.


#### 2. Major Regional Inequalities Exist

 **North Africa**

* Highest electricity access
* Highest clean cooking fuel adoption
* More industrialized
* Higher fossil-fuel dependence
* Higher CO₂ emissions

 **East Africa**

* Strong renewable electricity mix
* Low emissions
* Weak clean cooking fuel progress

 **Southern Africa**

* Highest industrial emissions
* Coal-dependent electricity systems

 **West & Central Africa**

* Low household energy modernization
* High reliance on biomass
* Limited infrastructure growth


#### 3. Other Observations

* Economic Growth Moderately Increases Emissions which indicates that industrial structure and electricity generation mix matter more than economic growth alone.

* Energy Intensity Alone Does Not Explain Emissions. This therefore suggests that Africa’s emissions problem is more strongly linked to fossil electricity generation than to energy inefficiency alone.

* Clean Cooking Remains a Major Development Gap Despite improvements in electricity systems: East and West Africa showed minimal progress in clean cooking fuel access. This reveals that Clean electricity growth does not automatically mean improved clean household cooking fuel access.

* Foreign Financial Assistance Shows Weak Structural Influence which suggests that funding alone does not guarantee successful renewable transition outcomes.


## Key Figures

The project includes:

* CO₂ Emissions vs Economic Development
* CO₂ Emissions vs Energy Intensity
* Foreign Financial Assistance vs Renewable Energy Adoption
* Regional Sustainability Heatmap
* Weighted Low-Carbon Electricity Trends
* Clean Cooking Fuel Access Trends
* Renewable Capacity Growth Comparisons
* Electricity Generation Mix by Region
* Correlation Heatmap of Sustainability Indicators


![Correlation Heatmap of Sustainability Indicators](ca_regional_indicator_corr.png)

*Figure 1: Correlation Heatmap of Sustainability Indicators.*



## Conclusions

Africa’s sustainable energy transition remains highly uneven and structurally complex.

The analysis shows that in Africa:

* renewable dominance alone is not sufficient evidence of modernization,
* household energy poverty remains widespread,
* economic growth still tends to increase emissions in fossil-dependent economies, and
* cleaner electricity systems do not automatically translate into broader energy access improvements.


## Recommendations

#### Infrastructure & Policy

* Expand modern electricity infrastructure in underserved regions
* Accelerate clean cooking fuel programs
* Strengthen grid reliability and transmission systems


#### Renewable Transition

* Move beyond traditional biomass dependence
* Scale utility-scale solar, wind, and geothermal deployment
* Improve regional grid integration


#### Decarbonization

* Reduce fossil-fuel electricity dependence in industrialized economies
* Prioritize coal transition strategies in Southern Africa


#### Financial Development

* Improve accountability and efficiency of foreign financial assistance
* Align funding toward measurable infrastructure outcomes


### Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy


## Author

CHIGOZIE OKONKWO  
Electrical Engineer | Data Science | Sustainable Energy Analytics

