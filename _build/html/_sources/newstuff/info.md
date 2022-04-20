# Policy Evaluation

This course teaches the theories and methods of policy evaluation integrating quantitative and qualitative skills. Thus, it provides students with the foundational knowledge to be considered for policy analysis positions in the public, private for-profit, and private non-profit sectors.

- **Prerequisites:** ECON 2105, ECON 2106, PMAP 4041, PMAP 4051
- **Course Dates:** August 23rd – December 6th, 2021
- **Class Times:** Mon & Wed at 2:00–3:15 PM
- **Location:** [Aderhold Learning Center (Room 107), 60 Luckie St NW, Atlanta, GA 30303](https://www.google.com/maps/place/Aderhold+Learning+Center/@33.7564192,-84.391006,17z/data=!3m1!4b1!4m5!3m4!1s0x88f503871aed7f0b:0x7739c4923f8b8ca0!8m2!3d33.7564068!4d-84.3888237)

---

## Syllabus

Please refer to the [Outline](./outline.md) section for information around the class content, class meetings, reading assignments, and assignments.

---

## Grading

The student is graded out of 100 points and 5 more bonus points are available through in-class exercises. Letter grades are assigned as per the table below.

|--------------------|--------------|--------------|-------------|
| A+ (98-100)        | B+ (88-89.9) | C+ (78-78.9) | D (60-69.9) |
| A (93-97.9)        | B (83-87.9)  | C (73-77.9)  | F (0-59.9)  |
| A- (90-92.9)       | B- (80.82.9) | C- (70-72.9) |             |



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









## Description



---

## Instructor

- **Name:** Matteo Zullo
- **Affiliations**: [Andrew Young School of Policy Studies](https://aysps.gsu.edu/phd-student/zullo-matteo/), [Georgia Tech's Data Science and Policy Lab](https://datasciencepolicy.gatech.edu/team/)
- **e-mail:** mzullo1@student.gsu.edu
- **Office Hours:** Wed, 3:30-5:00 PM at [AYSPS (3rd floor), 14 Marietta St NW, Atlanta, GA 30303](https://www.google.com/maps/place/Georgia+State+University-Andrew+Young+School+of+Policy+Studies/@33.7544008,-84.3922993,17z/data=!3m1!4b1!4m5!3m4!1s0x88f5038613efe1b9:0x910c3981f9a5cf85!8m2!3d33.7543964!4d-84.3901053)

---






Total grade is broken down as follows:

* Participation [25 pts.]
* Quizzes [25 pts.]
* Project [50 pts.]
* Bonus [2.5 pts.]

### Participation
At the end of each module, students will post a brief comment note of 200 words or less to any of the articles referenced in the [Outline](/outline.md). Therefore, students must identify a reading of their interest, go through it, and submit their note through the participation forum in iCollege. This approach uses the light touch to give undergraduate students some exposure to top-notch academic materials which are most often parts of graduate courses. Students will be awarded full credits for turning in the comments.

### Quizzes
Five quizzes will be issued during the semester and must be completed through iCollege (solutions will be posted in the [Schedule](/schedule.md) section of the website). Quizzes are open-book (i.e., consultation of web sources and class notes is allowed) and contain 10 questions each to be completed within 45 minutes. Please note that this is an extremely generous time allocation and expected time for completion is about half-an-hour. At the end of the course, quiz scores will be totaled up and curved if average class performance falls below the expected grade of B.<br>
Occasionally, students might encounter terminology which they are not really familiar with. That is why quizzes have been opened up for consultation of web sources and use of class notes. Policy analysts often grapple with domains that they have little knowledge of, but they are able to learn quickly and effectively.

### Project
Please refer to the [Project](/project.md) section for more information. The project consists of a policy report to be completed in teams of three to four. Each group member will be awarded the same grade, however students who wish to complain about their group collaboration are encouraged to voice their concerns as early as possible. Also, a "Fair Collaboration" clause ensures ongoing committment of all team members.

### Bonus
In-class exercise will be conducted in the same groups that will complete the group project. The team ranking first overall will be awarded 2.5 points at the end of the course (i.e., each group member will add 2.5 bonus points to her total grade). There might be more opportunities for bonus points throughout the semester.

---

## Policies

### Late Policy
Late work is not in the spirit of the class and is **wholeheartedly discouraged** but no late policy applies. Students who fail to meet deadlines must follow-up on their late submissions with an e-mail note providing a justification for the delay.

### Issues
Broader issues which affect student performance throughout the semester – including and not limited to disability, childcare, and mental health – must be notified to the instructor **at the beginning of the semester**. Late notifications of longstanding issues might not be a reason to waive any class requirements.

### Attendance
Class attendance is **required**. Students who experience personal or work-related issues might occasionally skip class meetings. When that happens, students are reponsible for sending out an e-mail note to the instructor and encouraged to attend office hours to make up for the material.

### Withdrawal
- Students wishing to withdraw within the official deadline as per the [Academic Calendar](https://registrar.gsu.edu/registration/semester-calendars-exam-schedules/#fall-2021) might do so without receiving a grade of F.
- Students wishing to withdraw past the official deadline might do so in accordance with the [Emergency Withdrawal](https://deanofstudents.gsu.edu/student-assistance/emergency-withdrawal/) policy.

### University
Standard university policies apply to this class. Students might read up on them at:

- [AYSPS Career Services & Student Life Office](https://career.aysps.gsu.edu)
- [Student Code of Conduct](https://codeofconduct.gsu.edu)
- [Policy on Academic Honesty](https://deanofstudents.gsu.edu/student-conductpolicy-on-academic-honesty/)
- [Disability Services](https://access.gsu.edu)
```