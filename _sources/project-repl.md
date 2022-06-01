# Project II

## Checklist

- You will be turning the items below. You probably want to use Microsoft Word for your write-up but really any text editor (e.g., Pages) and markup language (e.g., LateX) is fair game. Adherence to the [APA style guidelines](https://apastyle.apa.org) is encouraged.
- **Introduction** [25%]: research question(s), statistical technique(s).
- **Methodology** [25%]: model, variables, data.
- **Results** [50%]: key table or figure.

## Structure
In this assignment, you will be replicating the findings of an empirical research article in the social sciences. Any social science research article (psychology, sociology, economics, public policy, etc.) published in a peer-reviewed journal is fair game. You can find papers with code online from sources such as the [Harvard Dataverse](https://dataverse.harvard.edu/dataverse/RepData) or the [Replication Wiki](https://replication.uni-goettingen.de).
The article must implement one of the statistical methods covered in the class (e.g., difference-in-differences, synthetic control, neural networks, etc.). Any other advanced methodologies which have not been presented in class are also fair game. However, you might not choose articles that implement basic statistical techniques (e.g., descriptive statistics, linear regression, logistic regression, etc.). The other requirements are quite loose; however, you ideally want to find an article that:
- Has been published in the last two decades;
- Implements a code routine in one or more programming languages (Python, R, STATA, etc.).
- Includes a data submission. Some papers would use publicly available data sources which might be downloaded for free from the web. If this is the case of your article, please make sure to download the data and include it in your submission. 

Replicating a paper is running the analysis from beginning to end using the code and data provided in the authors' submission. You will need to:
- Read the paper and understand the research question it addresses;
- Download all the replication materials;
- Install the relevant software and packages on your machine. Note that version requirements are often an issue for reproducibility. At times, authors reference the package versions used for analysis (e.g., R version 3.6). Version compatibility is one of the reasons why you want to start early. Trust me, running the code without errors means you are at least halfway through completing the assignment.
- Rerun the code line by line.
- Save all the outputs from analysis.

To complete the assignment, you will need to turn in a replication memo, which includes the parts below.

### Introduction 
Here, you introduce the:
- *(Main) research question*. The causal relationship that the paper is looking at. You typically want to express the research question in terms of dependent and independent variables.
- *Statistical or machine learning technique*. Name the technique used for identification of the causal effect. Include information about the identification conditions. For example, regression discontinuity requires that the running variable is discontinuous around the cutoff. The authors would need to have said something about it. Note any other details that are relevant for understanding.

### Methodology
Here, you discuss the:
- *Model*. Rewrite the empirical model – yes, this means you will need to rewrite the regression equation or the other math used in the original paper – walking the reader through the different variables and parameters. Discuss the functional form, the structure of the error term, the coding of the variables. Make sure to distinguish between dependent variable, control variables, and key explanatory variable(s).
- *Data*. Generate a toy example of the data with all the variables and their coding. This can be done via screenshot (not recommended), in Excel (recommended), or using the other software of your choosing (also recommended). If the script recodes, reshapes, and reformats the dataset included in the submission – this is typically the content of the first few lines of a script – please report the dataset which results from manipulation, not the original dataset. While I don't want you to understand and comment a code script line by line; this assignment tests your high-level understanding of a script. Ability to locate variable manipulations is integral to this skillset.

### Results
- *Key table or figure*. Reproduce the most important table or figure in the paper extracting and commenting the corresponding code – yes, you will need to copy and paste the code the paper from the script into your replication memo. For example, a paper implementing the synthetic control method in STATA will likely be using the *synth* command followed by the relevant call. Make sure to report and comment the code line by line providing contextual information. This assignment does not ask you to redo and comment the whole code analysis; however, it tests your ability to locate the most important command from a script. For most empirical papers, you will be extracting one regression table.
Please do not include or screenshot a table or figure from the online version of the paper. You need to include the table and figure that your replication of the paper generates on your machine.


## Fair Collaboration
Teams will complement each submission with a note breaking down individual contributions to the project (e.g., student A did X; student B did Y, etc.). The note should also state that "each team member has contributed fairly to the group project" and must go in a footnote or in a *Collaboration* section at the end of the file which will not count towards the word limit. If contribution has not been fair or balanced, this must be written in place of the fair collaboration clause.
It is expected that some students will go the extra mile because of their interest in the project, and that some students who are better at writing will be contributing more to the write-up and less to the model. This is totally fine. What matters is that everyone brings her fair contribution to the project, where the threshold for "fair" has to be aggreed upon by the team members. If collaboration falls apart or some team members are pushing the "fair" hreshold too hard, teams should reach to the instructor as soon as possible.