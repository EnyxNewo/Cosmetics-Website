## THE MAKE UP LAB COSMETICS

## Notes:

## Accounts Storing and Creation FAQ:
- Does this project have a backend (PHP, MySQL, Node.js)?  
No, the current project is front-end only. There is no database languages yet

- Where are accounts stored?
Accounts are not stored. Login and register pages are static placeholders

- If we want to add real login functionality, what should we do?
  Implement a backend with PHP, Node.js, or another server technology and connect to a database

## HTML and File Structure FAQ:
- Where is the main entry point of the website?
  login.html

- Where is the login page located?
  -login.html with its styles in login-styles.css

- Where do we add new CSS rules?
  Each page has a separate stylesheet, for example main-page-styles.css and login-styles.css

- Where do we put images such as logos and icons?
  Place them inside the assets/ folder

## Designing FAQ:
- How do I change the site logo in the header?
  Update the `<img src="assets/your-logo.png">` tag in the HTML file

- How do I change the favicon (tab icon)?
  Update `<link rel="icon" type="image/png" href="your-logo.png">` in the <head>

-how do i add/change the picture of my products?
 Locate product-page.html and use this template:
  `<div class="product-card">`
                `<img src="assets/file-name.webp" alt="Product Name" class="product-image">`
                `<h2 class="product-name">THE MAKEUP LAB COSMETICS</h2>`
                `<h2 class="product-name">Product Name</h2>`
                `<p class="product-price">Price</p>`
/* Dont change the class element because it is connected to the css file of the product

- How is the background animation handled?
  Through CSS @keyframes bgAnimation applied to the body element

- How do i link another html page and css file?       Use the tag `<link rel="stylesheet" href="stylename.css">`

- How do i open the files without Visual Studio Code?
  Right Click the file then select "open with" then press the application you desire


## Responsive Design FAQ:
- Is the website responsive?
  Yes, CSS media queries adjust styles for smaller screens (969px and 768px breakpoints on main page, 400px on login page)

- How can I add new responsive rules?
  Add additional @media queries inside the respective CSS file

##Scripts FAQ:

- Is there any working JavaScript yet?
  No, script.js is empty. Add logic there if needed

## Programming FAQ:
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
  Verify that the correct CSS file is linked in the HTML head using '<link rel="stylesheet" href="filename.css">'

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
  Replace background-color with background in `button[type="submit"]:hover`

- Link to login not working
  Confirm that login.html exists in the same directory

- Form not submitting data
  Expected, since there is no backend. Needs PHP, Node.js, or API endpoint to store user data
  
- Form action points to main.html but there is no backend handling (placeholder only)
   Password and confirm password fields are independent; no client-side validation yet


## Notes from the developer
- This project is **frontend only**.  
- No JavaScript, PHP, MySQL, or other backend technologies are included.  
- All forms (Login, Register) are static and do not connect to a database.  
- Navigation is handled with **HTML links**.  
- CSS files are used for styling, responsiveness, and animations.  
- Assets (logos, icons, product images) should be placed inside the **assets/** folder.  



## Documentation of Files:

### login.html
- Provides the login page.  
- Elements:  
  - `<img class="logo">` for the user icon.  
  - `<h1>` title "Login".  
  - `<form>` with `username`, `password`, and `remember me` checkbox.  
  - `<a class="forgot">` link for password recovery.  
  - `<button>` to log in.  
  - `<p>` with `<a class="register">` link to registration page.  
- Redirects to `main-page.html` on submit.  
- Uses `login-styles.css`.  

### login-styles.css
- Styles the login form and its elements.  
- Elements:  
  - `body`  gradient animated background, centered container.  
  - `.logo`  resizable logo with hover transform.  
  - `.login-container`  blurred box container with hover effect.  
  - `.input-group`  styled input fields with hover and focus effects.  
  - `input[type="checkbox"]`  custom checkbox scaling on hover.  
  - `button[type="submit"]`  gradient button with hover scaling.  
  - `.register, .forgot`  links with hover color change.  
- Includes `@keyframes submit` and `@keyframes bgAnimation`.  
- Responsive rules for screen width under 400px.  

### register-page.html
- Provides the registration form.  
- Elements:  
  - `<h1>` title "Register".  
  - `<form>` with inputs: username, email, password, confirm password.  
  - `<button>` to register.  
  - `<p>` with `<a class="login">` link to login page.  
- Redirects to `main.html` on submit.  
- Uses `register-page-styles.css`.  

### register-page-styles.css
- Styles the registration form and its elements.  
- Elements:  
  - `body` animated gradient background, centered container.  
  - `.register-container`  blurred box container with hover effect.  
  - `.input-group`  styled input fields with hover/focus glow.  
  - `input[type="checkbox"]`  checkbox support (not in HTML yet).  
  - `button[type="submit"]`  gradient register button with hover scaling.  
  - `.login`  link to login page with hover color change.  
- Includes `@keyframes submit` and `@keyframes bgAnimation`.  
- Responsive rules for screen width under 400px.  

### main-page.html
- Main homepage.  
- Elements:  
  - `<div class="main-header">` containing:  
    - `<img class="header-logo">` for the logo.  
    - `<a class="header-home-button"> HOME </a>`  
    - `<a class="header-category-dropdown"> CATEGORY </a>`  
    - `<a class="header-products-button"> PRODUCTS </a>`  
- Links to `main-page-styles.css`.  

### main-page-styles.css
- Styles the homepage and header.  
- Elements:  
  - `body`  gradient background with animation, centered.  
  - `.header-design-contents1`  fixed header bar with pink background.  
  - `.header-logo`  circular logo with hover animation.  
  - `.header-home-button`, `.header-category-dropdown`, `.header-products-button`  styled navigation links with hover background color.  
- Includes `@keyframes hoverAnim` and `@keyframes bgAnimation`.  
- Responsive rules for screen width under 400px.  

### notice.html
- Placeholder page.  
- Elements:  
  - Same `<div class="main-header">` header as `main-page.html`.  
  - `<h1>` centered message: “THIS PAGE IS STILL UNDER DEVELOPMENT.”  

### products-page.html
- Product listing page.  
- Elements:  
  - Same header as `main-page.html`.  
  - `<div class="product-card">` blocks containing:  
    - `<img>` product image.  
    - `<h2 class="product-name">` product name.  
    - `<p class="product-price">` product price.  
- Uses `products-page-styles.css`.  

### products-page-styles.css
- Styles product listings.  
- Elements:  
  - `.product-grid`  grid layout for products.  
  - `.product-card`  product container with shadow hover effect.  
  - `.product-name`  product title styling.  
  - `.product-price`  price styling.  
- Responsive rules adjust grid to 2 columns (tablets) and 1 column (mobile).  


## Limitations
- No real login, registration, or shopping cart system (frontend only).  
- No dropdowns or interactivity without JavaScript.  
- Not secure for production use until backend is implemented.  

---

## Developer Notes
- CSS animations and responsive design included.  
- Extendable with JavaScript or backend later.  







  
