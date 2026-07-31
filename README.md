# Has Anything Actually Changed? Post-Apartheid Labor Outcomes in South Africa

**Erin Brzusek**  
Georgetown University

# Abstract

This study seeks to examine the long-term economic effects of legalized discrimination in post-Apartheid South Africa. Recreating the methodological framework of previous research on the effects of government-mandated racial classification, I utilize data from the 2001 and 2011 South African Census to evaluate labor outcomes. Specifically, I analyze income disparities among men and women across "White" and "Coloured" racial categories. Utilizing various approaches to Ordinary Least Squares (OLS) regression, I analyze income and assess the extent to which historical socioeconomic divides persist. By recreating the previous analysis with more recent census data, this project provides insights into the current state of economic inequality in South Africa.

| 2001 Income by Sex | 2011 Income by Sex |
|:---:|:---:|
| ![2001 Income by Sex](images/2001_income.png) | ![2011 Income by Sex](images/2011_income.png) |

## Repository Structure

```
├── index.qmd        
├── library_zortero.bib    
├── style.css
├── chicago-17-no-url.csl
├── _quarto.yml
├── .gitignore
├── images/      
├── docs/
├── assets
├── apartheid.ipynb                 
└── README.md              
```

# Introduction

The history of South Africa stands as a fascinating case study for the field of `Causal Inference for Computational Social Science`. The Apartheid era was black-and-white legalized discrimination. The implementation of the National Party's ideological framework hinged on the Population Registration Act of 1950, which required every citizen to be classified and registered under racial categories. The government was then able to dictate an individual's rights from "cradle to grave". Legislation such as the Group Areas Act forced non-white populations into the country’s most economically unproductive areas, while "pass laws" criminalized the unregulated movement of Coloured citizens within urban spaces. Systemic oppression extended to all individual pursuits: schools were segregated and interpersonal relationships across racial lines were legally barred through measures like the Prohibition of Mixed Marriages Act. 

In their study examining the direct impacts of Apartheid-era racial classifications, Pellicer et al. (2023) utilized historical census microdata around the Registration Act of 1950 in a Fuzzy Regression Discontinuity (Fuzzy RD) framework. The Fuzzy RD design isolated the causal effect of being classified as White rather than Coloured. Their findings demonstrate that receiving a White classification yielded a massive 4.5-fold increase in male income and an average of 5 additional years of formal education. This accounted for approximately 94% of the total observed mean income disparity between White and Coloured men.

Though Apartheid formally ended in 1994, whether market forces and post-Apartheid reforms have succeeded in closing historical gaps remains a question. While all South Africans are now constitutionally recognized as equals, state policies such as employment equity targets were explicitly designed to remediate historical disenfranchisement. These policies remain highly contentious; critics characterize them as unconstitutional forms of social engineering. The competing sociological and political realities underscore a fundamental economic inquiry: *in the wake of Apartheid, to what extent have labor market disparities between racial categories actually changed?*

This study seeks to address this question by examining a decade of post-Apartheid labor dynamics using 10% microdata samples from the 2001 and 2011 South African Censuses. To address omitted variable bias and non-linearities, I employ various approaches to Ordinary Least Squares (OLS) regression including single cross-section, pooled cross-section, and propensity score matching. Ultimately, this paper evaluates whether the conditional racial wage gap between White and non-White individuals has narrowed, stagnated, or widened, providing new empirical evidence on post-Apartheid economic convergence.