# Template Repository

CSGE602022 - Web Design & Programming (Perancangan & Pemrograman Web) @
Faculty of Computer Science Universitas Indonesia, Odd Semester 2018/2019

Modified from : https://gitlab.com/PPW-2017/ppw-lab

* * *

## Table of Contents

Welcome to the code repository.
This repository hosts weekly tutorial codes and other, such as course-related
code snippets.

1. [Quickstart Guide](#tldr)

## TL;DR

1. Clone this repository  (`git clone https://github.com/agasyan/ppw18-template`)
2. Ensure that your repository page has visibility level set to
**Internal** or **Public**. Check it in **Edit Project** menu at
your repository page.

Working on a story problem set:

1. Create new apps on Django Project based on your story `python manage.py startapp [bla-bla]` 
2. Do the exercises as instructed in story.
3. Commit your work frequently
4. Write good commit message(s)
5. If your work is ready for grading: `git push origin master`

If you want to know the detailed explanation about each instructions above,
please read the following sections.

## Doing the Story

1. Suppose that you want to work on Story 4 problem set. Go to the
story 4 to read the instructions.
2. To ensure your work regarding Story 4 problem is isolated from
your other attempts on other problems, create a new apps
specifically for working on Story 4 problem. Use Python command:
`python manage.py startapp story_4`
3. Read the Story carefully because It contains set of tasks and instructions that you can work on.
4. Do the tutorial.
5. Use `git add` or `git rm` to stage/unstage files that you want to
save into Git later.
6. Once you want to save your progress, commit your work to Git. Use
Git command: `git commit` A text editor will appear where you should
write a commit message. Please try to follow the guidelines written
in [this guide](http://chris.beams.io/posts/git-commit/) on how to
write a good commit message.
7. Repeat steps 4 - 6 until you finish the tutorial.
8. Once you are ready to submit your work or you want to save it to
your repository on GitLab, do a Git **push**. The Git command: 
`git push origin master`


## Show Code Coverage in Gitlab

1. Go to Pipeline Settings (`Settings -> Pipelines`)
2. Go to section Coverage Settings (`Pipelines -> Test coverage parsing`)
3. Write this Regex (Regular Expression) in textbox `Test Coverage Parsing` 

    > TOTAL\s+\d+\s+\d+\s+(\d+)%

4. Now your pipelines page will show your Code Coverage

## Grading Scheme & Demonstration

Weekly tutorials contribute **20%** to the final grade of this course.
For each exercises, student can obtain grade ranging from **A (4)** to
**E (0)**. The grading scheme is as follows and divided to small parts on 
each story:

1. **A** (75 - 100) if student achieve **the story is done perfectly**
2. **B** (50 - 75) if student completed **the story is done well**
3. **C** (25 - 50) if student completed **the story only implemented knowledge learned in class**
4. **D** (0 - 25) if student completed **Minimum story done**

All students required to demonstrate their work to teaching assistant with PDF on SCeLe.

### Happy Coding :)

## 1st Installation

1. Create a **virtual environment** for this tutorial by using this command:

    ```bash
    python -m venv env
    ```
    
    > Make sure that you executed the command in the root path of the repository.
2. Activate your virtual environment and install required packages. Note that
the command for activating virtual environment is different on Windows and
Unix-based OS.

    Windows:
    
    ```bash
    env\Scripts\activate.bat
    pip install -r requirements.txt
    ```

    Linux & Mac OS:

    ```bash
    source env/bin/activate
    pip install -r requirements.txt
    ```
3. Use your favourite editor to edit the code (Vim, VS Code, Atom) or use IDE (PyCharm).

4. When you are done with your tutorial or you want to switch to another
Python project, do not forget to deactivate your virtual environment. You
can do so by executing:

    ```bash
    deactivate
    ```
    
