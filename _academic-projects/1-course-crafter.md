---
title: "Class Planner and Recommender Website"
excerpt: "CourseCrafter is a full-stack web application designed as a class schedule organizing and recommendation tool. It offers dynamic academic planning with a user-friendly drag-and-drop interface and an integrated course rating system.<br/><a href='https://youtu.be/k9qI0a95mTM?si=KmedxhRdMtFJmpFa'><img src='/images/course_crafter.jpg'></a>"
permalink: /projects/course-crafter
collection: academic-projects
---


In Notre Dame's [Database Systems](https://timweninger.com/teaching/database-systems-concepts/) (CSE 30246) course, I worked in a group of three to develop CourseCrafter, a tool designed for class schedule organization and recommendation. This application helps users to construct their academic plans, accommodating various majors, minors, and concentrations. Its key feature is the real-time update of course prerequisites, corequisites, and credit requirements, which adds a dynamic aspect to academic planning. CourseCrafter also supports saving multiple schedules.

We integrated two main features into CourseCrafter: a user-friendly Schedule Planner with a drag-and-drop interface, and a Course Ratings system for users to rate and review classes. The Schedule Planner allows for straightforward organization of courses, while the Course Ratings system utilizes SQL queries to average ratings and compile common course statistics.

One of our main challenges was importing class data into a MySQL database. We tackled this by scraping data from a university registrar's website using Python and Selenium, incorporating error handling techniques to manage data inconsistencies.

CourseCrafter was initially deployed on Heroku, featuring a React/Next.js frontend and a Flask backend, with the MySQL database hosted on AWS. 

Currently, the website not operational due to cost factors. However, the project’s code is available on GitHub: [frontend code](https://github.com/johnflanagan827/course-crafter-frontend) and [backend code](https://github.com/johnflanagan827/course-crafter-backend). Additionally, for a more comprehensive understanding of CourseCrafter, a video tutorial can be viewed by clicking on the image below.


<a href='https://youtu.be/k9qI0a95mTM?si=KmedxhRdMtFJmpFa'><img src='/images/course_crafter_large.jpg'></a>