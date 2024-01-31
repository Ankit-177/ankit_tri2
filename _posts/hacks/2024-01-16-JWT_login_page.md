---
toc: false
comments: true
layout: post
title: JWT Login
description: Mini login system using JWT.
type: hacks
courses: { compsci: {week: 7} }
---

<html>
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>JWT Authentication</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f4f4f4;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      margin: 0;
    }
    .auth-container {
      background-color: #fff;
      padding: 20px;
      border-radius: 8px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
    input {
      width: 100%;
      padding: 10px;
      margin: 8px 0;
      box-sizing: border-box;
    }
    button {
      width: 100%;
      padding: 10px;
      background-color: #3498db;
      color: #fff;
      border: none;
      border-radius: 4px;
      cursor: pointer;
    }
    button:hover {
      background-color: #2980b9;
    }
  </style>
</head>
<body>
  <div class="auth-container" id="signup-container">
    <h2>Sign Up</h2>
    <form id="signup-form">
      <label for="signup-username">Username:</label>
      <input type="text" id="signup-username" name="signup-username" required>
      <label for="signup-password">Password:</label>
      <input type="password" id="signup-password" name="signup-password" required>
      <button type="button" onclick="attemptSignup()">Sign Up</button>
    </form>
  </div>

  <div class="auth-container" id="login-container" style="display: none;">
    <h2>Login</h2>
    <form id="login-form">
      <label for="login-username">Username:</label>
      <input type="text" id="login-username" name="login-username" required>
      <label for="login-password">Password:</label>
      <input type="password" id="login-password" name="login-password" required>
      <button type="button" onclick="attemptLogin()">Login</button>
    </form>
  </div>

  <script>
    function attemptSignup() {
      const signupUsername = document.getElementById("signup-username").value;
      const signupPassword = document.getElementById("signup-password").value;

      // Make an HTTP request to your backend for signup
      // Example using fetch API
      fetch('http://127.0.0.1:8086/api/users/authenticate', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({ username: signupUsername, password: signupPassword }),
      })
      .then(response => response.json())
      .then(data => {
        if (data.success) {
          // Signup successful
          alert('Account created successfully! Now you can log in.');
          // Show the login container and hide the signup container
          document.getElementById("signup-container").style.display = "none";
          document.getElementById("login-container").style.display = "block";
        } else {
          // Signup failed
          alert('Signup failed. Please try again.');
        }
      })
      .catch(error => {
        console.error('Error:', error);
      });
    }

    function attemptLogin() {
      const loginUsername = document.getElementById("login-username").value;
      const loginPassword = document.getElementById("login-password").value;

      // Make an HTTP request to your backend for authentication
      // Example using fetch API
      fetch('your-backend-api-url/login', {
        method: 'POST',
        headers: {
          'Content-Type': 'application/json',
        },
        body: JSON.stringify({ username: loginUsername, password: loginPassword }),
      })
      .then(response => response.json())
      .then(data => {
        if (data.token) {
          // Authentication successful
          alert('Login successful!');
          // You can store the token in localStorage or a secure way for future requests
        } else {
          // Authentication failed
          alert('Login failed. Please check your credentials.');
        }
      })
      .catch(error => {
        console.error('Error:', error);
      });
    }
  </script>
</body>
</html>