
# Developer Salary Analysis: Influence of Database Skills

This project analyzes how a developer’s experience with different database technologies influences their yearly compensation, based on the 2024 Stack Overflow Developer Survey.

Followed CRISP-DM methodology for the project:
1. **Business Understanding** – Explore whether database skills are predictive of developer salaries.
2. **Data Understanding** – Use survey data and understand its schema.
3. **Data Preparation** – Clean and transform the data, especially the `DatabaseHaveWorkedWith` column.
4. **Modeling** – Train a linear regression model to predict salary from database usage.
5. **Evaluation** – Evaluate performance using R² and MSE.
6. **Deployment** – Present findings in an annotated Jupyter Notebook.

The notebook addresses three core questions:
1. Which databases are associated with higher median yearly salaries?
2. What does the overall salary distributionl look like (and what does that imply for analysis)?
3. Can we predict salary from database experience alone (and how good is the prediction)?


## Project Goals

  Determine which databases correlate with higher compensation.
  Visualize salary distribution by database technology.
  Predict salary using a machine learning model.
  Interpret model results with coefficients.


## Technologies Used

- **Python** (pandas, numpy, matplotlib, seaborn, scikit-learn)
- **Jupyter Notebook**
- **Stack Overflow Survey 2024**


## Files

- `Developer_Salary_Database_Analysis.ipynb`: Main notebook with code, visualizations, and model.
- `survey_results_public.csv`: Raw survey data from Stack Overflow.
- `survey_results_schema.csv`: Schema file explaining each column.

## Visuals


## The notebook includes:

- Distribution plot of yearly salary
- Bar plot of median salary by database
- Box plot of salary ranges for top databases
- Coefficient plots from the regression model


## Model

We train a **linear regression model** using one-hot encoded database usage features. The model attempts to predict developer compensation based solely on database experience. The results are evaluated using:
- **Mean Squared Error (MSE)**
- **R² Score**


## Conclusion

- Databases like **Redis**, **PostgreSQL**, and **Microsoft SQL Server** are associated with **higher compensation**.
- Database experience alone explains only part of salary variation. 
- Future iterations can incorporate other predictors like job title, education, experience, and location.


## Acknowlegments
Big thanks to [Stack Overflow](https://survey.stackoverflow.co/) for releasing this awesome data each year.
