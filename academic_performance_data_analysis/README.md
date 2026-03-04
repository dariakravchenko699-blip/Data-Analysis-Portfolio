## Student Academic Performance Analysis

# Project overview

This project investigates factors influencing academic performance (GPA) using 
statistical analysis and data visualization. The analysis explores relationships 
between key success metric GPA and demographic factors (age, gender) as well as behavioral 
patterns (study time, absences). This research also aims to help understand models for predicting 
GPA.

# Key Research Questions

1) What is the proportion of female to male high school students?
2) Does GPA differ across age groups (15-18)?
3) Is there a significant GPA difference between males and females?
4) Does weekly study time influence GPA?
5) Which factors have the strongest correlation with GPA?

# Tools and Technologies

Python was used for data analysis and statistical modelling of the dataset while 
Power Bi and Tableau were used for visualization.

Python libraries

pandas
seaborn
matplotlib
scipy
statsmodels

# Dataset 

The dataset used in the analysis contains information on performance metrics such 
as grades and GPA, as well student background information including demographical factors, 
such as ethnicity, gender, age, parents' education levels and behavioral factors including absences
extra study time, tutoring and various extracurricular activities.

<img width="915" height="623" alt="Screenshot 2026-03-03 at 10 26 03 PM" src="https://github.com/user-attachments/assets/ec25ea09-b5f7-4a27-b56b-5aea22c663ba" />


# ANALYSIS PROCESS

# 1. Data Cleaning 

Before evaluation the data was cleaned from empty values and duplicates. 

# 2. Exploratory Data Analysis

Initial exploration included:

- summary statistics for gender, age, GPA and study time weekly
- 
<img width="565" height="407" alt="Screenshot 2026-03-03 at 10 28 54 PM" src="https://github.com/user-attachments/assets/54746311-698d-496e-b637-77954641deb7" />
<img width="586" height="408" alt="Screenshot 2026-03-03 at 10 28 46 PM" src="https://github.com/user-attachments/assets/e82e0181-8458-4b03-8f8a-2615dabf763f" />

- GPA and Study Time Weekly distribution analysis and normality testing
  
<img width="600" height="466" alt="Screenshot 2026-03-03 at 10 29 02 PM" src="https://github.com/user-attachments/assets/aaa31efd-8d49-4d1c-b58e-047cc9c07c74" />
<img width="598" height="457" alt="Screenshot 2026-03-03 at 10 29 11 PM" src="https://github.com/user-attachments/assets/da3996b7-b6ea-4b92-8af9-518a3b33c7e1" />

- Boxplots for demographic comparisons
  
<img width="320" height="672" alt="Screenshot 2026-03-03 at 3 05 12 PM" src="https://github.com/user-attachments/assets/b8a2e80e-44fd-4959-8d26-57dee87fd8a5" />
<img width="235" height="667" alt="Screenshot 2026-03-03 at 3 05 05 PM" src="https://github.com/user-attachments/assets/dbb504bb-6922-4c8b-857d-7049a2bd7b06" />

- Correlation heatmap

# 3. Hypothesis Testing

Using individual T-test and ANOVA test for group comparisons we have arrived 
at the conclusion that there is no significant differenc to GPA across different
genders and ages.

# 4. Regression Modelling 

The correlation heatmap showed a few numerical factors that could have a relationship with 
GPA. Study Time Weekly showed a very week positive correlation and absences showed
a really strong negative correlation with GPA. 

Having found these correlations, we have built simple linear regression with the OLS method
to describe GPA by absences and study time weekly independently. Both models turned out
to be statistically significant.

<img width="599" height="486" alt="Screenshot 2026-03-03 at 10 31 10 PM" src="https://github.com/user-attachments/assets/ab885229-3608-4b21-86e4-b5bf2c526d54" />
<img width="657" height="608" alt="Screenshot 2026-03-03 at 3 05 29 PM" src="https://github.com/user-attachments/assets/1430844f-f12d-423b-817a-94ab9d5c6f42" />

# CONCLUSIONS

Our goal was to observe relationships between GPA, demographic and behavioral factors.

So far research has shown:

1) Age and gender have no statiscally significant impact on GPA.
2) Even though the heatmap seems to imply a positive correlation between GPA and Study
   Time Weekly, its correlation is very weak according to Pearson coefficient.
4) The only statistically significant correlation between variables and GPA is observed between GPA and absences, which
   implies that out of all observed factors (demographic and behavioural) absences have the greatest
   impact on GPA.

<img width="836" height="480" alt="Screenshot 2026-03-03 at 11 05 31 PM" src="https://github.com/user-attachments/assets/ed762b3c-8bf9-42b5-a9f6-f97119a8771d" />


