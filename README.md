House Price Prediction (ML)
A focused Machine Learning project using Python to predict residential property prices. The analysis contrasts a baseline model with Ridge and Lasso regularization, demonstrating proficiency in data preprocessing and model optimization.

Model Performance Summary
The performance of the final model, measured by the R² score on the unseen test data, indicates its predictive power.

Metric	Model	Score	Impact
R² Score (Test Set)	Optimized Ridge	0.5495. The model explains about 55% of the variability in house prices.

Key Predictive Insights
The top feature coefficients reveal the most influential factors, sorted by absolute impact on the standardized price.

Feature	Coefficient	Impact Direction	Business Insight
poor_prop	-3.77	Strong Negative	Higher concentration of low-quality properties strongly drives down price.
room_num	+2.78	Strong Positive	The number of rooms is the most significant structural value factor.
teachers	+2.40	Strong Positive	High teacher-to-capita ratio acts as a strong proxy for neighborhood quality.

Export to Sheets
Technical Workflow
Data Cleaning: Implemented outlier capping (e.g., on n_hot_rooms and rainfall), missing value imputation, and log transformation on the skewed crime_rate feature.

Modeling & Optimization: Employed Standard Scaling before training the final model. Used validation_curve to perform hyperparameter tuning for the best-performing Ridge model.

Repository Files
time\_series\_analysis (1).py: Python Script (full code for all preprocessing and ML models).

04\_House\_Price.csv: Raw Dataset.
