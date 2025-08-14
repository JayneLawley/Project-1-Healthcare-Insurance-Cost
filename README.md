# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)
## Project 1 Healthcare Insurance Cost

This project explores how personal and geographic factors (such as age, gender, BMI, smoking status, and region) influence insurance costs. The aim is to examine patterns and relationships in the data to better understand what drives variations in healthcare charges, using visual exploration and summary insights to explain the findings.

## Dataset Content
* The dataset contains information about individual's age, gender, body mass index (BMI), number of children, smoking status, and region within the United States in relation to the medical insurance charges they were charged.

## Business Requirements
* To understand how different geographical, personal and lifestyle factors affect healthcare insurance costs in the United States, in order to improve cost estimation, support pricing strategies and identify areas of customer risk.

## Hypothesis and how to validate
**Hypotheses:**
* People who smoke are likely to have higher medical healthcare insurance charges than those who don’t.
* Higher BMI may also be linked to increased medical healthcare insurance charges. 
* Medical healthcare insurance charges increase with age.
* Geographic region may influence medical healthcare insurance charges.
* Number of children might affect medical healthcare insurance charges.
* Sex may influence medical healthcare insurance charges.

I will use visualisations like boxplots, scatter plots and bar charts to compare charges across different groups (for example smokers vs non-smokers, different BMI levels, age ranges and regions) to check the above hypotheses.
 

## Project Plan
* **Data Collection and setup**: The dataset was downloaded from Kaggle and saved as csv file into the 'raw' data folder.
* **Initial Data Review and Cleaning**: The data was reviewed for duplicates, missing values, and incorrect datatypes. Any necessary cleaning was completed before analysis began.
* **Exploratory Data Analysis and Visualisation**: Visualisation techniques (such as boxplots, scatter plots, bar charts, line plots, and violin plots) have been used to explore the data. Chart types were selected based on what best suited the data being compared and the hypotheses being tested. 

## The rationale to map the business requirements to the Data Visualisations
The aim of this project was to understand how different factors influence healthcare insurance charges in the United States (this type of information can help with predictive analysis of charges, and can help identify risks). Visualisation was the main tool used to explore patterns, compare groups, and test hypotheses. Here's how the business questions were mapped to the visual tools used:
- Are smokers charged more than non-smokers?
- Visualisations used: Boxplots, scatter plots, histograms, KDE plots and seaborn lineplot.

I used these charts as they clearly show the distribution and spread of charges for smokers vs non-smokers, making differences easy to spot. Scatter plots also reveal how charges escalate with other variables (like age and BMI) depending on smoking status.

**Does BMI affect medical insurance charges?**
- Visualisations used: Scatter plots, line (rounded BMI values), and boxplots (with BMI categories).
I used scatter plots and box plots as BMI is a continuous variable, so scatter plots were helpful for spotting trends. Grouping BMI into medical categories made patterns easier to interpret and allowed visual comparisons across standardised health risk groups.

**Do charges increase with age?**
- Visualisations used: Line plots (with age groups), scatter plots with trendlines.
As age is a continuous variable, plotting it with line and scatter plots helped to show the gradual increase in charges with age. Adding a trendline made the pattern clearer.

**Does region influence charges?**
- Visualisations used: Boxplots and violin plots by region.
I used a boxplot and found limited evidence that region influenced charges. I then used a violin plot to delve deeper. The plot tpyes made it easy to compare distributions across the four regions. These visuals helped confirm that region had limited influence.

**Do other demographic factors (like sex and number of children) affect charges?**
- Visualisations used: Boxplots with smoker hue
These visuals were used to test for patterns, but helped show that sex and number of children do not appear to be strong predictors of insurance charges in this dataset.

## Analysis techniques used

I used visual exploratory analysis (EDA) as my primary method for indentifying relationships and trends within the dataset. The main focus was on understanding how different factors (such as BMI, age and smoking status) relate to healthcare insurance costs. 
**Methods used:**
- Boxplots: to show distributions and spot differences between categories (e.g. smoker vs non-smoker).
- Scatter plots: for exploring continuous variables like age and BMI in relation to charges.
- A violin plot: to show shape and spread of distribution (to delve deeper in a region based comparison).
- Histograms and KDE plots: to show charge distributions for smokers vs non-smokers.
- Line plots: used for trends across binned ages and rounded BMI values.

I tested each business question with a visualisation that best suited the variable types (categorical vs numerical, numerical vs numerical, and category vs category). For example:
- BMI was continuous, so I used scatter plots first, then grouped it into medical categories to simplify as the first plot was too noisy.
- Region was categorical, so I used box and violin plots to compare spreads. I used resources such as data to Viz to help guide me on what might work best (https://www.data-to-viz.com/).

## Limitation and alternative approaches:
- Some variables (like region, number of children and sex) showed little variation or impact on charges, limiting their usefulness in drawing insights and conclusions. 
- BMI values were unevenly distributed. I tried a line plot using rounded values, but found some limitations within the dataset information (particularly in the higher ranges).

## Use of generative AI tools: 
- I used CoPilot when writing code to help troubleshoot, and it also helped speed up commenting on my code.
- I used Chat GPT 4.0 to also help debug code, and suggest clearer visualisation choices.
- I have used Chat GPT 4.0 to check my markdown, and help review my work for clarity.

## Ethical and legal considerations

The dataset used in this project is sourced from Kaggle and is intended for learning and practice. It does not contain real personal data, so it does not pose any direct privacy or ethical risks in its use.

However, the dataset represents real-world, sensitive personal attributes such as age, BMI, and smoking status. This could raise ethical questions around how such data is used, particularly if it were applied in real settings to make decisions (e.g. refusing insurance cover or setting higher premiums for certain groups).

While this project does not involve predictive modelling or decision-making, it’s important to remain aware of these implications when working with data related to health, lifestyle, or demographic factors.

## Dashboard Design
- The project does not include a formal dashboard, as the focus is on exploratory data analysis and visualisation using Jupyter Notebooks. However, the notebook has been structured in a clear and logical way to serve a similar function, walking the user through the insights step by step. The combination of markdown commentary and visuals is designed to communicate findings to both technical and non-technical audiences.
- A range of visual types were used to suit different audiences (e.g. scatter plots, boxplots, violin plots, line plots, histograms). Some less successful plots have been kept to show the exploratory process and demonstrate why certain chart types were chosen over others.
- Annotations, titles, and axis labels were added to support understanding without needing to read raw code. I have used comments to explain what each plot is trying to show (and what the key insights are) for both technical and non-technical audiences.

## Unfixed Bugs
- There was one small bug in the Jupyter notebook related to a code block intended for folder creation. The code is shown below:
import os  
try:  
  # create your folder here  
  # os.makedirs(name='')  
except Exception as e:  
  print(e)
As this section was not essential to the functioning of the notebook, and was intended to be replaced with a conclusion section later. This code has since been removed.It did not affect analysis, or outputs, during project development.

## Knowledge Gaps
A few knowledge gaps were identified around:
- selecting most appropriate data visualisation types
- managing code errors
- identifying that an upgrade patch was needed for Plotly to display correctly
These were addressed by:
- experimenting with plot types
- seeking help from my tutor
- using online resources like 'data to Viz'
- using tools like CoPilot and ChatGPT to debug, explore alternatives, and understand syntax

## Development Roadmap
- Challenges faced:
    Choosing the most effective visualisation types for different data relationships
    Folder and file structure not being recognised and realised I needed to restart my kernel!
    Managing early bugs and syntax issues, especially when switching between libraries like Seaborn, Matplotlib, and Plotly
    Interpreting charts accurately and drawing clear conclusions
- Strategies used:
    Reviewing course notes and tutorial notebooks
    Asking for help from my tutor
    Using online tools like ChatGPT and GitHub Copilot for debugging and testing alternative approaches
- Next steps:
    Build confidence in interpreting and presenting data insights
    Explore more advanced visualisation techniques and interactive dashboards
    Strengthen skills in hypothesis testing and statistical analysis

## Conclusion
In this project I set out to explore how personal, lifestyle, and regional factors influence healthcare insurance charges using a publicly available Kaggle dataset. Through visual analysis, I identified several key insights:
- Smoking status had the strongest impact on charges, with smokers consistently incurring much higher costs.
- BMI and age were also strong predictors, particularly when combined with smoking.
- Region, sex, and number of children showed little to no significant effect on charges in this dataset.

Using a range of visualisation techniques (including Matplotlib, Seaborn, and Plotly), I tested each hypothesis and refined the approach as insights became visible. Some visuals were included even where clarity was lower, to demonstrate the exploratory process and support learning.

The project met its goal (to uncover relationships in the data and explain what influences variations in insurance charges). It also allowed me to develop and demonstrate skills in data cleaning, visual data analysis, and data driven storytelling.

### Heroku

* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the runtime.txt Python version to a [Heroku-20](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
6. If the slug size is too large then add large files not required for the app to the .slugignore file.

## Main Data Analysis Libraries
* Pandas, Matplotlib, Seaborn, Plotly

## Credits 
* For help choosing apppropriate visualisation types, I referred to [data to Viz]: https://www.data-to-viz.com/#line, and my tutorial notebooks developed while working through the Code Insitute LMS. 
* I used the CDC (U.S. Centers for Disease Control and Prevention) website for medical BMI category groupings https://www.cdc.gov/bmi/adult-calculator/bmi-categories.html?CDC_AAref_Val=https://www.cdc.gov/obesity/basics/adult-defining.html
* I received support from my tutor Vasi Pavaloi for resolviong coding issues and understanding how to approach certain tasks.
* I have used Chat GPT 4.0 and GitHub CoPilot to debug code, understand errors, and explore different ways to write and (or improve) functions and code.

### Content 
- The text for the Home page was taken from Wikipedia Article A
- Instructions on how to implement form validation on the Sign-Up page was taken from [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media
- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site

## Acknowledgements (optional)
* Thank you to Vasi who has provided support through this project.