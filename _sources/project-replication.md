# Project III

## Description
In this assignment, you will be replicating the findings of an empirical research article in the social sciences. Any social science research article (psychology, sociology, economics, public policy, etc.) published in a peer-reviewed journal is fair game. You can find papers with code from sources such as the [Harvard Dataverse](https://dataverse.harvard.edu/dataverse/RepData) or the [Replication Wiki](https://replication.uni-goettingen.de).

## Checklist

- You will be turning in the items below. Page limits must be within reason. You will want to use Microsoft Word or any text editor (e.g., Pages) or markup language (e.g., LateX) for the write-up. Adherence to the [APA style guidelines](https://apastyle.apa.org) is recommended.
- **Introduction** [25\%]: research question(s), statistical technique(s).
- **Methodology** [25\%]: model, variables, data.
- **Results** [50\%]: key table or figure.

## Structure
The replicated article must implement one of the statistical methods covered in the class (e.g., difference-in-differences, synthetic control, neural networks, etc.). Any other advanced methodology which has not been presented in class is also fine. You might not choose articles that implement basic statistical techniques (e.g., descriptive statistics, linear regression, logistic regression, etc.). The other requirements are quite loose; ideally, however, you want to find an article that:
- Has been published in the last two decades;
- Implements a code routine in one or more programming languages (Python, R, STATA, etc.).
- Includes a data submission. Some submissions point to a publicly available dataset which might be downloaded for free from the web. If this is the case, make sure to download the data and include it in your submission.

Replicating a paper means re-running the analysis from begin to end using the code and data provided. That entails:
- Reading the research paper and understand the research question it addresses;
- Downloading all the replication materials;
- Installing the required software and packages on your machine. Note that version requirements are often an issue for reproducibility. At times, authors reference the package versions (e.g., R version 3.6). This is THE reason why you want to start early. Believe it or not, you are more than halfway through your project when the replication code runs without error on your machine.
- Running the code line by line.
- Saving all the outputs.

To complete the assignment, you will need to turn in a replication memo including the parts below.

### Introduction 
Here, you introduce the:
- *(Main) research question*. This is the causal relationship that the paper is looking at. You typically want to express the research question in terms of dependent and independent variables.
- *Statistical or machine learning technique*. Name the technique used for identification of the causal effect. Include information about the identification conditions. For example, regression discontinuity requires that the running variable is discontinuous around the cutoff. The authors must have said something about it. Please note down any other details that are relevant for understanding of the study.

### Methodology
Here, you will discuss the:
- *Model*. Rewrite the empirical model. Yes, you will need to rewrite the regression equation or the other maths used in the original paper walking the reader through the variables and parameters. No creative heroics here. Discuss the functional form, the structure of the error term, the coding of the variables. Make sure to distinguish between dependent variable, control variables, and key explanatory variable(s).
- *Data*. Generate a toy example of the data with all the variables and their coding. This can be a screenshot (not recommended), an Excel file (recommended), or any other file format (also recommended). If the script recodes, reshapes, and reformats the native dataset – this is typically accomplished in the first few lines of a script – please report the dataset resulting from the data manipulation, not the original dataset. You must not comment the code script line by line; however, this assignment does test your high-level understanding of a code script.

### Results
- *Key table or figure*. Reproduce the most important table or figure in the paper extracting and commenting the corresponding code – yes, you will need to copy and paste the code from the script into your replication memo. For example, a paper implementing the synthetic control method in STATA will likely be using the *synth* command. Make sure to report and comment the relevant code – and the relevant code only – providing a line-by-line explanation and contextual information. This assignment does not ask you to redo the whole code analysis; yet again, it tests your ability to locate the most important commands in the script. For most papers, you will be extracting one regression table.
Please do not include or screenshot a table (or figure) from the online version of the paper. You must include the table (or figure) from the replication.

## Fair Collaboration
Teams complement the submission with a note breaking down the individual contributions (e.g., student A did X; student B did Y, etc.). The note should also state that "each team member has contributed fairly to the group project" and must go in a footnote or in a *Collaboration* section at the end of the file. This will not count towards the word limit. If contribution has not been fair or balanced, this must be written in place of the fair collaboration clause.
Some students are better at writing and some other students are better at coding or at doing math. This is totally fine. What matters is that everyone contributes her fair share to the project, where the threshold for "fair" has to be agreed upon by the team members. If collaboration falls apart or some team members push the "fair" threshold a little bit too hard, teams should reach to the instructor immediately.