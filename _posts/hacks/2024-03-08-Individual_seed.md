---
toc: false
comments: true
layout: post
title: Individual seed
description: Summary of individual work thus far; justification for 100% seed.
type: tangibles
courses: { compsci: {week: 13} }
permalink: /plans/week1
---

## Justification for 100% (3.0/3.0) seed based on individual work:

- I achieved above a 93% last trimester:
![alt text](<../../images/AP CSP - Trimester 2 grade - Ankit.png>)

## Contributions to team:
- As a group, only 2 of our members were active contributors. The other 2 members were completely inactive and did not contrinute to the success of the project much. However, as an individual, I rallied us together and pushed for active contribution every day leading up to the presentation of the CPT project. In many instances, I called for meetings in order to set definite tasks for every person in the group. In terms of the CPT project, I created the sign up and login features along with adding a new `email` parameter to our SQLite database. This allows users to enter their email address while creating an account, allowing the application to store the email to be constantly used in the application process for each college. Additionally, I created the welcome page that greeted the users upon visiting the website and allowed them to navigate to the login page. I also created the error pages that redirected the user to the appropriate error page when using the wrong login credentials or trying to navigate to a non-existent subpage.

## Task organization and set ideals as a team:
- I created the project ideation issue and the team agile manifesto, which are linked in the project issues below:
[CollegeApp Scout issues](https://github.com/Ankit-177/cpt_project/issues)

### Below are my key commits from the CPT project:
[Website login and sign up feature implementation along with menu, home page, and personalized application tracker page](https://github.com/Ankit-177/cpt_project/commit/03562415d09fb96b0c3c3aea12ca2cc8919b0106)<br><br>
[Edit and delete user functionalities for admin](https://github.com/Ankit-177/cpt_project/commit/c1d6bdc69b2af05c3287120d50e1cb25c3ef471c#diff-d2405490b89e560cdcbc1abe42af7a0de13941d6bc4e1e9213e2597511001bdd)<br><br>
[user.py customization, auth_middleware.py addition, and major init.py and model users.py changes](https://github.com/Ankit-177/cpt_backend/commit/f523a154e59dd4405ff32ca20ba42b4e770d0c33)<br><br>
[Admin role implementation in backend](https://github.com/Ankit-177/cpt_backend/commit/2c2d735be850f8dbc2ec6f608e2389069e24373f)

## Github analytics - Proof of project contribution:
![alt text](<../../images/AP CSP - Github analytics overall - Ankit.png>)
![alt text](<../../images/AP CSP - Github analytics personal - Ankit.png>)

## Learnings and notes from CB MCQ:
- <mark>Binary bits</mark>: A bit is the smallest unit of data that a computer can process and store. A bit state is represented using 1s and 0s as each bit is always in one of two physical states. Usually, all 8 bits are used. However, in some cases, not all bits are required, as seen in Q49:
![Alt text](<../../images/AP CSP - Q49 mistake - Ankit.png>)

- <mark>Internet Protocol (IPv6)</mark>: The Internet Protocol (IP) is a protocol, or set of rules, for routing and addressing packets of data so that they can travel across networks and arrive at the correct destination. IPv6 is the most recent version of Internet Protocol (IP). It's designed to supply IP addressing and additional security to support the predicted growth of connected devices in IoT, manufacturing, and emerging areas like autonomous driving.

- <mark>Algorithm run-times</mark>: We can categorize the run time of an algorithm according to how the number of steps increases as the input size increases. According to CollegeBoard, accessing elements `2n` times, or `2` times per element, is considered reasonable run-time. Also, accessing elements `n^2` times, or `n` times per element, is considered reasonable run-time. This is seen in Q50, which I got wrong:
![Alt text](<../../images/AP CSP - Q50 mistake - Ankit.png>)

### Final score for CB MCQ:
![Alt text](<../../images/AP CSP - CB MCQ 2020 score - Ankit.png>)