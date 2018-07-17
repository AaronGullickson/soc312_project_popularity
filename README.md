# Putting It All Together Group Project

Throughout the term, we will be working in groups to build up an analysis of a specific research question, detailed below. At the conclusion of most modules, you will complete a Putting It All Together assignment that asks you to analyze the dataset using the specific tools you have learned within that module. For each assignment, you will report your results in a brief report. The goal of this set of assignments is to prepare you for the solo research project that you will conduct at the end of the term, in which you will put all of these components together to answer a different research question. 

You are free to organize your group as you like, but I recommend that you nominate one person to be the organizational lead for each assignment. This person will be responsible for handling conflicts, knitting final results, and communicating completion to me. You can rotate this responsibility among group members if you like. 

## Research Topic: Popularity and Substance Use among Adolescents

We will use data from the Add Health survey of adolescents in a sample of American high schools. This survey asked students to nominate their friends from the same school, from which one can construct network data. A subset of the  data that we will use for this analysis and more information about the dataset can be found in the `input` directory of this repository. 

Public health researchers have long been concerned about the effect of peer pressure and social networks on adolescents’ use of alcohol, tobacco, and drugs. The Add Health survey provides an important opportunity to study such effects because it contains data on both substance use and students’ social networks. We will use the Add Health data to address the question of how academic achievement and substance use (smoking and alcohol) affect a student’s popularity, as measured by the number of friend nominations received.

## Technical Issues

We will be using several technical tools that will help facilitate group work for this project. You may initially find these tools frustrating due to lack of familiarity, but ultimately they should help your group to better work on this project collaboratively and to track each student's contribution to the project. These tools will also make it easier for me to provide assistance to your group. 

All of the work for this project will be done using the [git](https://git-scm.com/) version control system and GitHub classroom. You should read the separate instructions on Canvas about how to install git and how to use it through RStudio. You should also sign up for an account on [GitHub](https://github.com). All of the data and documentation for this project is contained within a git repository that you will clone to your own computer. You can then make changes to files in that repository through RStudio and commit and push those changes so that other group members can see the work that you have done. 

We will also be using [R Markdown](https://rmarkdown.rstudio.com/) to write the actual reports as HTML (web page) documents. You should read in full the instructions for using R Markdown on the Canvas page and be sure to install the necessary packages in order to run R Markdown through RStudio. R Markdown will allow you to create professional quality reports with your tables and figures fully integrated. All of the reports that you need to create for this project already have R Markdown templates for you to follow in order to produce the report. 

Finally, you can and should use the GitHub interface to help coordinate activities between team members. In particular, the **issues** tab above can be used for group communication. You can reference specific team members by prefacing their GitHub user name with a `@` (like twitter). This feature can also be used to get my attention by using `@AaronGullickson` to summon me. 

## Assignment 1: Getting used to Git and Markdown

This assignment is intended to ensure that you have git and Markdown properly installed on your system and understand how to use them. 

First clone the GitHub Classroom repository for this project through the `New Project` interface in RStudio, as described on the git instructions on the Canvas page. This should make a copy of the entire repository on your system and load the project into RStudio. You can always reload the project into RStudio from your filesystem by double-clicking the `popularity.Rproj` file.

Second, open up the `collaborator_bio.Rmd` file from within RStudio. Add a paragraph (at least three sentences) to this document describing yourself. You should also include your GitHub user name. When you are done, commit **and push** your changes. Remember that you must push your changes after the commit in order for other group members to get your changes when they pull. You should also run a pull command regularly to see the descriptions that other committee members have made. 

Its possible that you may run into conflicts if you and another group member edit the same line in this document. Don't panic! Just refer to the Canvas page instructions on how to resolve a conflict and fix it. 

Once all roup members have submitted their bios, you can use the knit command in RStudio to turn your collaborator_bio.Rmd file into an HTML. One group member should commit and push this to the GitHub repository. Then go to the issues page on GitHub, open up a new issue, and summon me with the `@AaronGullickson` tag to let me know you are ready for assignment review. 

## Assignment 2: Describing the Key Variables

In this assignment, we will begin the analysis of the Add Health data. Our first step is to identify and describe the key variables in the analysis. These key variables are:

- The number of friend nominations (indegree) which will serve as our measure of popularity. 
- A "pseudo" measure of GPA (pseudoGPA) which will serve as our measure of academic achievement. 
- Alcohol use (alcoholuse).
- Smoking behavior (smoker). 

Please look at the descriptions of each variable in the information in the `input` directory and make sure you understand how they are being measured. The next step is to look at the distribution of each of these key variables in the dataset. You should consider how each variable is measured and use appropriate techniques to describe the distribution of the variables accurately in your report. 

### Report Guidelines

Your report should include the following information:

- A statement of the research question (in your own words) and a justification for why it is important to know the answer to this research question. Use your sociological imagination for the justification. This should be a single paragraph.

- A description of the dataset (in your own words) being used to analyze the data. Where does this data come from? When was it collected? Is it representative of all students? This should be a single paragraph. 

- Descriptions of the key variables (in your own words) that will be used to address the research question. Clarify what type of variable you have in each case and how the variable was measured. Describe the distribution of each variable focusing on issues of center, spread, shape, and outliers. You should describe each variable in a paragraph and include at least one figure showing its distribution.

Use clear, concise and accessible language throughout the report. Your target reader is not me, but rather a smart group of people who have little experience in interpreting statistics. Your job is to explain your results to them. Because you will be describing things that are already described from other sources, be sure to not accidentally plagiarize text. Describe everything in your own words. 

When your final report is ready, one team member should knit the final report to HTML and commit and push this report to GitHub. Then open a new issue, and summon me with the `@AaronGullickson` tag to let me know you are ready for assignment review. 

## Assignment 3: Bivariate Relationships

In this assignment, we will continue the analysis of the Add Health data discussed in the Putting It All Together Overview. You can download the data here. Information about the dataset is available herePreview the document. 

Our next step is to look at the key relationships between variables in the dataset. I want you to analyze the following relationships. 

The relationship between smoking and friend nominations.
The relationship between alcohol use and friend nominations.
The relationship between pseudo-GPA and friend nominations. 
For your report, provide graphical and numerical summaries of these relationships using the tools that we have developed in this module. You will need to pay attention to the type of variable you have in each case in order to use the right measure of association and provide the correct graph. You should conduct your analysis using a well-commented R script. 

### Report Guidelines

Your report should include a 1-2 page (single-spaced) description of each relationship as well as accompanying tables and figures.

Use clear, concise and accessible language throughout the report. Your target reader is not me, but rather a smart group of people who have little experience in interpreting statistics. Your job is to explain your results to them.

All figures and tables should be shown at the end of the report. Caption all figures and tables with numbers and reference them within the text. More information on getting tables and figures from R into Word can be found here. 

## Assignment 4: Full Report

In this assignment, we will continue the analysis of the Add Health data discussed in the Putting It All Together Overview. You can download the data here. Information about the dataset is available herePreview the document. 

We are now ready to build full multivariate models of the key relationships. For this assignment, I want you to create three OLS regression models as follows: 

Predict friend nominations by pseudo-GPA, smoking, and alcohol use.
Predict friend nominations by pseudo-GPA, smoking, and alcohol use, as well as the control variables of race, sex, number of sports (nsports), and parentinc. 
Use all the same variables as in (2) but also include an interaction between pseudo-GPA and smoking OR between pseudo-GPA and alcohol use. 
You should conduct your analysis using a well-commented R script. 

### Report Guidelines

Your report should include a 1-2 page (single-spaced) description of your results as well as a table of the regression results. You should interpret the results for the key variables of pseudo-GPA, alcohol use, and smoking across all three models as well as the interaction terms in model 3. You do not need to interpret all of the other variables, but you should note if results change for your key variables based on the inclusion of these control variables.  

Use clear, concise and accessible language throughout the report. Your target reader is not me, but rather a smart group of people who have little experience in interpreting statistics. Your job is to explain your results to them.

The table should be shown at the end of the report with a proper caption. More information on producing a nicely formatted table of regression results using Word can be found here. 

Please remember these guidelines in writing your report:

Do not refer to variables by their label in R (e.g. "indegree"). Do refer to variables in concrete meaningful ways (e.g. "number of friend nominations")

Do not provide a narrative of your R script (e.g. "Then, I ran the tapply command to calculate mean differences between A and B "). Do present the results from your analysis in R in a way that someone who didn't know R from a hole in the ground would understand (e.g. "On average, members of A had XX more friend nominations than members of B").

Do not use a causal tone. Do use a professional tone. 