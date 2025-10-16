# Healthcare Insurance - My First Individual project

# ![alt text](assets/images/data-analytics-charts.jpg)

**Healthcare Insurance** is a dataset found in kaggle that I intend to use for my individual project. 

* The project focuses on analyzing health insurance data to understand the correlations between variables, discover underlying trends, and identify patterns that are not easily explained. 

* The aim is to clean, transform, and engineer the data to build a robust pipeline for visualizations. Hypothesis testing will be employed to draw meaningful and statistically valid conclusions from the analysis.


## Dataset Content
* The dataset provides information on clients' personal characteristics (such as gender, age, family size and smoking status) as well as geographical location (the region of the country they belong to).

* The dataset further tells us how much each client is charged for their healthcare insurance.

The complete dataset can be found here [Healthcare insurance](<jupyter_notebooks/Source Data/insurance.csv>)

## Business Requirements

* As a healthcare provider, the business will inevitably charge some clients more than others. A key objective is to understand the factors that determine these pricing differences.

* A set of hypothesis will be formulated and tested using tools such as data transformation, feature engineering as well as data visualisation using Python tools such as Matplotlib, Seaborn and PLotly.


## Hypothesis and how to validate?

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
* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations
* List your business requirements and a rationale to map them to the Data Visualisations

## Analysis techniques used
* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques. Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations
* Were there any data privacy, bias or fairness issues with the data?
* How did you overcome any legal or societal issues?

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Main Data Analysis Libraries
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section up into Content and Media, depending on what you have included in your project. 

### Content 

- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)
* Thank the people who provided support through this project.