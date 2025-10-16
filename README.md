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

* **Hypothesis 1**: Smoking affects body fat distribution, increasing abdominal fat and influencing BMI. This variation in BMI induced by smoking contributes to differences in health insurance costs

*Validation* : In Python, create BMI categories based on NHS guidelines and analyze their relationship with smoking status.

* **Hypothesis 2**: Body Mass Index (BMI) category significantly impacts insurance charges, as BMI often serves as a proxy for health risk in insurance calculations.

*Validation* : Analyze how insurance charges vary across different NHS-defined BMI categories to understand the impact of body weight on insurance costs

* **Hypothesis 3**: Clients residing in certain geographic locations incur higher insurance costs, potentially due to regional healthcare costs, risk profiles, or socioeconomic factors.

*Validation* : Analyze how insurance charges vary across different geographic locations to identify regions where costs are significantly higher compared to others.

* **Hypothesis** 4: Age has a strong correlation with insurance charges, reflecting increased health risk and medical costs as clients get older.

*Validation* : Analyze how insurance charges vary across the ages presented in the dataset to determine if increased age corresponds with higher health risks and insurance costs

* **Hypothesis 5**: Smoking status is a primary driver of higher insurance charges, with age acting as an additional compounding factor.

*Validation* : Examine how insurance charges vary based on both smoking status and age in the dataset to assess whether these factors are associated with increased health risks and higher insurance costs


## Project Plan

I used Github for the following tasks.

* Regularly push my updated code to [Github repo](https://github.com/ali-khurshid/My-Individual-Project)

* [Project Board](https://github.com/users/ali-khurshid/projects/2) to help me plan and keep track of my progress

![alt text](<assets/images/Project Board - Start.jpg>)


Day 1 — Data Understanding & Preparation
 
1. Import and Inspect the Dataset
2. Data Cleaning and Pre-processing
3. Exploratory Data Analysis (EDA)
4. Feature Engineering

Day 2 — Analysis, Visualisation & Insights

1. Data Visualisation (Matplotlib, Seaborn, Plotly)
2. Descriptive Statistics & Correlation Analysis 
3. Key Insights & Recommendations.


## The rationale to map the business requirements to the Data Visualisations

* The **first visualization** is a bar chart showing smoker and non-smoker counts across BMI categories—Underweight, Normal, Overweight, and Obese—highlighting the relationship between smoking status and BMI.

* The **second visualization** is a boxplot comparing insurance charges between smokers and non-smokers, highlighting differences in distribution and median costs. This helps reveal the significant impact smoking status has on insurance expenses. 

* The **third visualization** is a boxplot comparing insurance charges across geographic locations, highlighting differences in median, interquartile range, and outliers. This helps assess the impact of location on insurance costs.

* The **fourth visualization** is a scatterplot that illustrates how age and BMI together influence insurance costs. It reveals trends such as whether increasing age and BMI are associated with higher charges. Additionally, this plot helps identify clusters or anomalies, offering insights into extended risk factors beyond the known variables.

* The **fifth visualization** is a faceted scatterplot that groups multiple categorical and numerical variables—such as smoker status, BMI category, age group, and geographic location—to confirm and reinforce patterns observed in previous visualizations. By displaying these variables simultaneously, it provides a comprehensive view of the data, helping to validate earlier findings and uncover any additional insights. This approach enhances understanding by revealing how different factors interact and contribute to insurance costs, making it a valuable tool for thorough risk assessment and data interpretation.

* The **sixth and final visualization** is a correlation heatmap that definitively shows which variables have the strongest impact on insurance charges versus those with weak or no correlation. By color-coding correlation coefficients, this heatmap clearly highlights key predictors—such as age, BMI, and smoking status—that significantly influence insurance costs, while also identifying variables with minimal effect. This visual tool is essential for confirming relationships found in prior analyses and guiding targeted strategies in insurance risk assessment and pricing

## Analysis techniques used

* Performed extract, transform, and feature engineering tasks using Jupyter notebooks.

* Created new columns in the DataFrame, such as BMI category and Age Group, utilizing custom functions and pandas methods.

* Engineered categorical variables to prepare the data for visualization, specifically for a Plotly correlation heatmap.

* Developed various visualizations including bar charts, scatter plots, box plots, and heatmap correlation maps to explore relationships within the data. The charts were updated in size with axes labeling and titles.


## Ethical considerations

* Given that the data pertains to healthcare costs, clients' physical and geographic information, compliance with GDPR will be essential in real-world projects to ensure data privacy, security, and lawful processing, in accordance with regulations such as obtaining explicit consent and safeguarding sensitive health information


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


## Conclusion



## Credits 

* [The Code Institute](https://codeinstitute.net/courses/) Learning Management System modules on pandas and data visualisations with Matplotlib,Seaborn and Plotly.

* ChatGPT alongside Microsoft Copilot integrated into Visual Studio Code was used to help with code generation and debugging.

* Template files provided by the course facilitator 

## Media

- The photos used on the home page was downloaded from Google Images

## Acknowledgements (optional)

* Thanks to all the teaching and support staff at Code Institute.
* Special thanks to Kuminda for clearing the Github roadblock for me.