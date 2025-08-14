# Test Plan: Luxor.cz - API Testing

**Product Name:** Luxor (https://www.luxor.cz/)  
**Prepared by:** Tetiana Yachna  
**Date:** 13.05.2025  
**Version:** 1.0  

---

## 1. Objective

This test plan defines the strategy for testing the APIs of the Luxor.cz e-commerce platform.  
The goal is to ensure the backend services related to product browsing, user registration, cart handling, and checkout behave correctly and securely under different conditions.  
This plan is based on a mock Swagger/OpenAPI specification. The endpoints, parameters, and expected responses are assumptions to simulate real-world API testing scenarios.

---

## 2. Test Scope

### In Scope:
- Product search API  
- Product detail API  
- Cart: add/view/remove items  
- User registration and login  
- Checkout endpoint  
- Delivery/payment method endpoints  

### Out of Scope:
- UI or third-party API integrations (e.g. payment gateways, delivery services)  
- Load/performance testing (covered in a separate plan)

---

## 3. Test Types

- **Functional Testing** – Validation of business logic and correct responses  
- **Negative Testing** – Testing with invalid input or unauthorized access  
- **Security Testing** – Token checks, unauthorized access  
- **Contract Testing** – Validate response format using JSON schema  
- **Status Code Testing** – Ensure use of proper HTTP codes (200, 400, 401, 404, 500)

---

## 4. Test Strategy

### 4.1 Test Design Phase:
- Create test scenarios and checklists based on mock Swagger/OpenAPI and UI behavior.  
- Apply formal test design techniques:
  - Equivalence Class Partitioning  
  - Boundary Value Analysis  
  - Decision Table Testing  
  - State Transition Testing  
  - Use Case Testing  
- Use exploratory and error-guessing approaches for edge cases:
  - Malformed JSON, missing headers, invalid tokens  
- Prioritize test cases based on business impact:
  - **P0** – Order placement, checkout, authentication  
  - **P1** – Product search, filtering  
  - **P2** – Optional user data

### 4.2 Test Execution Phase:
- Perform smoke testing on core endpoints  
- Reject unstable builds and wait for a stable environment  
- Execute prioritized test cases and validate:
  - HTTP status codes (200, 400, 401, 404)
  - Response schemas (vs. Swagger)
  - Error messages (language, consistency)  
- Report and track defects in Jira  
- Test types executed:
  - Smoke Testing  
  - Sanity Testing  
  - Regression Testing  
  - Retesting  

### 4.3 Testing Recommendations:
- **Context-Driven Testing:** Adapt to backend/frontend limitations  
- **Exploratory Testing:** Real-world simulation  
- **End-to-End Flow Testing:** Example flow – login → add product → cart → checkout

---

## 5. Test Environment

- **API Base URL:** `https://api.luxor.cz/v1/` *(mock)*  
- **API Documentation:** `https://api.luxor.cz/v1/docs` *(mock Swagger)*  
- **Tools Used:**
  - Postman (test execution and test scripts)
  - Mock Server (simulated backend)
  - JSON Schema Validator plugin  
- **Authentication:** Bearer Token  
- **Test Data:**
  - `ISBN-IN-STOCK-001` – available product  
  - `ISBN-OUT-OF-STOCK-002` – out of stock

---

## 6. Entry Criteria

- API environment is stable and accessible  
- Mock Swagger is available  
- Postman is installed and configured  
- Test data is prepared

---

## 7. Exit Criteria

- All test cases executed  
- All critical/high-priority bugs reported  
- All expected and edge case behavior validated  
- Test summary report delivered

---

## 8. Risks & Mitigation

| Risk                                 | Mitigation                                |
|--------------------------------------|-------------------------------------------|
| No official API docs                 | Use UI behavior, DevTools, mock Swagger   |
| Token expiration                     | Re-authenticate as needed                 |
| API service downtime                 | Use mock server or local test data        |
| Missing test data (e.g., product ID) | Maintain static test user and known ISBNs |
| No access to external systems        | Simulate with stubs or mocks              |
| Non-standard status codes            | Add validation and report to developers   |

---

## 9. Deliverables

- Test Plan (this document)  
- Test Scenarios  
- Test Cases (in Jira)  
- Postman Collection  
- Bug Report  
- Test Summary Report  

---

## 10. Roles and Responsibilities

| Name       | Role                 | Responsibilities                                                     |
|------------|----------------------|----------------------------------------------------------------------|
| Name A     | Test Lead            | Create plan, coordinate testing, defect triage, client communication |
| Name B     | Senior Test Engineer | Design and execute test cases, report defects                        |
| Person C   | Test Engineer        | Execute test cases, validate responses, report issues                |

