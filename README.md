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

First clone the GitHub Classroom repository for this project through the `New Project` interface in RStudio, as described on the git instructions on the Canvas page. This should make a copy of the entire repository on your system and load the project into RStudio. You can always reload the project into RStudio from your file system by double-clicking the `popularity.Rproj` file.

Second, open up the `collaborator_bio.Rmd` file from within RStudio. Add a paragraph (at least three sentences) to this document describing yourself. You should also include your GitHub user name. When you are done, commit **and push** your changes. Remember that you must push your changes after the commit in order for other group members to get your changes when they pull. You should also run a pull command regularly to see the descriptions that other committee members have made. 

Its possible that you may run into conflicts if you and another group member edit the same line in this document. Don't panic! Just refer to the Canvas page instructions on how to resolve a conflict and fix it. 

Once all group members have submitted their bios, you can use the knit command in RStudio to turn your collaborator_bio.Rmd file into an HTML. One group member should commit and push this to the GitHub repository. Then go to the issues page on GitHub, open up a new issue, and summon me with the `@AaronGullickson` tag to let me know you are ready for assignment review. 

## Assignment 2: Describing the Key Variables

In this assignment, we will begin the analysis of the Add Health data. Our first step is to identify and describe the key variables in the analysis. These key variables are:

- The number of friend nominations (indegree) which will serve as our measure of popularity. 
- A "pseudo" measure of GPA (pseudoGPA) which will serve as our measure of academic achievement. 
- Alcohol use (alcoholuse).
- Smoking behavior (smoker). 

Please look at the descriptions of each variable in the information in the `input` directory and make sure you understand how they are being measured. The next step is to look at the distribution of each of these key variables in the dataset. You should consider how each variable is measured and use appropriate techniques to describe the distribution of the variables accurately in your report. 

### Report Guidelines

Use the R Markdown file `describe_vars.Rmd` to write your report. Your report should include the following information:

- A statement of the research question (in your own words) and a justification for why it is important to know the answer to this research question. Use your sociological imagination for the justification. This should be a single paragraph.

- A description of the dataset (in your own words) being used to analyze the data. Where does this data come from? When was it collected? Is it representative of all students? This should be a single paragraph. 

- Descriptions of the key variables (in your own words) that will be used to address the research question. Clarify what type of variable you have in each case and how the variable was measured. Describe the distribution of each variable focusing on issues of center, spread, shape, and outliers. You should describe each variable in a paragraph and include at least one figure showing its distribution.

Please keep the following guidelines in mind for all project reports: 

- Use clear, concise and accessible language throughout the report. Your target reader is not me, but rather a smart group of people who have little experience in interpreting statistics. Your job is to explain your results to them. 
- Because you will be describing things that are already described from other sources, be sure to not accidentally plagiarize text. Describe everything in your own words. 
- Do not refer to variables by their label in R (e.g. "indegree"). Do refer to variables in concrete meaningful ways (e.g. "number of friend nominations")
- Do not provide a narrative of your R script (e.g. "Then, I ran the tapply command to calculate mean differences between A and B "). Do present the results from your analysis in R in a way that someone who didn't know R from a hole in the ground would understand (e.g. "On average, members of A had XX more friend nominations than members of B").
- Do not use a casual tone. Do use a professional tone. 

When your final report is ready, one team member should knit the final report to HTML and commit and push this report to GitHub. Then open a new issue, and summon me with the `@AaronGullickson` tag to let me know you are ready for assignment review. 

## Assignment 3: Bivariate Associations

In this assignment, we will continue the analysis of the Add Health data. For this assignment we will look at the key bivariate relationships between variables in the dataset. I want you to analyze the following associations: 

- The association between smoking and alcohol use.
- The association between smoking and pseudo-GPA.
- The association between alcohol use and pseudo-GPA. 
- The association between smoking and friend nominations.
- The association between alcohol use and friend nominations.
- The association between pseudo-GPA and friend nominations. 

For your report, provide graphical and numerical summaries of these relationships using the tools that we have developed in the course. You will need to pay attention to the type of variable you have in each case in order to use the right measure of association and provide the correct graph. 

### Report Guidelines

Use the R Markdown file `bivariate_models.Rmd` to write your report. Your report should describe the relationships listed above, using 1-2 paragraphs to describe each relationship along with accompanying figures that show the relationship graphically. You do not need to provide an introduction or background for this report. 

Refer to the instructions for the previous assignment for further expectations about the report.

## Assignment 4: Full Report

In this assignment, we will complete the analysis of the Add Health data by constructing multivariate models predicting the number of friend nominations a student receives. You will then write a full report of your entire analysis, drawing upon the analysis conducted here and the results of your prior assignments. 

For this assignment, I want you to create three OLS regression models as follows: 

1. Predict friend nominations by pseudo-GPA, smoking, and alcohol use.
2. Predict friend nominations by pseudo-GPA, smoking, and alcohol use, as well as the control variables of race, sex, number of sports (nsports), and parentinc. 
3. Use all the same variables as in model (2) but also include an interaction between pseudo-GPA and smoking OR between pseudo-GPA and alcohol use (your choice). 

### Report Guidelines

Use the `full_report.Rmd` file to write your report. You should write a full report that contains the following sections:

1. Introduction: A statement of the research question (in your own words) and a justification for why it is important to know the answer to this research question. Use your sociological imagination for the justification. This should be a single paragraph.
2. Data: A description of the dataset (in your own words) being used to analyze the data as well as a description of the key variables used in the analysis, including figures.
3. Results: Present and describe the results of the multivariate OLS regression models. You do not need to interpret every slope in your regression model, but you should describe in simple terms the meaning of the slope for all of the key variables in your analysis and discuss how these results change across different models. You should also discuss the statistical significance of your findings. 
4. Conclusion: Summarize the findings as they relate to the original research question. 

You can draw upon your work in prior assignments for some of these sections, but be sure to consider any comments I have provided on these assignments for the final report. 

You must present your regression results using a table. The easiest way to do this is with the add-on `stargazer` package for R. You can install this package with the following command, when connected to the internet:

```r
install.packages("stargazer")
```

The `full_report.Rmd` contains a template code chunk using stargazer that should help get you started. Be sure to look at the Canvas page on using stargazer for more information. 

Refer to the instructions for assignment 2 for further expectations about the report.

