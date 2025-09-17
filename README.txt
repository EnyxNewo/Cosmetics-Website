# THE MAKE UP LAB COSMETICS

Notes:

Accounts Storing and Creation FAQ:
- Does this project have a backend (PHP, MySQL, Node.js)?
  No, the current project is front-end only. There is no database languages yet

- Where are accounts stored?
  Accounts are not stored. Login and register pages are static placeholders

- If we want to add real login functionality, what should we do?
  Implement a backend with PHP, Node.js, or another server technology and connect to a database

HTML and File Structure:
- Where is the main entry point of the website?
  login.html

- Where is the login page located?
  login.html with its styles in login-styles.css

- Where do we add new CSS rules?
  Each page has a separate stylesheet, for example main-page-styles.css and login-styles.css

- Where do we put images such as logos and icons?
  Place them inside the assets/ folder

Designing FAQ:
- How do I change the site logo in the header?
  Update the <img src="assets/your-logo.png"> tag in the HTML file

- How do I change the favicon (tab icon)?
  Update <link rel="icon" type="image/png" href="your-logo.png"> in the <head>

- How is the background animation handled?
  Through CSS @keyframes bgAnimation applied to the body element

Responsive Design FAQ:
- Is the website responsive?
  Yes, CSS media queries adjust styles for smaller screens (969px and 768px breakpoints on main page, 400px on login page)

- How can I add new responsive rules?
  Add additional @media queries inside the respective CSS file

Scripts FAQ:
- Where is script.js used?
  Currently script.js is referenced in login.html but incorrectly with <link>. Replace with <script src="script.js"></script>

- Is there any working JavaScript yet?
  No, script.js is empty. Add logic there if needed

Programming FAQ:
- Which IDEs can be used?
  Any text editor or IDE like VS Code, IntelliJ, or Notepad++

- How do I run the website?
  Open the HTML files directly in a browser or use a local server (Live Server extension in VS Code is recommended)

- What should I do before editing CSS?
  Check if the style is inside the correct stylesheet (main-page-styles.css, login-styles.css, etc.)

- What if I want to add new pages?
  Create a new HTML file, link its CSS, and update the header navigation links

- The logo or icons are not showing
  Check that the image file is inside the assets/ folder and the file path matches in HTML

- Styles are not applied
  Verify that the correct CSS file is linked in the HTML head using <link rel="stylesheet" href="filename.css">

- Background animation is not moving
  Ensure the CSS includes @keyframes bgAnimation and body has animation applied

- Website looks broken on mobile
  Check if you edited inside the right @media query. For small screens, review max-width: 969px, 768px, or 400px rules

- Hover effects not working
 Try to Confirm the class names in HTML match the CSS selectors exactly

- Page shows blank or errors
  Ensure all HTML tags are properly opened and closed, and no missing > or quotation marks
- Styles not showing
  Check if register-page-styles.css is correctly linked in <head>

- Gradient animation not moving
  Ensure @keyframes bgAnimation is defined at bottom of CSS

- Button hover not showing gradient
  Replace background-color with background in button[type="submit"]:hover

- Link to login not working
  Confirm that login.html exists in the same directory

- Form not submitting data
  Expected, since there is no backend. Needs PHP, Node.js, or API endpoint to store user data

Known Issues / Notes
--------------------
- Form action points to main.html but there is no backend handling (placeholder only)
- Password and confirm password fields are independent; no client-side validation yet
- Button hover effect uses background-color: linear-gradient which is invalid
  Should use background: linear-gradient instead
- No logo is included in HTML even though .logo class exists in CSS
  Add <img class="logo" src="assets/logo.png"> inside .register-container if needed



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

CSS STRUCTURE
- body
  Sets global font, text color, animated gradient background, centers login container, removes default margin

- .header
  Styles optional header section with bottom margin and centered text

- .logo
  User icon with fixed width, centered, drop-shadow effect, and hover scaling

- .login-container
  Glassmorphic container with blur effect, border, rounded corners, padding, and hover lift effect

- .input-group
  Wrapper for form inputs with spacing, font size adjustment, and alignment

- .input-group input
  Styles inputs with white text, semi-transparent background, border, padding, rounded corners, and hover focus effects

- .input-group input[type="checkbox"]
  Styles checkbox size and hover scaling

- .input-group label
  Styles checkbox label with smaller font and pointer cursor

- button[type="submit"]
  Gradient button with padding, rounded corners, bold text, shadow, and hover scale effect

- .register, .forgot
  Styles links with smaller font, light color, and hover color change

- @keyframes submit
  Fade and slide animation applied when the login container loads

- @keyframes bgAnimation
  Moves background gradient left to right continuously

- @media (max-width: 400px)
  Makes login container, logo, inputs, and button smaller for mobile screens

Documentation for register-page.html
- Main container
  <div class="register-container"> wraps the entire form and message

- Title
  <h1>Register</h1> for page heading

- Form
  <form action="main.html" method="post"> sends input data to main.html (currently placeholder, no backend)

- Input fields
  Username, Email, Password, Confirm Password
  All are required inputs with placeholder text

- Submit button
  <button type="submit"><strong>Register</strong></button> styled with gradient and hover effect

- Link to login page
  <a class="login" href="login.html">Log-in here</a>

CSS Structure:
- Body
  Uses linear-gradient background with animated movement (@keyframes bgAnimation)
  Centers container using flexbox
  Font: Arial

- Container (.register-container)
  Semi-transparent blurred box (backdrop-filter: blur)
  Animated entrance (@keyframes submit)
  Hover: lifts slightly (translateY)

- Input groups (.input-group)
  Margin spacing around inputs
  Inputs styled with semi-transparent background and white text
  Focus effect adds glowing border and box shadow
  Hover effect enlarges slightly

- Checkbox styles
  Supports input[type="checkbox"] with scaling hover effect and small label font

- Submit button
  Gradient background, white text, rounded corners, shadow
  Hover: scales up and changes gradient

- Login link (.login)
  Light gray text, hover becomes white

- Animations
  @keyframes submit handles fade-in + upward slide
  @keyframes bgAnimation animates gradient background

Responsive Design:
- Breakpoint at max-width: 400px
  Container shrinks to 90% width with smaller padding
  Logo shrinks to 80px
  Inputs and button font-size reduced for mobile


Documentation for main-page.html and main-page-styles.css

HTML Structure:
- Header container
  <div class="main-header"> wraps everything

- Header content
  <div class="header-design-contents1"> fixed header bar

- Logo
  <img src="assets/test-logo.png" class="header-logo"> placed inside header

- Navigation links
  - <a href="main-page.html" class="header-home-button"> HOME </a>
  - <a href="" class="header-category-dropdown"> CATEGORY </a>
  - <a href="" class="header-products-button"> PRODUCTS </a>

CSS Structure:
- Body
  Gradient background with @keyframes bgAnimation for animated color shift
  Centered layout with flexbox (note: header is fixed so body centering is less visible)

- Header container (.header-design-contents1)
  Fixed position at top, full width
  Height: 100px (shrinks in mobile view)
  Background color: #f33c8b
  Flexbox used to align children

- Logo (.header-logo)
  Size: 60px wide, circular (border-radius: 100%)
  Drop shadow applied
  Hover: slight scale + rotation
  Positioned using margin-left and margin-right

- Navigation buttons
  .header-home-button, .header-category-dropdown, .header-products-button
  Small font size (10px by default)
  White text, rounded pill background on hover
  Positioned absolutely with left: % values
  Hover: background turns white, text becomes pink

- Animations
  @keyframes bgAnimation animates background gradient
  @keyframes hoverAnim is defined but not applied anywhere

Responsive Design:
- Breakpoint at max-width: 400px
  - Header height reduced to 80px
  - Logo size remains 60px but shifts margin-right
  - Buttons shrink font-size to 4px and padding smaller
  - Home and Category buttons aligned further left







  
