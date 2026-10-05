# Test Plan

---

## Quick Navigation
- [Scope](#scope)
- [Resources](#resources)
- [Approach](#approach)
- [Entry & Exit Criteria](#entry-criteria)
- [Assumptions & Risks](#assumptions)
- [Deliverables](#deliverables)
- [Defect Management](#defect-management)
- [Traceability](#traceability)

---

## Scope
- Authentication
  - Login
  - Registration

- Search
  - Search input
  - Categories

- Product
  - Product details
  - Product selection

- Cart
  - Add product
  - Remove product
  - Quantity
  - Price calculation


## Out of scope
- Payment
- Checkout

---

## Resources

### Test Environment
- Browser: Chrome, Edge;
- OS: Windows 11;
- Application: Allegro Sandbox;
- Screen resolutions: 1920x1080, 1366x768, 1024x768, 768x1024, 390x844, 320x400;

### Test Resources
- QA Tester - Ilkarion
- Test account: test user account
- Test devices: PC

### Test Tools
- Chrome DevTools, Edge DevTools
- Jira
- XRay

---

## Approach
- Functional testing
- Positive and negative testing
- Boundary value analysis
- UI testing
- Responsive testing

---

## Entry Criteria
- Required test data is available
- Application is accessible
- Required test environment is available
- Test accounts can be created
- Main application functionality is accessible   

## Exit Criteria
- All planned test cases have been executed
- Critical and high-severity defects have been reported and reviewed
- Test results have been documented
- Final test summary has been prepared

---

## Assumptions
- The observed application behavior is treated as the primary source of
  expected behavior when formal requirements are unavailable.
- Business rules that cannot be verified are documented as assumptions.
- Test data available in the sandbox environment may differ from production.
- Testing is performed using a regular user account.
- user reached the age of 18

## Risks
- Requirements may be incomplete or unavailable.
- Sandbox behavior may differ from production.
- Third-party services may be unavailable.
- Some functionality may be restricted in the test environment.

---

## Deliverables
- Test Plan
- Test Basis
- Test Scenarios
- Bug Reports
- Test Cases Report
- Test Sets Report
- Test Execution Report
- Traceability Report
---

## Defect Management
Defects will be documented with:

- Title
- Environment
- Preconditions
- Steps to reproduce
- Actual result
- Expected result
- Priority
- Status

---

## Traceability
Requirement -> Test Scenario -> Test Case -> Execution -> Bug
