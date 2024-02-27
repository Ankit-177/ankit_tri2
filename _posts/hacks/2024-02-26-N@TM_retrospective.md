---
toc: false
comments: true
layout: post
title: CSP Final - N@TM Retrospective and Final Project Review
description: Project task completion summary along with a video link
type: tangibles
courses: { compsci: {week: 12} }
permalink: /plans/week1
---

# Project Summary:
- Considering the difficulty of the college application process, we have created an app that allows students to organize their application progress to ensure efficiency and ease of access. Our CPT project is an application that allows users to create their own, personalized accounts and login using the same credentials to track their application progress from a variety of colleges stored in our database.

# My Features:
- I created the sign up and login features along with adding a new `email` parameter to our SQLite database. This allows users to enter their email address while creating an account, allowing the application to store the email to be constantly used in the application process for each college. Additionally, I created the welcome page that greeted the users upon visiting the website and allowed them to navigate to the login page. I also created the error pages that redirected the user to the appropriate error page when using the wrong login credentials or trying to navigate to a non-existent subpage.

**[Click here for CollegeBoard requirements document (Both components A and B)](https://apcentral.collegeboard.org/media/pdf/ap-csp-student-task-directions.pdf)**

<br>

# CollegeBoard Requirements:

## Component A
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CollegeBoard requirements summary: Component A</title>
    <style>
       table {
    width: 120%;
    border-collapse: collapse;
    margin-top: 20px;
    }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>CB Requirement</th>
                <th>Fulfillment</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Instructions for input from one of the following: the user, a device, an online datas stream, a file</td>
                <td>Our project includes a login feature that prompts the user to enter the correct credentials in order to access their personalized college application tracking page. Furthermore, we also have a sign up feature that allows the user to input their name, username, password, date of birth, and email.  
                <img src="/ankit_tri2/images/AP CSP - Login page image - Ankit.png" alt="Login page">
                <img src="/ankit_tri2/images/AP CSP - Sign up page image - Ankit.png" alt="Sign up page">
                </td>
            </tr>
            <tr>
                <td>Use of at least one list (or other collection type) to represent a collection of data that is stored and used to manage program complexity and help fulfill the users purpose</td>
                <td>For storing user data, we used an SQLite database that stores user information in the following paramters: `id`, `name`, `uid` or username, `password`, `dob`, and `email`.
                <img src="/ankit_tri2/images/AP CSP - SQLite database image - Ankit.png" alt="SQLite database">
                </td>
            </tr>
            <tr>
                <td>At least one procedure that contributed to the program’s intended purpose where you have defined: the name, return type, one or more parameters</td>
                <td> The following procedure checks for the validity of the login information (obtained from the backend using a `fetch` function) and allows the user to login and access their college application tracker. It also redirects users to the specific error pages based on different error cases.
                <img src="/ankit_tri2/images/AP CSP - Fetch function image - Ankit.png" alt="Fetch function">
                </td>
            </tr>
            <tr>
                <td>An algorithm that includes sequencing, selection, and iteration that is in the body of the selected procedure
                </td>
                <td> The code snippet below is from our user.py API file. For the user deletion feature, which is exclusive to the Admin role, the code iterates through the list of users retrieved from the database. If a user's 'uid' matches the 'uid' obtained from the request payload, it deletes that user. After the deletion loop, it attempts to return a JSON response containing the details of the deleted user.
                <img src="/ankit_tri2/images/AP CSP - Iteration image 2 - Ankit.png" alt="Iteration">
                </td>
            </tr>
            <tr>
                <td>Calls to your student-developed procedure</td>
                <td> This code uses the GET request to read and extract all the users and their corresponding information from our database in order to be used in the frontend database viewer.
                <img src="/ankit_tri2/images/AP CSP - GET method image - Ankit.png" alt="GET method">
                </td>
            </tr>
            <tr>
                <td>Instructions for output (tactile, audible, visual, or) based on input and program functionality</td>
                <td> This code fetches the corresponding college list based on the user making the request. It uses the `/edit` endpoint in our user.py API.
                <img src="/ankit_tri2/images/AP CSP - Output image - Ankit.png" alt="Output">
                </td>
            </tr>
        </tbody>
    </table>
</body>
</html>

<br>

## Component B
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CollegeBoard requirements summary: Component B</title>
    <style>
       table {
    width: 120%;
    border-collapse: collapse;
    margin-top: 20px;
    }
    </style>
</head>
<body>
    <table>
        <thead>
            <tr>
                <th>CB Requirement</th>
                <th>Fulfillment</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>Input to your program</td>
                <td> - </td>
            </tr>
            <tr>
                <td>At least one aspect of the functionality of your program</td>
                <td> - </td>
            </tr>
            <tr>
                <td>Output produced by your program</td>
                <td> - </td>
            </tr>
            <tr>
                <td>DOES NOT contain any distinguishing information about yourself</td>
                <td> - </td>
            </tr>
            <tr>
                <td>DOES NOT contain voice narration (though text captions are encouraged)</td>
                <td> - </td>
            </tr>
            <tr>
                <td>Video is either .webm, .mp4, .wmv, .avi, or .mov format</td>
                <td> - </td>
            </tr>
            <tr>
                <td>Video is no more than 1 minute in length</td>
                <td> - </td>
            </tr>
            <tr>
                <td>Video is no more than 30MB file size</td>
                <td> - </td>
            </tr>
        </tbody>
    </table>
</body>
</html>

<br>

# Key Commits:
[Website login and sign up feature implementation along with menu, home page, and personalized application tracker page](https://github.com/Ankit-177/cpt_project/commit/03562415d09fb96b0c3c3aea12ca2cc8919b0106)<br><br>
[Edit and delete user functionalities for admin](https://github.com/Ankit-177/cpt_project/commit/c1d6bdc69b2af05c3287120d50e1cb25c3ef471c#diff-d2405490b89e560cdcbc1abe42af7a0de13941d6bc4e1e9213e2597511001bdd)<br><br>
[user.py customization, auth_middleware.py addition, and major init.py and model users.py changes](https://github.com/Ankit-177/cpt_backend/commit/f523a154e59dd4405ff32ca20ba42b4e770d0c33)<br><br>
[Admin role implementation in backend](https://github.com/Ankit-177/cpt_backend/commit/2c2d735be850f8dbc2ec6f608e2389069e24373f)


