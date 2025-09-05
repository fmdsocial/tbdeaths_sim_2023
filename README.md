Author: Felipe Delpino

Year: 2025

Data Source: SIM/DATASUS (Mortality Information System)

Overview
This repository contains a comprehensive analysis of tuberculosis mortality patterns at the municipal level in Brazil for 2022. The analysis explores demographic characteristics, geographic distribution, and municipal clustering patterns using data from the Brazilian Ministry of Health.
Key Findings
Municipal Distribution

Total TB Deaths: [Your number here]
Affected Municipalities: [Your number here]
Mean Age: [Your number here] years
Male Predominance: [Your percentage here]%

Show Image
Demographics
Age Distribution
Most tuberculosis deaths occur in working-age adults, with the 30-44 age group being particularly affected.
Show Image
Sex Distribution
Males show significantly higher mortality rates compared to females.
Show Image
Municipal Characteristics
Analysis reveals distinct patterns in municipal TB mortality profiles based on mean age and demographic composition.
Show Image
Clustering Analysis
Hierarchical clustering identified distinct groups of municipalities with similar TB mortality patterns.
Show Image
Geographic Distribution
Spatial analysis shows heterogeneous distribution of TB mortality across Brazilian municipalities.
Show Image
Methodology
Data Collection

Source: SIM-DO (Sistema de Informações sobre Mortalidade - Declarações de Óbito)
Period: 2022 (January-December)
ICD-10 Codes: A15-A19, B90 (Tuberculosis)
Geographic Coverage: All Brazilian states

Analysis Approach

Data Processing: Age calculation, demographic categorization, municipal aggregation
Descriptive Analysis: Distribution analysis by age, sex, and geography
Statistical Testing: Chi-square tests, correlation analysis
Clustering: Hierarchical clustering using Ward.D2 method
Visualization: Municipal-level mapping and demographic plots

Tools

R version: 4.x
Key packages: microdatasus, dplyr, ggplot2, sf, geobr, cluster

Repository Structure
tuberculosis-brazil-analysis/
├── README.md                           # This file
├── tuberculosis_analysis.R             # Main analysis script
├── outputs/                            # Generated figures and data
│   ├── 01_death_distribution_municipalities.png
│   ├── 02_age_distribution.png
│   ├── 03_sex_distribution.png
│   ├── 04_municipal_characteristics.png
│   ├── 05_municipal_clusters.png
│   ├── 06_geographic_map.png
│   ├── municipal_summary.csv
│   ├── top_municipalities.csv
│   ├── summary_statistics.csv
│   └── cluster_analysis.csv
├── .gitignore
└── LICENSE
How to Reproduce
Prerequisites
r# Install required packages
install.packages(c("microdatasus", "dplyr", "ggplot2", "sf", 
                   "geobr", "viridis", "knitr", "cluster"))
Running the Analysis
r# Clone the repository
git clone https://github.com/[your-username]/tuberculosis-brazil-analysis.git

# Set working directory
setwd("tuberculosis-brazil-analysis")

# Run the complete analysis
source("tuberculosis_analysis.R")
Key Results
Municipal Burden

Significant variation in municipal TB mortality burden
Top 20 municipalities account for [X]% of total deaths
Geographic concentration in [specific regions]

Demographic Patterns

Male-to-female ratio: [X:1]
Peak mortality in [age group] years
[X]% of deaths occur in individuals aged 30-59

Clustering Insights

[Number] distinct municipal clusters identified
Cluster characteristics:

Cluster 1: [Description]
Cluster 2: [Description]
Cluster 3: [Description]



Public Health Implications

Targeted Interventions: Results identify priority municipalities for TB control programs
Resource Allocation: Clustering analysis supports evidence-based resource distribution
Risk Group Focus: Demographic patterns inform targeted screening strategies
Geographic Surveillance: Municipal mapping highlights areas requiring enhanced monitoring

Limitations

Analysis limited to mortality data (does not include TB incidence)
Administrative boundaries may not reflect epidemiological patterns
Underreporting in some regions may affect completeness
Socioeconomic factors not included in current analysis

Data Availability
Raw data is publicly available through DATASUS (https://datasus.saude.gov.br/).
Processed datasets are included in the outputs/ folder.
Citation
If you use this analysis or code, please cite:
Delpino, F.M. (2025). Tuberculosis Mortality Analysis in Brazil: Municipal-Level 
Patterns and Clustering. GitHub repository: 
https://github.com/[your-username]/tuberculosis-brazil-analysis
Contact
Felipe Mendes Delpino
Email: felipe.delpino@gmail.com
ORCID: https://orcid.org/0000-0002-3562-3246
License
This project is licensed under the MIT License - see the LICENSE file for details.
Acknowledgments

Brazilian Ministry of Health for providing public access to mortality data
DATASUS team for maintaining the SIM database
R community for developing the analytical tools used in this study
