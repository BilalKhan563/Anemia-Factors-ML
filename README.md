# Factors Affecting Children Anemia Level

This dataset represents a cross-sectional study conducted during the 2018 Nigeria DHS. It aims to measure various factors that potentially influence anemia levels in children aged 0-59 months.

## Overview

### Dataset Description
- The dataset comprises several factors that could contribute to anemia levels in children, including demographics, health-related questions, and socioeconomic indicators.
- Columns like `Age_in_5year_groups`, `Type_of_place_of_residence`, `Highest_educational_level`, and `Wealth_index_combined` offer insights into potential influences on anemia.

### Data Exploration and Insights
- Visualizations revealed intriguing patterns:
  - **Anemia in Relation to Smoking:** Non-smokers seem more prone to anemia.
  - **Impact of Recent Fever:** Children who experienced fever in the last two weeks showed a higher likelihood of anemia.
  - **Medication Intake:** Anemia prevalence seems lower among those taking iron pills, sprinkles, or syrup.

### Model Development and Evaluation
- **Data Preprocessing:** Addressed missing values and converted data types for model compatibility.
- **Machine Learning Model:** Utilized RandomForestClassifier:
  - Trained on a split dataset (80% training, 20% testing).
  - Achieved a model accuracy of 99.38%.

### Model Performance Analysis
- While the model showcases high accuracy, further domain-specific considerations might be needed to determine practical implications.
- Considerations:
  - Are false negatives or false positives more critical in this context?
  - Sensitivity or specificity measures could provide a deeper understanding of the model's predictive power.

### Challenges and Limitations
- **Data Completeness:** Missing values, especially in hemoglobin-related columns, were handled by imputation.
- **Dataset Scope:** Limitations might exist in capturing all factors influencing anemia, requiring supplementary data or refined modeling techniques.

### Future Steps
- **Refinement and Validation:** Experiment with various models, conduct cross-validation, and hyperparameter tuning for robustness.
- **External Validation:** Validate the model with external datasets or conduct domain expert reviews for further validation and insights.
