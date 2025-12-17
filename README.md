# Titanic Survival Prediction

This project uses the Kaggle Titanic dataset to build machine learning models that predict whether a passenger survived the disaster.

## Project overview

The Jupyter notebook follows a simple progression:

1. **Data loading & basic EDA**
   - Load `train.csv` and `test.csv` from Kaggle.
   - Inspect columns, missing values, and basic summaries.
   - Plot simple relationships such as survival by sex and passenger class.

2. **Baseline model**
   - Apply basic cleaning (fill missing `Age`, `Embarked`, `Fare`).
   - Create a few simple features (for example, family size and a cabin flag).
   - Encode categorical variables and train a baseline Random Forest classifier.
   - Use a train/validation split to get an initial accuracy score.

3. **Advanced features & improved model**
   - Add richer features such as:
     - child indicator
     - ticket group size
     - fare per person
     - binned age and fare (bands)
   - Retrain models on this feature set and compare performance.
   - Tune the best model briefly to improve accuracy.

4. **Final predictions**
   - Fit the final model on all training data.
   - Generate predictions for the test set.
   - Export a `submission_final.csv` file in the Kaggle format (`PassengerId`, `Survived`).

## How to run

1. Download the Titanic data (`train.csv`, `test.csv`, `gender_submission.csv`) from Kaggle.
2. Place the files in the same folder as `Kaggle_Titanic_project.ipynb`.
3. Open the notebook in Jupyter and run the cells from top to bottom.

The notebook is meant as a learning exercise in basic EDA, feature engineering, and supervised classification on a well‑known dataset.
