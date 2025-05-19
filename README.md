# A-COMPARATIVE-STUDY-OF-ERROR-DISTRIBUTIONS-IN-HYBRID-TIME-SERIES-MODELS
Project involves using various error distributions in GARCH and EGARCH models to extract parameters, which are then utilized as input features for LSTM models. Later, different ensemble techniques will be applied to combine model outputs and evaluate improvements in forecast accuracy.

## Notebooks
1. **data_cleaning_and_preprocessing_and_graphs**: Data Cleaning, Data visualization, Feature engineering.
2. **Saving_GARCH_params_for_each_distribution_for_whole_data**: Using GARCH model to take last 23 days volatility data and predicting next day's volatility. Then extracting **alpha** and **beta**.
3. **Saving_EGARCH_params_for_each_distribution_for_whole_data**: Using EGARCH model to take last 23 days volatility data and predicting next day's volatility. Then extracting **alpha**, **beta** and **gamma**.
4. **walk_forward_val_for_GARCH**: Using walk-forward validation to train and test LSTM+GARCH models (LSTM + GARCH with ged, LSTM + GARCH with normal, ..)on different partitions of data.
6. **walk_forward_val_for_EGARCH**: Using walk-forward validation to train and test LSTM+EGARCH models (LSTM + EGARCH with ged, LSTM + EGARCH with normal, ..)on different partitions of data.
7. **Ensemble_model**: Using **average**, **median** and **ordinary linear regression** Ensemble techniques over predictions of all GARCH and EGARCH hybrib models combined.
