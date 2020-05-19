---
layout: page
title: Syllabus
catalog: BIO 316
credits: 3
semester: Summer 2020
professor: Dr. Robert Harbert (he/him)
office: Zoom 
email: rharbert@stonehill.edu
phone: 508-565-1248
schedule: Work at your own pace
location: Online
office_hours: TBA
office_hours_location: Zoom
TA: NA
TA_email: NA
---

# eSyllabus

**Official course syllabus posted on eLearn**

## Course

{{ site.title }}

{{ page.catalog }}, {{ page.credits }} Credits, {{ page.semester }}

### Instructor

{{ page.professor }}

Office: {{ page.office }}

Email (best way to contact us):
[{{ page.email }}](mailto:{{ page.email }})

Phone: {{ page.phone }}


### Location

{{location}}


### Times

{% for class in page.schedule %}
  {{ class }}
{% endfor %}


### Office Hours

Times: {{ page.office_hours }}

Location: {{ page.office_hours_location }}

Or by appointment. *Note: scheduling alternate appointments can be made by email or through Calendly link on eLearn*

### Teaching Assistant

{{ page.TA }}

Email: [{{ page.TA_email }}](mailto:{{ page.TA_email }})


### Website

The syllabus and other relevant class information and resources will be posted
at [{{ site.url}}]({{ site.baseurl }}/).
Changes to the schedule may be posted to this site so please try to check it
periodically for updates.


### Course Communications

Email: [{{ page.email }}](mailto:{{ page.email }})


### Required Texts

There is no required text book for this class.

All needed material is openly available on the course website. If you are
interested in additional reading on the topics we are covering I highly
recommend [R for Data Science](https://r4ds.had.co.nz/), which is freely
available on the web.


### Course Description

An introduction to data management, manipulation, and analysis, with an emphasis
on biological problems. Class consists of short introductions to new concepts
followed by hands on computing exercises using R and SQLite, but the concepts
apply to programming languages and databases more generally. No background in
computing is required.


### Prerequisite Knowledge and Skills

Knowledge of basic biology to provide context for exercises.


### Purpose of Course

In this course you will learn all of the fundamental aspects of computer
programming that are necessary for conducting biological research. By the end of
the course you will be able to use these tools to import data into R, perform
analysis on that data, and export the results to graphs, text files, and
databases. By learning how to get the computer to do your work for you, you will
be able to do more science faster.


### Course Objectives and Goals

Students completing this course will be able to:

* Create well structured databases
* Extract information from databases
* Write computer programs in R
* Automate data analysis
* Apply these tools to address biological questions
* Apply general data management and analysis concepts to other programming
  languages and database management systems


### Teaching Philosophy

This class is taught using a flipped, learner-centered, approach, because
learning to program and work with data requires actively working on
computers. Flipped classes work well for all kinds of content, but I think they
work particularly well for computer oriented classes. 

### Instructional Methods

As a flipped classroom, students are provided with either reading or video
material that they are expected to view/read on their own. While students are 
working on exercises the instructor will be available to actively engage with 
students to help them understand material they find confusing, explain 
misunderstandings and help identify mistakes that are preventing students from 
completing the exercises, and discuss novel applications and alternative approaches 
to the data analysis challenges students are attempting to solve. For more challenging topics class may start with 20-30 minute demonstrations on the concepts followed by time to work on exercises.


## Course Policies

### Make-up policy

Life happens and therefore there is an automatic grace period of 48 hours for
the submission of late assignments with no need to request an extension.
However, it is highly recommended that you submit assignments on time when
possible because assignments build on one another and it can be hard to catch up
if you fall behind. Reasonable requests for longer extensions will also be granted.
Assignments turned in after the 48 hour grace period without an extension will be
be graded with a 20% penalty.


### Assignment policy

Assignments are due Wednesday night by 11:59 pm Eastern Time. Assignments should be
submitted via eLearn. This timing allows you to finish with one week's assignment as a new week of material is released (on Tuesdays).


### Course Technology

Students are required to provide their own laptops and to install free and open
source software on those laptops (see [Setup]({{ site.baseurl }}/computer-setup)
for installation instructions). Support will be provided by the instructor in
the installation of required software. If you don't have access to a laptop
please contact the instructor and they will do their best to provide you with
one.


## Grading Policies

Grading for this course is based on 13 equally weighted assignments.

Exercises in assignments will be graded as follows:

* Produces the correct answer using the requested approach: 100%
* Generally uses the right approach, but a minor mistake results in an incorrect
    answer: 90%
* Attempts to solve the problem and makes some progress using the core concept:
    50%
* Answer demonstrates a lack of understanding of the core concept: 0%


### Grading scale

- **A 92.5-100**
- **A- 90-92.4**
- **B+ 87.5-89.9**
- **B 82.5-87.4**
- **B- 80-82.4**
- **C+ 77.5-79.9**
- **C 72.5-77.4**
- **C- 70-72.4**
- **D 60-69.9**
- **F <60**

## Course Schedule

The details course schedule is available on the course website at:
[{{ site.url }}/schedule]({{ site.baseurl }}/schedule).

