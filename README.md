```markdown
# Predicting Thermal Conductivity and Oxide Scale Thickness in ZrB₂ Composites

This repository contains the materials and code associated with the M.Tech thesis work titled **"Predicting Thermal Conductivity and Oxide Scale Thickness in ZrB₂ Composites: A Machine Learning Approach"** by Karthikeya Pervela. The project focuses on leveraging machine learning models to predict key thermal properties of ultra high temperature ceramic (UHTC) composites, with an emphasis on ZrB₂-based materials.

## Table of Contents

- [Overview](#overview)
- [Motivation](#motivation)
- [Objectives](#objectives)
- [Methodology](#methodology)
  - [Data Collection and Preprocessing](#data-collection-and-preprocessing)
  - [Machine Learning Models](#machine-learning-models)
- [Results and Analysis](#results-and-analysis)
- [Repository Structure](#repository-structure)
- [Usage](#usage)
- [Future Work](#future-work)
- [Acknowledgements](#acknowledgements)
- [License](#license)

## Overview

This project addresses the need for high-performance materials in aerospace applications such as hypersonic flight and re-entry. The focus is on predicting:
- **Thermal Conductivity:** Using regression models to forecast how the composition, microstructural parameters, and testing conditions affect thermal conductivity.
- **Oxide Scale Thickness:** Using machine learning techniques to determine the oxidation resistance and the corresponding oxide layer thickness.

The work also involves balancing imbalanced datasets with the Synthetic Minority Over-sampling Technique (SMOTE) and comparing performance improvements using Random Forest Regression and XGBoost Regression.

## Motivation

Ultra High Temperature Ceramics (UHTCs) are critical for aerospace applications due to their ability to withstand extreme thermal conditions. However, their performance is highly sensitive to compositional and microstructural variations. This project aims to:
- Develop data-driven models that predict the thermal performance of ZrB₂ composites.
- Identify the key parameters that influence thermal conductivity and oxide scale formation.
- Provide a framework that bridges experimental data with computational modelling, potentially guiding future experimental designs.

## Objectives

- **Develop Predictive Models:** Construct machine learning models to forecast thermal conductivity and oxide scale thickness.
- **Data Augmentation:** Apply SMOTE to balance datasets and improve model reliability.
- **Parameter Analysis:** Analyze the influence of compositional, microstructural, and testing parameters on the performance of ZrB₂ composites.
- **Model Evaluation:** Assess model performance using metrics like Mean Absolute Error (MAE) and R² value.

## Methodology

### Data Collection and Preprocessing

- **Datasets:** Initial datasets consist of measured properties for various compositions of ZrB₂ composites. Two main datasets are considered:
  - **Thermal Conductivity Dataset:** Comprising 90 initial compositions, later augmented to 172 using SMOTE.
  - **Oxide Scale Thickness Dataset:** Based on 84 compositions, balanced to 129 samples via SMOTE.
- **Feature Engineering:** The datasets include compositional features (e.g., ZrB₂, SiC, ZrC, etc.), microstructural properties (e.g., relative density, mean grain size), and testing conditions (temperature, time).
- **Data Binning:** Testing temperatures are divided into specific bins to account for variation in experimental conditions.

### Machine Learning Models

- **Random Forest Regression:** Applied to predict thermal conductivity, evaluating the influence of various parameters.
- **XGBoost Regression:** Employed for both thermal conductivity and oxide scale thickness prediction, with model performance improvements highlighted after SMOTE.
- **Model Evaluation:** Performance is assessed using R² values and Mean Absolute Error (MAE) for both prediction tasks.

## Results and Analysis

- **Thermal Conductivity:** The best model achieved an MAE of 8.95 W·m⁻¹K⁻¹ and an R² value of 0.66. Key influencing factors include relative density, temperature, and ZrB₂ content.
- **Oxide Scale Thickness:** XGBoost Regression improved the R² from 0.83 to 0.88 after applying SMOTE. Temperature and SiC content were identified as the most statistically significant factors.
- **Correlation Analysis:** Detailed correlation studies were performed to understand the statistical impact of each parameter on the predicted properties.


## Acknowledgements

- **Supervisor:** Prof. Kantesh Balani, Department of Materials Science & Engineering, IIT Kanpur.
- **Collaborators:** Lab members and staff of the Biomaterials Processing and Characterization Lab, and the Materials Science and Engineering Department.
- **Special Thanks:** Dr. Rubia Hassan for her guidance on problem formulation and Dr. Shipra Bajpai for assistance with thesis writing. Finally, heartfelt thanks to friends and family for their continuous support.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```
