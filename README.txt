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

-how do i add/change the picture of my products?
 Locate product-page.html and use this template:
  <div class="product-card">
                <img src="assets/file-name.webp" alt="Product Name" class="product-image">
                <h2 class="product-name">THE MAKEUP LAB COSMETICS</h2>
                <h2 class="product-name">Product Name</h2>
                <p class="product-price">Price</p>
/* Dont change the class element because it is connected to the css file of the product

- How is the background animation handled?
  Through CSS @keyframes bgAnimation applied to the body element

- How do i link another html page and css file?

- How do i open the files without Visual Studio Code?
  Right Click the file then select "open with" then press the application you desire


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






  
