# Test Plan

---

## Scope
- Authetication(login, registration)
- Search(filters, search input, by categories)
- Product
- Cart
- Performance

## Out of scope
- Payment
- Checkout

---

##Resources

### Test Environment
- Browser: Chrome, Edge;
- OS: Windows 11;
- Application: Allegro Sandbox;
- Screen resolutions: 1920x1080, 1366x768, 1024x768, 768x1024, 390x844, 320x400;

### Test Resources
- QA Tester - Ilkarion
- Test account: mastercomponents6@gmail.com
- Test devices: PC

### Test Tools
- Chrome DevTools, Edge Devtools
- Jira
- XRay
- Postman
- JMeter

---

## Approach
- Functional testing
- Positive and negative testing
- Boundary value analysis
- Exploratory testing
- UI testing
- Responsive testing
- API testing

---

## Entry Criteria
- Application is accessible
- Required test environment is available
- Test accounts can be created
- Main application functionality is accessible   

## Exit Criteria
- All planned test cases have been executed
- Critical and high-severity defects have been reported
- Test results have been documented
- Final test summary has been prepared


---

## Assumptions
- The observed application behavior is treated as the primary source of
  expected behavior when formal requirements are unavailable.
- Business rules that cannot be verified are documented as assumptions.
- Test data available in the sandbox environment may differ from production.

## Risks
- Requirements may be incomplete or unavailable.
- Sandbox behavior may differ from production.
- Third-party services may be unavailable.
- Some functionality may be restricted in the test environment.
- API availability may change during testing.

---

## Deliverables
- Test Plan
- Test Basis
- Test Scenarios
- Test Cases
- Exploratory Testing Sessions
- Bug Reports
- Postman API Collection
- Responsive Testing Results
- Test Execution Report
- Final Test Summary

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
Requirement
    ↓
Test Scenario
    ↓
Test Case
    ↓
Execution
    ↓
Bug
