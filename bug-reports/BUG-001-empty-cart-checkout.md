BUG-001 — Application Allows Checkout and Order Completion with an Empty Cart
Defect Information
Field	Details
Defect ID	BUG-001
Title	Application Allows Checkout and Order Completion with an Empty Cart
Related Test Case	TC-028
Module	Cart / Checkout
Severity	High
Priority	High
Status	Open
Test Type	Manual Functional / Negative Testing
Environment	SauceDemo Web Application
Browser	Google Chrome
Preconditions
User is logged in using a valid SauceDemo account.
Shopping cart initially contains a product.
Steps to Reproduce
Log in to SauceDemo using a valid standard user account.
Add any product to the shopping cart.
Open the shopping cart.
Remove the product so that the cart becomes empty.
Click Checkout, if available.
Enter a valid First Name.
Enter a valid Last Name.
Enter a valid ZIP Code.
Click Continue.
Click Finish.
Expected Result

The application should prevent the user from proceeding with checkout when the shopping cart is empty.

An order should not be created or completed without at least one product in the cart.

Actual Result

The application allows the user to proceed through checkout with an empty cart.

The user can enter valid checkout information, continue to the order summary, click Finish, and reach the "Thank you for your order!" confirmation page even though no product is in the cart.

Impact

This defect allows an invalid order to be completed without any products.

If present in a production e-commerce system, this could result in invalid business transactions, incorrect order records, and potential downstream processing issues.

Severity and Priority

Severity: High

The defect affects a core business workflow and allows an invalid transaction to be completed.

Priority: High

The issue should be addressed before production release because it affects order processing.

Evidence

Screenshot/video evidence: To be added.

Recommendation

The application should prevent checkout when the cart contains zero products.

The Checkout action should either be disabled/hidden for an empty cart or the application should display an appropriate validation message and prevent the user from proceeding.

Related Test Result

TC-028 — Checkout with Empty Cart: FAIL

This defect was identified during negative testing of the shopping cart and checkout workflow.