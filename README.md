Web Application Manual Testing
Project Overview

This project demonstrates a structured manual software testing process performed on the SauceDemo web application.

The project covers requirements analysis, test planning, test scenario creation, test case design, functional and negative testing, test execution, defect reporting, and end-to-end validation.

Application Under Test

Application: SauceDemo
Testing Type: Manual Web Application Testing
Primary Focus: Functional, Negative, Regression, and End-to-End Testing

Testing Scope

The following areas were tested:

User Login and Authentication
Product Listing
Product Details
Shopping Cart
Add/Remove Products
Checkout Information
Order Summary
Order Completion
Order Confirmation
Logout
Navigation
Cart Validation
Order Total Calculation
Test Execution Summary
Metric	Result
Total Test Cases	30
Passed	29
Failed	1
Pass Rate	96.7%
Defects Identified	1
High-Severity Defects	1
Defect Identified
BUG-001 — Checkout Allowed with an Empty Cart

During negative testing, a defect was identified where the application allowed a user to proceed through checkout and complete an order even when the shopping cart contained no products.

Severity: High
Priority: High
Status: Open

Detailed defect information is available in:

bug-reports/BUG-001-empty-cart-checkout.md

Testing Activities
Requirements Analysis
Reviewed application functionality and identified testable requirements.
Defined testing scope and expected application behavior.
Test Planning
Created a structured test plan.
Defined testing objectives, scope, and test approach.
Test Scenario Design
Created scenarios covering major application workflows.
Included positive and negative testing conditions.
Test Case Design
Designed 30 functional test cases.
Documented preconditions, test steps, expected results, and priorities.
Test Execution
Executed all 30 test cases manually.
Recorded PASS and FAIL results.
Verified expected versus actual behavior.
Defect Reporting
Documented the failed test case as BUG-001.
Included reproduction steps, expected result, actual result, severity, priority, and impact.
End-to-End Testing
Validated the complete shopping workflow from login through order confirmation.
Project Structure
web-application-manual-testing/
│
├── requirements/
│   └── requirements.md
│
├── test-plan/
│   └── test-plan.md
│
├── test-scenarios/
│   └── test-scenarios.md
│
├── test-cases/
│   ├── test-cases.md
│   └── defects.md
│
├── test-execution/
│   └── test-execution-results.md
│
├── bug-reports/
│   └── BUG-001-empty-cart-checkout.md
│
├── exploratory-testing/
│
└── regression-testing/
Tools & Technologies
Manual Web Application Testing
Chrome Browser
Git
GitHub
Markdown
SauceDemo
Testing Techniques
Functional Testing
Positive Testing
Negative Testing
Regression Testing
End-to-End Testing
Boundary/Validation Testing
UI Testing
Defect Reporting
Test Case Design
Test Execution
Key Results
Designed and executed 30 manual test cases.
Achieved a 96.7% test pass rate.
Identified and documented 1 high-severity defect.
Validated the complete purchase workflow.
Verified checkout calculations and cart behavior.
Documented the complete testing lifecycle from requirements through defect reporting.
Conclusion

This project demonstrates practical experience with the software testing lifecycle, including test planning, test design, execution, defect identification, and reporting. It also demonstrates the ability to organize QA documentation and use Git/GitHub to maintain testing artifacts.
