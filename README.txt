# THE MAKE UP LAB COSMETICS

Notes:

-There are no currently Javascript, mySQL, PHP, and other backend languages so there are currently no databases for your accounts, ordering processes, and security processes

-The starting page is login-page.html

- To change your logo in your website:
    - Go to the "assets" folder or /asset and put your logo there then name it however you want
    - Open any IDE's / Integrated Development Environment, Notepad, Notepad++, or any text editor
    - find the tag " <img src=assets/test-logo.png" alt="Test Logo" class=test-logo>" You can change their name to your likings /* Dont forget to add " to every attributes */

- To change your logo in your tab
     - Go to the "assets" folder or /asset and put your logo there then name it however you want
    - Open any IDE's / Integrated Development Environment, Notepad, Notepad++, or any text editor
    - find the tag "<link rel="icon" type="image/png" href="test-logo.png"> " You can change their name to your likings


Documentation for login.html:

login.html Documentation
------------------------

- <!DOCTYPE html>
  Declares the document type as HTML5

- <html lang="en">
  Root element of the page with English language

- <head>
  Contains metadata and links for styling and icons

- <meta charset="UTF-8">
  Sets character encoding to UTF-8

- <meta name="viewport" content="width=device-width, initial-scale=1.0">
  Ensures the page is responsive on all devices

- <link rel="stylesheet" href="login-styles.css">
  Links external CSS file for styling

- <link rel="script" href="script.js">
  Incorrect usage, script files should be linked with <script> not <link>

- <link rel="icon" type="image/png" href="your-logo.png">
  Sets the tab icon to a PNG image

- <title>Log-in</title>
  Defines the page title shown in browser tabs

- <body>
  Contains all visible content of the page

- <div class="login-container">
  Main container that holds the login form and its content

- <img src="assets/user.png" alt="User Icon" class="logo">
  User icon displayed at the top of the login box

- <h1>Login</h1>
  Page heading

- <form action="main-page.html" method="post">
  Login form that redirects to main-page.html after submission

- <div class="input-group">
  Wrapper for input fields such as email, password, and checkbox

- <input type="text" id="username" name="username" placeholder="E-mail" required>
  Input for the user email

- <input type="password" id="password" name="password" placeholder="Password" required>
  Input for the user password

- <input type="checkbox" id="remember-me" name="remember-me">
  Checkbox to remember user login

- <label for="remember-me">Remember me</label>
  Label for the remember me checkbox

- <a class="forgot" href="notice.html">Forgot password?</a>
  Link to forgot password page

- <button type="submit"><strong>Login</strong></button>
  Submit button for login
  
