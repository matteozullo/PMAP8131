# Policy Evaluation

## Description

This course teaches the theories and methods of applied social science research. The course blends causal inference and statistical and machine learning providing students with the foundational knowledge to conduct social science research and be considered for applied research scientist positions in the public, private for-profit, and private non-profit sectors.

- **Prerequisites:** ECON 2105, ECON 2106, PMAP 4041, PMAP 4051
- **Course Dates:** August 23rd – December 6th, 2021
- **Class Times:** Mon & Wed at 2:00–3:15 PM
- **Location:** [Aderhold Learning Center (Room 107), 60 Luckie St NW, Atlanta, GA 30303](https://www.google.com/maps/place/Aderhold+Learning+Center/@33.7564192,-84.391006,17z/data=!3m1!4b1!4m5!3m4!1s0x88f503871aed7f0b:0x7739c4923f8b8ca0!8m2!3d33.7564068!4d-84.3888237)

---

## Instructor

- **Name:** Matteo Zullo
- **Affiliations**: [Andrew Young School of Policy Studies](https://aysps.gsu.edu/phd-student/zullo-matteo/), [Georgia Tech's Data Science and Policy Lab](https://datasciencepolicy.gatech.edu/team/)
- **e-mail:** mzullo1@student.gsu.edu
- **Office Hours:** Wed, 3:30-5:00 PM at [AYSPS (3rd floor), 14 Marietta St NW, Atlanta, GA 30303](https://www.google.com/maps/place/Georgia+State+University-Andrew+Young+School+of+Policy+Studies/@33.7544008,-84.3922993,17z/data=!3m1!4b1!4m5!3m4!1s0x88f5038613efe1b9:0x910c3981f9a5cf85!8m2!3d33.7543964!4d-84.3901053)

---

## Syllabus

Please refer to the [Outline](./outline.md) section for information about the class content, meetings, reading assignments, problem sets, and slides.

---

## Grading

The student is graded out of 100 points and 5 more bonus points are available through in-class exercises. Letter grades are assigned as per the table below.

| student_id | year |  SAT | GPA |
|------------|:----:|:----:|:---:|
| 001        |   0  | 1100 | 3.2 |
| 001        |   1  | 1100 | 3.1 |
| 002        |   0  | 1300 | 3.5 |
| 002        |   1  | 1300 | 3.6 |
| 003        |   0  | 1450 | 3.5 |
| 003        |   1  | 1450 | 3.8 |

Total grade is broken down as follows:

* Participation [15\%]
* Individual quizzes [40\%]
* Group mini-projects [40\%]
* Bonus [5\%]


### Participation
At the end of each module, students will post a brief comment note of 200 words or less about the content discussed in the module. Students who wish to further their expertise by looking up research articles that complement the reading assignments are welcomed to do so. Comment notes serve as a checkpoint for learning jointly with the quizzes.

### Quizzes
Quizzes will be issued after the end of each module and must be completed individually through iCollege (solutions will be posted in the [Outline](/outline.md) section of the website). Quizzes are open-book (i.e., consultation of web sources and class notes is allowed) and contain 10 questions each to be completed within 45 minutes. Please note that this is an extremely generous time allocation as students are expected to complete quizzes in abut half-an-hour. At the end of the course, quiz scores will be summed up, aggregated, and curved if average class performance falls below the expected grade of B.

### Mini-Projects
Three mini-projects to be carried out in groups of 3 to 4 are envisioned. The mini-projects are described at length in their dedicated pages and dates are available in the [Outline](/outline.md). Each group member will be awarded the same grade; however, students who wish to complain about group collaboration are encouraged to voice their concerns as early as possible.
 
### Bonus
There will be opportunities for bonus points during the class. Because attendance is required as per institutional policy, bonus points will become available during instructional time.
---

## Policies

### Late Policy
Late work is not in the spirit of the class. A 10\% grade deduction applies to students and groups who submit their work within 24 hours of a deadline, and a 30\% grade deduction applies to submissions coming in anytime after the 24-hour window. Note that the instructor is flexible to change due dates if there is consensus that students and groups might not have enough time to complete any assignment. 

### Issues
Broader issues which affect student performance throughout the class – including and not limited to disability, childcare, and mental health – must be notified to the instructor **at the beginning of the semester**. Late notification of longstanding issues might not be a reason to waive any class requirements.

### Attendance
Class attendance is **required**. Students who experience personal or work-related issues might occasionally skip class meetings. When that happens, students are responsible for sending out an e-mail note to the instructor and encouraged to attend office hours to make up for the material.

### Withdrawal
- Students wishing to withdraw within the official deadline as per the [Academic Calendar](https://registrar.gsu.edu/registration/semester-calendars-exam-schedules/#summer-2022) might do so without receiving a grade of F.
- Students wishing to withdraw past the official deadline might do so in accordance with the [Emergency Withdrawal](https://deanofstudents.gsu.edu/student-assistance/emergency-withdrawal/) policy.

### University
Standard university policies apply to this class. Students might read up on them at:

- [AYSPS Career Services & Student Life Office](https://career.aysps.gsu.edu)
- [Student Code of Conduct](https://codeofconduct.gsu.edu)
- [Policy on Academic Honesty](https://deanofstudents.gsu.edu/student-conductpolicy-on-academic-honesty/)
- [Disability Services](https://access.gsu.edu)



In order to connect your hosted book with your book's source content, you should put your book's source content in a public repository. This section describes one approach to create your own GitHub repository and add your book's content to it.

1. First, log in to GitHub, then go to the "create a new repository" page: <https://github.com/new>

2. Next, give your online repository a name and a description. Make your repository public and do not initialize it with a README file, then click "Create repository".

3. Now, clone the (currently empty) online repository to a location on your local computer. You can do this via the command line with:

   ```bash
   git clone https://github.com/<my-org>/<my-repository-name>
   ```

4. Copy all of your book files and folders into this newly cloned repository. For example, if you created your book locally with `jupyter-book create mylocalbook` and your new repository is called `myonlinebook`, you could do this via the command line with:

   ```bash
   cp -r mylocalbook/* myonlinebook/
   ```

5. Now you need to sync your local and remote (i.e., online) repositories. You can do this with the following commands:

   ```bash
   cd myonlinebook
   git add ./*
   git commit -m "adding my first book!"
   git push
   ```

## Publish your book online with GitHub Pages

We have just pushed the *source files* for our book into our GitHub repository.
This makes it publicly accessible for you or others to see.

Next, we'll publish the *build artifact* of our book online, so that it is rendered as a website.


The easiest way to use GitHub Pages with your built HTML is to use the [`ghp-import`](https://github.com/davisp/ghp-import) package. `ghp-import` is a lightweight Python package that makes it easy to push HTML content to a GitHub repository.

`ghp-import` works by copying *all* of the contents of your built book (i.e., the `_build/html` folder) to a branch of your repository called `gh-pages`, and pushes it to GitHub. The `gh-pages` branch will be created and populated automatically for you by `ghp-import`. To use `ghp-import` to host your book online with GitHub Pages follow the steps below:

```{note}
Before performing the below steps, ensure that HTML has been built for each page of your book
(see {doc}`the previous section <../start/build>`). There should be a collection of HTML
files in your book's `_build/html` folder.
```

1. Install `ghp-import`

   ```bash
   pip install ghp-import
   ```
2. Update the settings for your GitHub pages site:

    a. Use the `gh-pages` branch to host your website.

    b. Choose root directory `/` if you're building the book in it's own repository.
       Choose `/docs` directory if you're building documentation with jupyter-book.

3. From the `main` branch of your book's root directory (which should contain the `_build/html` folder) call `ghp-import` and point it to your HTML files, like so:

   ```bash
   ghp-import -n -p -f _build/html
   ```

```{warning}
Make sure that you included the `-n` - this tells GitHub *not* to build your book with
[Jekyll](https://jekyllrb.com/), which we don't want because our HTML is already built!
If you do not do this you may see **404 not found** for your deployed content.
```

Typically after a few minutes your site should be viewable online at a url such as: `https://<user>.github.io/<myonlinebook>/`. If not, check your repository settings under **Options** -> **GitHub Pages** to ensure that the `gh-pages` branch is configured as the build source for GitHub Pages and/or to find the url address GitHub is building for you.

To update your online book, make changes to your book's content on the `main` branch of your repository, re-build your book with `jupyter-book build mybookname/` and then use `ghp-import -n -p -f mylocalbook/_build/html` as before to push the newly built HTML to the `gh-pages` branch.

```{warning}
Note this warning from the [`ghp-import` GitHub repository](https://github.com/davisp/ghp-import):

"...*`ghp-import` will DESTROY your gh-pages branch... and assumes that the `gh-pages` branch is 100% derivative. You should never edit files in your `gh-pages` branch by hand if you're using this script...*"

