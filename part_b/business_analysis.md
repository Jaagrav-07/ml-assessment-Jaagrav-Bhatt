B1 (a)
Target: items_sold
Features: store_size, location_type, promotion_type, competition_density, time features
Type: Supervised Regression

B1 (b)
Revenue depends on price → misleading
Items sold reflects true promotion effectiveness
Principle: Target variable must align with business objective

B1 (c)

Cluster-based models
OR
Store-specific models

B2 (a)
Join using:
store_id
date
Final grain:
store-month level

B2 (b)
Promotion vs sales
Seasonal trends
Store category comparison
Competition impact

B2 (c)
Problem: bias toward no promotion
Solution:
Resampling
Weighted modelsB3 (a)
Train: first 2.5 years
Test: last 6 months
Metrics:
RMSE → large errors
MAE → average error

B3 (b)
Use feature importance / SHAP
Show:
seasonality
promotions impact

B3 (c)
Save model → joblib
Monthly pipeline run
Monitor:
data drift
performance drop