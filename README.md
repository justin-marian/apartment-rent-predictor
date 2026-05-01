# :house: Apartment Rent Prediction

> [!NOTE]  
> Complete machine learning regression workflow for predicting apartment rental prices.

> [!TIP]
> Full experimental workflow, while the report summarizes the methodology, results, and conclusions.

> [!IMPORTANT]  
> The task was to build and evaluate a complete prediction pipeline, starting from exploratory analysis and ending with model comparison, tuning, and final validation.

## :pushpin: Project Includes

- :bar_chart: EDA of the dataset, including missing values, target distribution, correlations, outliers, and visualizations.
- :broom: Data preprocessing, including numeric conversion, invalid-value handling, missing-value imputation, categorical encoding, and target clipping.
- :building_construction: Feature engineering based on real-estate domain knowledge, such as area per room, room density, floor ratio, building age, spatial cluster features, central-sector indicators, premium-neighborhood flags, and amenity indicators extracted from text.
- :robot: Training and comparison of several regression models:
  - :straight_ruler: Ridge regression as a linear baseline
  - :deciduous_tree: Decision Tree regression
  - :evergreen_tree: Random Forest regression as a bagging method
  - :rocket: XGBoost regression as a boosting method
- :test_tube: Ablation experiments to compare preprocessing and feature-engineering variants, including raw vs. log-transformed target, base vs. engineered features, and different categorical encoding strategies.
- :mag: Hyperparameter tuning using `RandomizedSearchCV` for the strongest models.
- :jigsaw: Final ensemble validation using multiple XGBoost variants and out-of-fold RMSE evaluation.

> [!NOTE]  
> Multiple notebooks are included, each corresponding to experiments that obtain different RMSE scores. Some notebooks differ only slightly in preprocessing, features, tuning, or ensemble settings, while others may introduce larger changes that lead to more visible score differences.
