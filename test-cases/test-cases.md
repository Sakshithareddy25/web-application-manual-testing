Manual Test Cases
Test Case Format

Each test case contains a unique ID, objective, precondition, test steps, expected result, and priority.

Authentication
TC-001 — Valid Login

Priority: High

Precondition: User is on the SauceDemo login page.

Steps:

Enter a valid username.
Enter a valid password.
Click Login.

Expected Result: User is successfully logged in and redirected to the Products page.

TC-002 — Invalid Login

Priority: High

Precondition: User is on the login page.

Steps:

Enter an invalid username.
Enter an invalid password.
Click Login.

Expected Result: An appropriate login error message is displayed and the user remains on the login page.

TC-003 — Locked-Out User Login

Priority: High

Precondition: User is on the login page.

Steps:

Enter the locked-out user credentials.
Click Login.

Expected Result: Login is prevented and an appropriate error message is displayed.

TC-004 — Empty Username

Priority: Medium

Steps:

Leave the username field empty.
Enter a valid password.
Click Login.

Expected Result: A validation message indicates that the username is required.

TC-005 — Empty Password

Priority: Medium

Steps:

Enter a valid username.
Leave the password field empty.
Click Login.

Expected Result: A validation message indicates that the password is required.

TC-006 — Empty Username and Password

Priority: Medium

Steps:

Leave username empty.
Leave password empty.
Click Login.

Expected Result: A validation message is displayed indicating required login information.

TC-007 — Logout

Priority: High

Precondition: User is logged in.

Steps:

Open the application menu.
Click Logout.

Expected Result: User is logged out and returned to the login page.

Product Functionality
TC-008 — Product Listing Display

Priority: High

Precondition: User is successfully logged in.

Steps:

Navigate to the Products page.
Review the available products.

Expected Result: Products are displayed with relevant information such as name, price, and image.

TC-009 — Product Details

Priority: Medium

Precondition: User is on the Products page.

Steps:

Select a product.
Open the product details page.

Expected Result: The selected product's name, description, price, and image are displayed correctly.

TC-010 — Add Product to Cart

Priority: High

Precondition: User is logged in and on the Products page.

Steps:

Select a product.
Click Add to cart.
Open the cart.

Expected Result: The selected product appears in the cart and the cart count is updated.

TC-011 — Remove Product from Cart

Priority: High

Precondition: A product is available in the cart.

Steps:

Open the cart.
Click Remove for the selected product.

Expected Result: The product is removed from the cart and the cart count is updated.

TC-012 — Add Multiple Products

Priority: High

Precondition: User is logged in.

Steps:

Add multiple products to the cart.
Open the cart.

Expected Result: All selected products appear in the cart and the cart count reflects the number of selected products.

Shopping Cart
TC-013 — Cart Displays Selected Products

Priority: High

Precondition: At least one product has been added to the cart.

Steps:

Open the cart.
Review the listed products.

Expected Result: All selected products are displayed correctly.

TC-014 — Cart Count After Adding Product

Priority: Medium

Steps:

Add a product to the cart.
Observe the cart icon.

Expected Result: The cart count increases accordingly.

TC-015 — Cart Count After Removing Product

Priority: Medium

Precondition: At least one product is in the cart.

Steps:

Open the cart.
Remove a product.
Observe the cart icon.

Expected Result: The cart count decreases accordingly.

TC-016 — Remove All Products

Priority: High

Precondition: Multiple products are in the cart.

Steps:

Open the cart.
Remove each product.

Expected Result: All products are removed and the cart becomes empty.

TC-017 — Continue Shopping

Priority: Medium

Precondition: User is on the cart page.

Steps:

Click Continue Shopping.

Expected Result: User is returned to the Products page.

TC-018 — Empty Cart Handling

Priority: High

Precondition: Cart contains no products.

Steps:

Open the cart.
Review the page.

Expected Result: The cart displays no products and the application handles the empty state correctly.

Checkout
TC-019 — Valid Checkout Information

Priority: High

Precondition: At least one product is in the cart.

Steps:

Open the cart.
Click Checkout.
Enter a valid first name.
Enter a valid last name.
Enter a valid ZIP code.
Click Continue.

Expected Result: User proceeds to the order summary page.

TC-020 — Missing First Name

Priority: High

Steps:

Proceed to checkout.
Leave First Name empty.
Enter valid Last Name and ZIP Code.
Click Continue.

Expected Result: A validation message indicates that First Name is required.

TC-021 — Missing Last Name

Priority: High

Steps:

Proceed to checkout.
Enter valid First Name.
Leave Last Name empty.
Enter valid ZIP Code.
Click Continue.

Expected Result: A validation message indicates that Last Name is required.

TC-022 — Missing ZIP Code

Priority: High

Steps:

Proceed to checkout.
Enter valid First Name and Last Name.
Leave ZIP Code empty.
Click Continue.

Expected Result: A validation message indicates that ZIP Code is required.

TC-023 — All Checkout Fields Empty

Priority: High

Steps:

Proceed to checkout.
Leave First Name, Last Name, and ZIP Code empty.
Click Continue.

Expected Result: A validation message is displayed and the user cannot continue.

TC-024 — Back/Cancel from Checkout

Priority: Medium

Precondition: User is on the checkout information page.

Steps:

Click Cancel.

Expected Result: User is returned to the previous page without completing the order.

TC-025 — Checkout with Empty Cart

Priority: High

Precondition: Cart contains no products.

Steps:

Open an empty cart.
Click Checkout, if available.
Enter valid checkout information if the application allows access.
Continue through the checkout process.

Expected Result: The application should prevent checkout and order completion when the cart is empty.

Order Processing

TC-026 — Back Navigation from Checkout

Priority: Medium

Precondition: User has at least one product in the cart and is on the Checkout Information page.

Steps:

Open the cart.
Click Checkout.
On the Checkout Information page, click Cancel.

Expected Result: User is returned to the Cart page without completing the order.

TC-027 — Back Navigation from Order Summary

Priority: Medium

Precondition: User has at least one product in the cart and has entered valid checkout information.

Steps:

Open the cart.
Click Checkout.
Enter valid First Name, Last Name, and ZIP Code.
Click Continue.
On the Order Summary page, click Cancel.

Expected Result: User is returned to the Products page without completing the order.

TC-028 — Checkout with Empty Cart

Priority: High

Precondition: User is logged in and the shopping cart is empty.

Steps:

Add any product to the cart.
Open the cart.
Remove the product so the cart becomes empty.
Click Checkout, if available.
Enter valid First Name, Last Name, and ZIP Code if the application allows access.
Click Continue.
Click Finish if the application allows the user to proceed.

Expected Result: The application should prevent checkout and should not allow an order to be completed when the cart is empty.

Actual Result: The application allowed checkout and order completion with an empty cart.

Status: FAIL

Related Defect: BUG-001

TC-029 — Verify Order Total Calculation

Priority: High

Precondition: User has at least one product in the cart.

Steps:

Add one or more products to the cart.
Open the cart.
Click Checkout.
Enter valid checkout information.
Click Continue.
Review the order summary.
Verify the item subtotal, tax, and total.

Expected Result: The subtotal, tax, and final order total are calculated and displayed correctly based on the selected products.

Status: PASS

TC-030 — Complete Purchase Flow

Priority: Critical

Precondition: User has valid SauceDemo credentials.

Steps:

Log in with valid credentials.
Select a product.
Add the product to the cart.
Open the cart.
Click Checkout.
Enter valid First Name, Last Name, and ZIP Code.
Click Continue.
Review the order summary.
Click Finish.

Expected Result: The purchase is successfully completed and the order confirmation page is displayed.

Status: PASS