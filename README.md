# Chi-Square Test of Independence – Titanic Dataset

## Project Overview
This project applies the **Chi-Square Test of Independence** to the Titanic dataset to examine whether passenger gender and survival status are statistically associated.

The analysis uses Python and common data-analysis libraries. The Titanic dataset contains **891 passenger records and 15 columns** in the version loaded by this notebook.

## Objective
To test whether there is a statistically significant relationship between:
- **Gender** (`sex`)
- **Survival status** (`survived`)

## Tools and Libraries
- Python
- Pandas – data manipulation and contingency tables
- NumPy – numerical operations
- Seaborn – loading the Titanic sample dataset
- SciPy – performing the Chi-Square test

## Workflow
1. Import the required Python libraries.
2. Load the Titanic dataset using `seaborn.load_dataset("titanic")`.
3. Create a contingency table with `pd.crosstab()` using gender and survival status.
4. Run `scipy.stats.chi2_contingency()` to calculate the Chi-Square statistic, p-value, degrees of freedom, and expected frequencies.
5. Compare the p-value with the significance level (`alpha = 0.05`).
6. Interpret the test result.

## Key Results

| Measure | Result |
|---|---:|
| Chi-Square statistic | 260.7170 |
| p-value | 1.1973570627755645 × 10⁻⁵⁸ |
| Degrees of freedom | 1 |
| Significance level (α) | 0.05 |

### Observed Contingency Table

| Gender | Did not survive (0) | Survived (1) |
|---|---:|---:|
| Female | 81 | 233 |
| Male | 468 | 109 |

## Conclusion
Since the p-value is far below 0.05, the null hypothesis of independence is rejected. The analysis indicates a **statistically significant association between gender and survival status** in this Titanic dataset.

This result shows an association; it does not by itself establish that gender caused the difference in survival.

## How to Run
1. Download or clone this repository.
2. Open `Chi_Square_Test_Titanic.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab.
3. Run the cells from top to bottom.

The notebook loads the Titanic dataset through Seaborn, so an internet connection may be needed the first time the dataset is fetched.

## Repository Contents
- `Chi_Square_Test_Titanic.ipynb` – notebook containing the Python analysis.
- `README.md` – project documentation and summary.

## Author
Nagendran C
