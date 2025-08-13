# Project 1 Healthcare Insurance Cost

**Project Healthcare Insurance** explores how personal and geographic factors (such as age, gender, BMI, smoking status, and region) influence insurance costs. It will look at how this data can be used to estimate healthcare expenses and provide insights and predictive reports around healthcare insurance charges based.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)


## Dataset Content
* The dataset contains information about individual's age, gender, body mass index (BMI), number of children, smoking status, and region within the United States in relation to the medical insurance charges they were charged.


## Business Requirements
* To understand how different geographical, personal and lifestyle factors affect healthcare insurance costs in the United States, in order to improve cost estimation, support pricing strategies and identify areas of customer risk.


## Hypothesis and how to validate?
* People who smoke are likely to have higher insurance charges than those who don’t.
* Higher BMI may also be linked to increased charges. 
* Insurance charges are expected to increase with age.
* Geographic region might play a role in the variation of costs of medical insurance.

I will use visualisations like boxplots, scatter plots and bar charts to compare charges across different groups (for example smokers vs non-smokers, different BMI levels, age ranges and regions). I'll also review summary statistics such as averages and counts to support findings.

 

## Project Plan
* **Data Collection and setup**: The dataset will be downloaded from Kaggle and saved as csv file into the 'raw' data folder.
* **Initial Data Review and Cleaning**: The data will be checked for duplicates, missing values, and incorrect datatypes. Any necessary cleaning will be completed before analysis is undertaken.
* **Exploratory Data Analysis and Visualisation**: Visualisation techniques (such as boxplots, barcharts, line plots, and violin plots) will be used to explore the data. Visuals will be selected based on what best suits the data being compared and the hypotheses being tested. 

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

## Dashboard Design
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs
* Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap
* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Deployment
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
* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.


## Credits 

* For help choosing apppropraite visualisation types, I referred to [data to Viz]: https://www.data-to-viz.com/#line, and my tutorial notebooks developed whioole working through the Code Insitute LMS. 
* I received support from my tutor Vasi for resolviong coding issues and understanding how to approach certain tasks.
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