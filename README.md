GLOBAL CO2 EMISSIONS RESPONSIBILITY : Total vs Per-Capita vs Historical Accountability Dashboard

Project Overview 
This project presents an interactive dashboard that explores global CO₂ emissions responsibility from different perspectives. It compares total country emissions, emissions per capita, and historical cumulative emissions to better understand fairness and accountability in climate change.

The dashboard is designed to support climate policy discussions, sustainability planning, and public awareness by turning complex environmental data into clear and easy-to-understand visual insights for both technical and non-technical users.


#Dataset Content
The dataset used in this project was obtained from Our World in Data (OWID), which compiles global CO₂ emissions statistics from trusted research sources such as the Global Carbon Project.
The dataset includes country-level data across multiple years.
Key variables used in this project:
Country – Name of the country
Year – Reporting year
Total CO₂ emissions – Annual national emissions
CO₂ emissions per capita – Emissions per person
Population – Used for scaling and comparison
The dataset covers several years, which allows the analysis of historical trends and cumulative emissions.
The data is publicly available and licensed for reuse. It does not contain any personal or sensitive information.

# Business Requirements
The dashboard was developed to answer the following key business and policy questions:
Which countries contribute the most to global CO₂ emissions? 
How have global emissions changed over time?
How does per-capita responsibility differ from total emissions?
Which countries hold the greatest historical accountability?
Which regions are driving emissions growth?


# Hypothesis and how to validate?
H1: Global CO₂ emissions have increased significantly since 1990,the baseline year widely used in international climate agreements. 
Validation: This will be evaluated using a global emissions trend line to observe changes over time

H2: Developed countries tend to have higher CO₂ emissions per capita compared to developing countries.
Validation: This will be assessed through per-capita emission rankings and scatter plot comparisons.

H3: Countries with large populations account for higher total emissions but do not necessarily rank highest in per-capita emissions.
Validation: This will be analysed using a total versus per-capita scatter plot divided into responsibility quadrants.

H4: Countries with the highest historical cumulative emissions are not always the same as those with the highest current annual emissions.
Validation: This will be examined through cumulative emissions time-series analysis and ranking comparisons.

# Project Plan
Planning
    Define business case
    Identify datasets
    Establish hypotheses
Data Collection
    Source OWID dataset
    Verify licensing and governance
Data Processing
    Clean missing values
    Filter relevant years
    Create derived metrics
Analysis
    Trend analysis
    Responsibility comparisons
    Growth calculations
Dashboard Development
    Build visualisations in BI tool
    Apply UX principles
Evaluation
    Validate hypotheses
    Review usability
Deployment
    Publish repository
    Document workflow

# How was the data managed throughout the collection, processing, analysis and interpretation steps?
    Raw data stored in DataSet/Raw/
    Cleaned datasets stored in DataSet/Cleaned/



# Why did you choose the research methodologies you used?
# The rationale to map the business requirements to the Data Visualisations
# List your business requirements and a rationale to map them to the Data Visualisations
# Analysis techniques used
List the data analysis methods used and explain limitations or alternative approaches.
How did you structure the data analysis techniques. Justify your response.
Did the data limit you, and did you use an alternative approach to meet these challenges?
How did you use generative AI tools to help with ideation, design thinking and code optimisation?
Ethical considerations
Were there any data privacy, bias or fairness issues with the data?
How did you overcome any legal or societal issues?
Dashboard Design
List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
Later, during the project development, you may revisit your dashboard plan to update a given feature (for example, at the beginning of the project you were confident you would use a given plot to display an insight but subsequently you used another plot type).
How were data insights communicated to technical and non-technical audiences?
Explain how the dashboard was designed to communicate complex data insights to different audiences.
Unfixed Bugs
Please mention unfixed bugs and why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
Did you recognise gaps in your knowledge, and how did you address them?
If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.
Development Roadmap
What challenges did you face, and what strategies were used to overcome these challenges?
What new skills or tools do you plan to learn next based on your project experience?
Deployment
Heroku
The App live link is: https://YOUR_APP_NAME.herokuapp.com/
Set the runtime.txt Python version to a Heroku-20 stack currently supported version.
The project was deployed to Heroku using the following steps.
Log in to Heroku and create an App
From the Deploy tab, select GitHub as the deployment method.
Select your repository name and click Search. Once it is found, click Connect.
Select the branch you want to deploy, then click Deploy Branch.
The deployment process should happen smoothly if all deployment files are fully functional. Click now the button Open App on the top of the page to access your App.
If the slug size is too large then add large files not required for the app to the .slugignore file.
Main Data Analysis Libraries
Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.
Credits
In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials, however, it is important to be very specific about these sources to avoid plagiarism.
You can break the credits section up into Content and Media, depending on what you have included in your project.
Content
The text for the Home page was taken from Wikipedia Article A
Instructions on how to implement form validation on the Sign-Up page was taken from Specific YouTube Tutorial
The icons in the footer were taken from Font Awesome
Media
The photos used on the home and sign-up page are from This Open-Source site
The images used for the gallery page were taken from this other open-source site
Acknowledgements (optional)
Thank the people who provided support through this project.