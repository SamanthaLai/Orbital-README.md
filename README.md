# TWeduElite
# Orbital 2021
## Proposed level of Achievement:
Apollo 11

## Motivation
Back in high school days, both of us felt that aside from going through all the context in textbooks, practising questions is an excellent way to seize each chapter’s main point. However, for talented Taiwanese students who pursue further understanding, it is often time-consuming to find relevant resources with clear explanations and well-designed questions. Therefore, our friends and we have formed a team to ameliorate the situation. We have published several study notes, answers to unanswered problems from each high school and science-related articles. Moreover, we aim to provide a platform for Taiwanese students, parents, and teachers to interact. Most of the resources will be complimentary, but we will charge a small amount for users who wish to access our full notes.

## Aim
Build a website that collaborates with different education-related resources for talented high school students, including practice questions, forum discussion, note sharing, etc.
 
## User core Stories
1. As a visitor, I want to **receive latest information through email**.
2.	As a user viewing this website, I want to clearly know the **function provided** on this platform. 
3.	As a user using this website, I want to **ask questions** and **receive reply** from other users.
4.	As a student **practising questions**, I want to get access to the **answers** and **analyse my answer's preformance**.
5.	As a student checking the **analysing result**, I want to know which part of the knowledge in math/science do I lack of.
6.	As a parent, I want to get complete information of **how to prepare** and know **which school provides science class**.
7.	As a teacher, I want to get **enough questions** for my students to practice. 

## Scope of Project
We wish to build an educational platform with login features--TWeduElite. The platform(website) provides three main features: note sharing, practicing exercises, forum for discussion.

### Features completed by the end of June (milestone 2)
- Log in system
- An email form for users to subscribe
- Latest News
- Study note
- Weekly exercise
- Related links (to other websites related to our platform)
- Forum (only the interface so far)

### Features to be completed by the end of July (milestone 3):
- Before early-July
  - Forum
  - User profile page
- Before mid-July
  - Website styling (colors, font, UI/UX)
- Before the end of July
  - Testing and debugging
  - (If time permits) EXP system
    - Provide a reward system for users to quantify their contribution on forums and articles. 

### UML
[UML](https://app.diagrams.net/?libs=general;uml#G1OzdGA4ugDbxHxd_d0G_qbGyw0AcOdgej)

### Roadblocks of our features / solution we encountered
- User system
  - The default Django user model is not sufficient for us. There are several ways to extend the model, but not all of them can be used in our situation.
  - We choose to add some fields to our extended user model (e.g., wish to get latest news from us via email or not), and add other information to other model (e.g., user picture to profile model)
- Media files will get lost in heroku app
  - This is because the ephemeral design of heroku.
  - We decide to use other saving platform like Amazon S3 or Cloudinary to save the media files.
- Several smaller issues related to Django. Most of them are related to url parameters, models creation and querying and filtering data. They have been solved.

## Feature Limitations/Constraints
We would like to talk about the limitations of our web application that we would like to imrpove in the future. 
1. 
2. Non mobile-user friendly
    Our initial plan was to focus on web design, since **the information can be more readable if shown on website**. We do make some changes to let the mobile-version become more user friendly (eg. conclude expanded navbar options into navbar burger), however, we still suggest users to view our platform through web interface to read the complete information in one page. 
    

## Technology/framework used
- Adobe XD (UI)
- Bulma (CSS Framework)
  - A modern CSS framework base on flexbox.
  - 100% CSS, which implies that it can be used with almost all JS frameworks.
- Vue.JS (frontend)
  - A progressive light-weight JS framework.
- Django (backend)
  - A well-development high level backend framework written in Python.
  - By using Django, we can build our website in an structured way.
- PostgreSQL (database)
- Heroku (Cloud platform)
  - Used to deploy our website.
  - Support Django.
  - It's free plan is sufficient for us.

## Planned testing schedule / detail
- Before early-July
  - Self test the features we have proposed by Django test.
  - We will also test the features by creating an actual account and using all the features.
  - Also, we will discuss with other five team members. They are not part of the orbital team, but we worked together on making/publishing our books for over one year. 
- Before mid-July
  - We will create a google form and provide them to potential users. Our facebook page has over 2,500 subscribers so far, and over 200 users have bought our books. We hope to get sufficient data and suggestions from our customers.
- Before milestone 3
  - We will adjust our website / testing method according to the feedbacks.

## How are we different from similar platforms? 
1. [Snapask](https://snapask.com/zh-tw/) <br />
  Snapask is a educational platform where students can find tutors or where teachers can apply for being tutors. There are also vidoes or online courses about teaching different subjects on it. All of them are chargable. TWEduElite focuses on providing **free information, weekly exercises; only the study note is chargable**. We are not a tutoring platform, we are an **information sharing platform**. 
2. [Super Think](https://superthink.org/) <br />
  Super Think is a platform that also aim for students who are interested to get in science class. They provide chargable notes that include questions and answers. Some of the features are unfunctional, and the UI/UX design is lack of well-organized. TWEduElite provides **forum for users to interact** with each others, and we have **free data analyse** that link to the answer performance from weekly exercise. We are a **quiestion and answer website** for tutors and junior high students. 
3. [Moseley Natural Science](https://www.moseleytw.com/blog/21) <br />
  Moseley Natural Science is a teaching platform that provides sicience teaching videos, practice questions, and advanced knowledge for grade 8 to grade 10 students. TWEduElite is specifically for students who are aiming for getting into science class, users can easily get access to direct information from our website. 
## Program Flow
![program Flow](/programFlow.png)

## Technical Proof of Concept
[Technical Proof of Concept](https://tweduelite.herokuapp.com/)
