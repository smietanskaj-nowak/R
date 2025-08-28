# College Classification Project in R

This repository contains an R Markdown project that performs classification on the **College dataset** from the `ISLR` package.  
The goal of the project is to predict whether a university is **private or public** based on selected institutional and financial parameters.

---

## Dataset

The **College** dataset includes information on U.S. colleges and universities across 18 variables, such as:

- `Private` – institution type (Yes = private, No = public)
- `Apps` – number of applications received
- `Accept` – number of applications accepted
- `Enroll` – number of new students enrolled
- `Outstate` – out-of-state tuition
- `Room.Board` – room and board costs
- `F.Undergrad` – number of full-time undergraduates
- `P.Undergrad` – number of part-time undergraduates
- `Terminal` – percentage of faculty with terminal degree
- `perc.alumni` – percentage of alumni who donate
- `Expend` – instructional expenditure per student
- `S.F.Ratio` – student–faculty ratio
- `Grad.Rate` – graduation rate

---

## Methods

The analysis focuses on predicting the `Private` variable (Yes/No) using selected predictors:

- `Outstate`
- `Room.Board`
- `F.Undergrad`
- `Terminal`
- `perc.alumni`
- `Expend`
- `S.F.Ratio`

### Models used:
- **Logistic Regression** – baseline classification model
- **Classification Trees (CART)** – tree-based classification approach

---

## ⚙️ Implementation

The project is implemented in **R** using:

- `ISLR` – dataset
- `tidyverse` – data manipulation and visualization
- `tree` – classification trees

---

## Running the Project

1. Clone or download this repository.
2. Open `projekt_Joanna_SmietanskaNowak.Rmd` in RStudio.
3. Knit the document to HTML/PDF to reproduce the full analysis.

---

## Results

- Logistic Regression provides an interpretable baseline model for predicting whether a college is private.  
- Classification Trees are applied to improve predictive performance and to visualize decision rules.  
- The models are evaluated using accuracy and confusion matrices.
- - **Classification Trees** were implemented using the `tree` package in R. 

  - The overall classification error rate was **7.20%**, meaning the tree correctly classified **92.8% of cases**.  
  - The model demonstrated robust performance in predicting institutions classified as `Private` (`Yes`).  

- To improve model performance, **tree pruning** was also experimented with, which reduced model complexity and helped to avoid overfitting while maintaining a high level of accuracy.  

---

## License

This project is provided for educational purposes.  
If you use or adapt it, please cite the author of the project report.

