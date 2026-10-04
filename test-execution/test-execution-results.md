Test Execution Results
Project Information

Project: Web Application Manual Testing
Application: SauceDemo
Test Type: Manual Functional Testing
Environment: Chrome Browser
Test Execution: Completed

Execution Summary
Metric	Result
Total Test Cases	30
Passed	29
Failed	1
Pass Rate	96.7%
Test Case Results
Test Case ID	Test Case	Status
TC-001	Valid Login	PASS
TC-002	Invalid Login	PASS
TC-003	Locked-Out User Login	PASS
TC-004	Login with Empty Username	PASS
TC-005	Login with Empty Password	PASS
TC-006	Login with Empty Username and Password	PASS
TC-007	Product Listing Display	PASS
TC-008	Product Details Display	PASS
TC-009	Add Product to Cart	PASS
TC-010	Remove Product from Cart	PASS
TC-011	Valid Checkout Information	PASS
TC-012	Checkout with Missing First Name	PASS
TC-013	Checkout with Missing Last Name	PASS
TC-014	Checkout with Missing ZIP Code	PASS
TC-015	Checkout with All Fields Empty	PASS
TC-016	Order Summary Display	PASS
TC-017	Product Appears in Order Summary	PASS
TC-018	Complete Order	PASS
TC-019	Order Confirmation	PASS
TC-020	Logout	PASS
TC-021	Continue Shopping from Cart	PASS
TC-022	Remove Product from Cart	PASS
TC-023	Cart Count Updates After Removing Product	PASS
TC-024	Add Multiple Products to Cart	PASS
TC-025	Remove All Products from Cart	PASS
TC-026	Back Navigation from Checkout	PASS
TC-027	Back Navigation from Order Summary	PASS
TC-028	Checkout with Empty Cart	FAIL
TC-029	Verify Order Total Calculation	PASS
TC-030	Complete Purchase Flow	PASS
Failed Test Case
TC-028 — Checkout with Empty Cart

Status: FAIL

Expected Result:
The application should prevent the user from proceeding with checkout when the cart is empty.

Actual Result:
The application allowed checkout and order completion with an empty cart and displayed the order confirmation.

Related Defect: BUG-001

Defect Summary
Defect ID	Description	Severity	Priority	Status
BUG-001	Application allows checkout and order completion with an empty cart	High	High	Open
Overall Result

The test execution achieved a 96.7% pass rate, with 29 of 30 test cases passing. One high-severity defect was identified during negative testing involving checkout with an empty cart.