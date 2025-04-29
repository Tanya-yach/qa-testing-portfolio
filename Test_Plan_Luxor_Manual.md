# Test Plan: Luxor.cz – Manual Testing

**Product Name:** Luxor (https://www.luxor.cz/)  
**Prepared by:** Tetiana Yachna  
**Date:** 15.04.2025

---

## 1. Objective
This test plan outlines the approach for manual testing of the Luxor.cz e-commerce website (bookstore).
The goal is to verify that all critical functionalities work as expected. Ensure that all UI elements are displayed correctly across browsers/devices. Identify and report bugs or inconsistencies.

---

## 2. Test Scope

### In Scope:
- Homepage & navigation
- Search & product filtering
- Shopping cart & checkout
- User account (registration, login, profile management)
- Responsive layout (mobile/tablet/desktop)
- Basic UI/UX checks

### Out of Scope:
- Payment gateway integration (payment gateways in sandbox mode)
- Backend database validation
- Third-party API integrations

---

## 3. Test Types

| Test Type            | Focus Area                       | Techniques                           |
|----------------------|----------------------------------|--------------------------------------|
| Functional           | Forms, buttons, navigation       | Positive/Negative testing            |
| UI/UX                | Layout, responsiveness, access.  | Visual inspection, DevTools          |
| Cross-browser testing| Chrome, Firefox, Safari          | Manual verification                  |
| Cross-device testing | Desktop, tablet, mobile          | Visual inspection, real devices      |

---

## 4. Test Strategy

### 1. Test Design Phase:
- Creation of Test Scenarios and Test Cases (Checklists) using:
  - Equivalence Class Partitioning
  - Boundary Value Analysis
  - Decision Table Testing
  - State Transition Testing
  - Use Case Testing
- Experience-based techniques:
  - Error Guessing
  - Exploratory Testing
- Prioritization:
  - **P0**: Checkout, payments, search
  - **P1**: User accounts, reviews, wishlists
  - **P2**: Minor UI elements

### 2. Test Execution Phase:
- Smoke Testing
- Full Functional Testing
- Logging and reporting defects
- Types of testing:
  - Smoke Testing
  - Sanity Testing
  - Regression Testing
  - Usability/UI Testing
  - Retesting
- End-to-End Flow Testing
- Context-Driven Testing

---

## 5. Test Environment
- **Website:** https://www.luxor.cz
- **Devices:** Desktop (1920x1080), Tablet (768x1024), Mobile (375x667)
- **OS:** Windows, macOS
- **Browsers:** Chrome (latest), Firefox (latest), Safari
- **Test Data:**
  - Valid user: `test_user@gmail.com` / `Password123!`
  - ISBN-IN-STOCK-001 (available)
  - ISBN-OUT-OF-STOCK-002 (not available)

---

## 6. Entry Criteria
- Website is accessible and stable
- Test data is prepared
- Test documentation is ready
- Major features deployed

---

## 7. Exit Criteria
- All planned manual tests executed
- All critical/high-priority bugs reported
- Major regressions addressed
- Test Summary Report shared

---

## 8. Risks & Mitigation

| Risk                                           | Mitigation                                                             |
|------------------------------------------------|------------------------------------------------------------------------|
| Frequent changes on prod site                  | Frequent regression/smoke tests                                        |
| Third-party service failures                   | Use sandbox and tag as external                                        |
| Dynamic content (book stock)                   | Use static ISBNs                                                       |
| No payment gateway                             | Mock payment step                                                      |
| Resource unavailability                        | Assign backup testers                                                  |
| Build URL not working                          | Pause or use alternative environments                                  |
| Less time for testing                          | Ramp up resources dynamically                                          |

---

## 9. Deliverables
- Test Plan (this document)
- Test Scenarios
- Test Cases (Jira)
- Checklists
- Bug Reports
- Test Summary Report

---

## 10. Roles and Responsibilities

| Name      | Role                   | Responsibilities                                                                 |
|-----------|------------------------|----------------------------------------------------------------------------------|
| Name A    | Test Lead              | Create plan, coordinate execution, verify defects, communicate with client       |
| Name B    | Senior Test Engineer   | Write and execute test cases, report defects                                     |
| Person C  | Test Engineer          | Execute test cases, report defects                                               |

