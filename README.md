# Healthcare Insurance - My First Individual project

# ![alt text](assets/images/data-analytics-charts.jpg)

**Healthcare Insurance** is a dataset found in kaggle that I intend to use for my individual project. 

* The project focuses on analyzing health insurance data to understand the correlations between variables, discover underlying trends, and identify patterns that are not easily explained. 

* The aim is to clean, transform, and engineer the data to build a robust pipeline for visualizations. Hypothesis testing will be employed to draw meaningful and statistically valid conclusions from the analysis.


## Dataset Content
* The dataset provides information on clients personal characteristics (such as gender, age, family size and smoking status) as well as geographical location (the region of the country they belong to).

* The dataset further tells us how much each client is charged for their healthcare insurance.

The complete dataset can be found here [Healthcare insurance](<jupyter_notebooks/Source Data/insurance.csv>)


## Business Requirements

* As a healthcare provider, the business will inevitably charge some clients more than others. A key objective is to understand the factors that determine these pricing differences.

* A set of hypothesis will be formulated and tested using tools such as data transformation, feature engineering as well as data visualisation using Python tools such as Matplotlib, Seaborn and Plotly.


## Hypothesis and Validation

| Hypothesis number | Hypothesis description | Validation method |
|-------------------|------------------------|--------------------|
|1 | Smoking affects body fat distribution, increasing abdominal fat and influencing BMI, contributing to differences in health insurance costs. | In Python, create BMI categories based on NHS guidelines and analyze their relationship with smoking status. |
|2 | Body Mass Index (BMI) category significantly impacts insurance charges, as BMI serves as a proxy for health risk in insurance calculations. | Analyze how insurance charges vary across different NHS-defined BMI categories to understand BMI’s impact. |
|3 | Clients residing in certain geographic locations incur higher insurance costs due to regional healthcare costs, risk profiles, or socioeconomic factors. | Analyze how insurance charges vary across geographic locations to identify regions with significantly higher costs.|
| 4 | Age strongly correlates with insurance charges, reflecting increased health risks and medical costs as clients age. | Analyze insurance charge variation across ages to determine the relationship between age and insurance costs. |
|5 | Smoking status is a primary driver of higher insurance charges, with age acting as an additional compounding factor. | Examine insurance charges by smoking status and age to assess their combined effect on health risks and costs.|


## Project Plan

I used Github for the following tasks.

* Regularly push my updated code to [Github repo](https://github.com/ali-khurshid/My-Individual-Project)

* [Project Board](https://github.com/users/ali-khurshid/projects/2) to help me plan and keep track of my progress

![alt text](<assets/images/Project Board - Start.jpg>)


**Day 1 — Data Understanding & Preparation**
 
1. Import and Inspect the Dataset
2. Data Cleaning and Pre-processing
3. Exploratory Data Analysis (EDA)
4. Feature Engineering

**Day 2 — Analysis, Visualisation & Insights**

1. Creating a set of hypothesis and validation rules.
2. Data Visualisation (Matplotlib, Seaborn, Plotly) 
3. Descriptive Statistics & Correlation Analysis 
4. Key Insights, discussion and conclusion.


## The rationale to map the business requirements to the Data Visualisations

| Hypothesis                                                      | Visualization       | Description                                                                                  | Insights Highlighted                                                                                  |
|-----------------------------------------------------------------|---------------------|----------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| Smoking is directly related to weight gain. | Bar Chart           | Shows smoker and non-smoker counts across BMI categories (Underweight, Normal, Overweight, Obese) | Highlights the relationship between smoking status and BMI                                         |
| Smokers have higher insurance charges than non-smokers.         | Boxplot (Smoker Status)  | Compares insurance charges between smokers and non-smokers                                   | Reveals differences in distribution and median costs; impact of smoking on expenses                 |
| Insurance charges vary by geographic location.         | Boxplot (Location)     | Compares insurance charges across geographic locations                                        | Shows differences in median, IQR, and outliers; assesses the impact of location                      |
| Higher age and BMI correlate with increased insurance charges.  | Interactive Scatterplot (Age & BMI) | Plots age and BMI against insurance costs                                                    | Explores how both variables influence charges; identifies clusters and anomalies                     |
| Combined risk factors have a compounded effect on insurance costs. | Interactive Faceted Scatterplot   | Groups by smoker status, BMI, age group, and location                                         | Confirms previous patterns; visualizes interaction of multiple variables                             |
| Smoking status, age, and BMI are the strongest predictors.       | Interactive Correlation Heatmap   | Shows variable correlations with insurance charges                                            | Identifies strongest predictors and variables with little effect                                    |
                

## Analysis techniques used

* Performed data extraction, inspection, transformation, and feature engineering tasks using Jupyter notebooks.

* Created new columns in the DataFrame, such as BMI category and Age Group, utilizing custom functions and pandas methods.

* Engineered categorical variables to prepare the data for visualization, specifically for a Plotly correlation heatmap.

* Developed various visualizations including bar charts, scatter plots, box plots, and heat correlation maps to explore relationships within the data. The charts were updated in size with axes labeling and titles.


## Ethical considerations

* Since the data is anonymized, there is no risk of exposing personal information to the public. Additionally, because the data pertains to individuals residing in the USA, the data protection regulations under the UK and EU GDPR do not apply in this case.

* The age distribution is skewed toward younger individuals, which may introduce bias and limit the reliability of advanced data analytics methods, such as machine learning models. This imbalance can reduce model generalizability and lead to underperformance when predicting outcomes for older populations


## Unfixed Bugs

* I have no unfixed bugs to report. 


## Development Roadmap

* I encountered difficulties getting Plotly graphs to work due to a missing nbformat file. Using Microsoft Copilot, I discovered that a pip update was necessary to resolve the issue.

* Additionally, I faced a roadblock with Git commands returning errors. Kuminda assisted me by demonstrating an alternative approach and updating my Git main branch, which successfully resolved the problem


## Main Data Analysis Libraries

* Pandas
* Numpy
* Matplotlib
* Seaborn
* Plotly
* Sklearn Pre Processing
    * OneHotEncoder
    * LabelEncoder


## Discussion and Conclusion

**Note** - *Over one hundred outliers have been identified, representing less than 10% of the dataset. After careful consideration, the decision was made to retain these outliers in their original state to preserve the integrity and variability of the data. Removing or altering outliers without clear justification can risk loss of valuable information or introduce bias as these could point to additional unknown factors, such as pre-existing illness for example diabetes, high blood pressure etc. Therefore, they remain unchanged for further analysis.*

* **Hypothesis 1** was debunked --> Smoking is not a driving force for weight gain.

![alt text](<assets/images/1st Plot - Smoker Status vs BMI.jpg>)

* **Hypothesis 2**: There is a strong trend showing that smoking significantly increases insurance charges, with a well-documented positive correlation due to the elevated health risks smokers face. Increasing BMI categories also show a pattern of higher charges, although their impact is generally weaker compared to smoking. The exact strength of the correlation between BMI and insurance costs requires further verification, but it is clear that BMI contributes to risk assessment alongside smoking.

![alt text](<assets/images/2nd plot - Insurance charges vs Smokers and BMI.jpg>)

* **Hypothesis 3** was also debunked --> Geographic location has minimal impact on insurance charges when comparing median values across regions. However, variations in interquartile ranges suggest other factors influence costs within each area. Additionally, the presence of several outliers indicates that individual circumstances or additional variables contribute to the variability in insurance charges beyond geographic location alone. 

![alt text](<assets/images/3rd plot - Insurance charges vs location.jpg>)

* **Hypothesis 4**: A clear trend shows that insurance charges increase with client age, reflecting the higher health risks older individuals face. Additionally, heavier clients tend to incur higher insurance costs due to the increased risk associated with higher BMI. However, some anomalies exist, such as younger clients with lower BMI categories paying premium rates. One possible explanation for these outliers is that younger, healthy-weight individuals may have pre-existing conditions that elevate their insurance risk and costs. Multiple factors could drive these exceptions, highlighting the complexity of insurance pricing beyond age and BMI alone

![alt text](<assets/images/4th plot - Interactive scatterplot - insurance charge vs age and BMI.jpg>)

![alt text](<assets/images/5th plot - Interactive faceted scatterplot - insurance charge vs all variables.jpg>)

The following links will open in a web browser (preferably Chrome) to provide an interactive experience with the generated graphs.

[Insurance costs vs Age & BMI - Interactive Plot](<jupyter_notebooks/My Code/Scatterplot.html>)

[Insurance costs vs BMI category, Region, Age Group and Smoker Status](<jupyter_notebooks/My Code/Interactive Scatterplot.html>)


* **Hypothesis 5**: Smoking is clearly a significant contributor to higher healthcare costs, demonstrated by its strong correlation of 0.787 with insurance charges. Age is the next most influential factor, with a moderate correlation of 0.299, indicating that older individuals generally face higher costs. BMI, in contrast, has a weaker correlation, suggesting a lesser impact on insurance charges. Geographic regions show relatively weak negative correlations. These findings underscore that smoking is the most substantial driver of increased insurance costs among the variables analyzed, reflecting its well-documented health risks and associated expenses.

![alt text](<assets/images/6th plot - Correlation Heatmap.jpg>)

Here is the link that will provide an interactive experience with the Correlation heatmap. [Interactive Correlation heatmap](<jupyter_notebooks/My Code/Correlation Heatmap.html>)

### **Progress Summary**

Overall, the project board performed well. I successfully completed all 'Must Have' tasks, along with a couple of 'Could Have' items. Two tasks have been set aside to be addressed in future improvements to ensure continuous progress and refinement. This approach allowed the project to meet its core objectives while laying the groundwork for ongoing development.

![alt text](<assets/images/Project Board final.jpg>)


## Credits 

* [The Code Institute](https://codeinstitute.net/courses/) Learning Management System modules on pandas and data visualisations with Matplotlib,Seaborn and Plotly.

* ChatGPT alongside Microsoft Copilot integrated into Visual Studio Code was used to help with code generation and debugging.

* Template files provided by the course facilitator 


## Media

- The photo used on the home page was downloaded from Google Images, which is an open source site.


## Acknowledgements

* Thanks to all the teaching and support staff at Code Institute.
* Special thanks to Kuminda for clearing the Github roadblock for me.