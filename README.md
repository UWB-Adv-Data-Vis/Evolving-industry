# Evolving-industry: Examining Key Industry Sector Growth and Decline in Washington 
This data challenge attempts to visualize the growth and decline of key industry sectors in Washington State. Data come from the U.S. Bureau of Labor and Statistics. 

### Team
-   📊 Challenge created by and made for the BDATA 412 [Advanced Data Visualization](https://github.com/UWB-Adv-Data-Vis) course at the [University of Washington Bothell](https://www.uwb.edu/).
-   ✍️ Authored by [Toby M.](https://github.com/), [Bryan H.](https://github.com/).
-   🔍 Challenge review committee: [Toby M.](https://github.com/),
-   🛠️ Edited and supervised by Prof. [Caleb Trujillo](https://github.com/calebtru).

## Learning Objectives
In this assignment you will demonstrate your ability to:

*    Prepare data by appropriately formatting it for analysis, summarizing, and filtering.
*    Answer meaningful research questions using the tools in one or more software packages to work with authentic data.
*    Be capable of running, modifying, and sharing scripts to accomplish analyze data and visualize in one scripting language (R).
*    Manage project development to store, organize, and track code using digital collaboration tools for reproducibility (GitHub).
*    Create a data dashboard for the web to disseminate findings and visualization (R Shiny)
*    Describe the rationale, methods, results, and broader social context of your student-led project that used data to answer an interesting question.
*    Describe and use different types of critical and scientific thinking to develop inquiry into selected projects and critique visualizations.

## Challenge Overview 

Our data challenge is to focus in Washington and examine 3 different sectors and their related occupations: Aerospace, Agriculture/manufacturing and Information/Communications technology. Using the datasets provided by the U.S Bureau of Labor, we want to see and visualize the overall growth/decline within these occupations and sectors, based on employment numbers and wages in the past 3 years.

## Intent of the Dashboard

The goal here is to create some awareness for job seekers interested in the industry and related occupations and help analysts and people working at the federal level insights about the economic state and health. From this information, we also hope to see how any recent technological developments could have influenced any growth/decline we may find in regards to these industries in Washington. Our possible stakeholders are people who may be interested in these occupations/sectors and want to see the current job markets for them and policymakers/analysts interested in seeing the current health of parts of Washington’s economy and current state based on a fraction of their labor force.

## Data Challenge Statement

This challenge asks teams to turn complex industry data into a clear, easy-to-use dashboard using R Shiny and ggplot2. We intend the dashboards to be accessible and understandable to the general public, prioritizing creative layouts, clear labeling, and clear data storytelling so that it enables non-technical users to engage with the visualizations meaningfully. By making the dashboard easily accessible to the public, it will provide a good reference for students or any public stakeholders trying to understand the trends of industry sectors. 

### Why This Challenge Matters

As students who are preparing to enter the workforce, knowing what industries have opportunity and what industries are oversaturated is necessary for future success. In addition, recent technological developments have continually made headlines on the disruptiveness in several industries; by viewing how these sectors have been affected in recent years, we can see how much they’ve either grown or declined from them. In addition, by identifying the growth or decline in the number of available jobs and the growth or decline in wages across different industries we can better determine where to direct our efforts in job searching. 


### What We Hope to Learn

We hope to learn, through this project, what industries have the best future prospects for a career. Our claim is that different industries have different career opportunities, and we would like to show a trend over the past three years to demonstrate this difference. We will be letting the data speak for itself rather than weaving a narrative. Our purpose isn't to explain why a given industry is experiencing an upturn or downturn, but to instead make use of that information to make good judgements. With that in mind, there should only be one conclusion to our data rather than multiple interpretations which is to see whether or not a given industry is doing well or poorly for employment opportunities and financial gain.


## Tasks to address for our challenge

The dashboard _could_ function visuals:
- Show the change over time in regards to wages and overall employment in these three sectors.
- Compare these occupations and sectors against each other by year.
- Correlate wages with employee growth/decline over the years.
- Relate wage and employment for comparing industries across years.
- Determine consistency, growth and decline with both occupations and sectors.
- Create a dashboard compiling all plots together.

# The Data
## Background 

The Occupational Employment and Wage Statistics (OEWS) dataset, produced annually by the U.S. Bureau of Labor Statistics (BLS), provides employment and wage estimates for more than 800 occupations across the United States. It includes national and state-level estimates of employment, hourly and annual wages, percentile wages, and measures of statistical reliability. The data for wages and employment was collected through a semiannual survey of approximately 1.1 million business establishments and are processed using weighting, validation, and statistical adjustment methods before publication. 

As this dataset is annually collected by a federal department with employment and wages in mind, the data collected from it serves as a reliable viewpoint into the current state of the economy and workforce across industries to be used in labor market analysis, workforce planning, economic forecasting, compensation benchmarking, and public policy, whether at a national level or by specific state. Because of these possibilities of analysis and insights, government agencies and employers can use these to find out about employment and wage trends, and job seekers interested in these sectors can help better grasp these trends and help reach a decision to enter or reconsider based on what they find. Some publications have gathered many findings as a result from using this datasets, such as finding out which jobs were below $15 per hour (Mattingly, 2024) and the state of the oil and gas industry in 2024 (Occupational Employment and Wages in Oil and Gas Industries, May 2024 : Monthly Labor Review : U.S. Bureau of Labor Statistics, 2024). 

## Data set details

The published data are summarized statistical estimates rather than raw responses. Most employer information is kept confidential.
Other limitations include the exclusion of self-employed workers, unpaid family workers, and most agricultural workers; possible suppression of estimates due to confidentiality or insufficient sample sizes; sampling error; and a time lag between data collection and publication. 
Comprehensive documentation, metadata, and methodology are available from the BLS, and numerous research publications have relied on OEWS data to analyze wage and employment patterns. 

### Dataset details:

The data source that we will be using is from the U.S. Bureau of Labor Statistics for Labor Force, we will be looking at the annual average years from 2011 to 2024 dataset of 11b. Employed persons by detailed occupation and age. This range attempts to capture the different trends of more than a decade of labor market dynamics from the Great Recession recovery, COVID-19, and now the current labor market restructuring. The dataset is split between management/professional occupations and service occupations, spanning over 300 occupations combined, each is a table. 
 
### Data Source Links: 
 - U.S. Bureau of Labor Statistics for OEWS Dataset [Link](https://www.bls.gov/oes/tables.htm)
 - Consider using a R package like blscrapeR, blsAPI, BLSloadR to avoid limitations related to multiple sheets and large data storage.

### Understanding Table Organization :
 - Example Table: Overview of May 2022 occupational employment and wages [2022] [https://www.bls.gov/cps/aa2014/cpsaat11.htm](https://www.bls.gov/oes/2022/may/overview_2022.htm)
 - OEWS documentation [https://www.bls.gov/oes/oes_doc.htm](https://www.bls.gov/oes/oes_doc.htm)

### Data Accessibility and Quality:
For data retrieval specifically where the data sources are:

- Occupational Employment and  Wage  Statistics (BEWS) [https://www.bls.gov/oes/tables.htm](https://www.bls.gov/oes/tables.htm)
- Other sources (Aiding in the objectives of the dashboard, Demographic Data Sources, etc) [https://www.bls.gov/data/apps.htm](https://www.bls.gov/data/apps.htm)


## Project Plan:
Week-phase planned tasks with goals are listed.

### First Week: 
Planning, Design, and Data Cleaning 
- Draw sketches for the visualizations we want to produce.
- Use and identify OCC codes + industries, including only the ones related to three sectors (ITC, Agricultural, Aerospace).
- Filter and organize based on information or missing values.
- Combine datasets into a single excel/csv format for all 3 years and for occupations.
 
### Second Week: 
Prototyping and 
- Begin programming and create visualizations/plots for the data.
- Planned charts are line, scatterplot and bar, but we can research additional ones that may better suit our visualizations.
- Make prototypes of the sketches we made.
- Create some basic ggplot visuals.
- Correct any miscellaneous errors with visuals or data.
- Do a preliminary data analysis.
- Go through many visualization iterations to narrow down on visuals we like best.
- Get feedback from team mates, professor, and others.

### Third Week: Programming 
- We will focus on pulling out the most important information and visualizations.
- We will do more complex aggregations on the data if necessary for better visuals.
- Remove unnecessary visuals.
- Add labels to the ggplots.
- Refine the visual appearance of the project.

### Fourth Week: Refinement & Publishing
- Examine our variables and see if there's connections and fits our purpose.
- Add a user interface if there is time.
- Use visualization principles to refine and polish visualizations to be more appealing.
- Gather feedback and finalize.
- Revise the final visualizations.
- Upload the visuals online.


## References
Key Industries. (2024, September 9). Washington State Department of Commerce. [https://www.commerce.wa.gov/key-sectors/](https://www.commerce.wa.gov/key-sectors)

Mattingly, A. (2024, September 25). A Look at Jobs Paying Less Than $15.00 Per Hour. Bureau of Labor Statistics. [https://www.bls.gov/spotlight/2024/a-look-at-jobs-paying-less-than-15-00-per-hour/home.htm]([https://www.bls.gov/spotlight/2024/a-look-at-jobs-paying-less-than-15-00-per-hour/home.htm])

U.S. Bureau of Labor Statistics. (2019, August 26). Occupational Employment and  Wage  Statistics. Bls.Gov. [https://www.bls.gov/oes/tables.htm](https://www.bls.gov/oes/tables.htm)

Watson, Audrey, Occupational employment and wages in oil and gas industries, May 2024 : Monthly Labor Review : U.S. Bureau of Labor Statistics. (2024). Bureau of Labor Statistics. [https://www.bls.gov/opub/mlr/2026/article/occupational-employment-and-wages-in-oil-and-gas-industries-may-2024.htm](https://www.bls.gov/opub/mlr/2026/article/occupational-employment-and-wages-in-oil-and-gas-industries-may-2024.htm)
