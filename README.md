# QA Testing Portfolio – Tetiana Yachna

Welcome to my testing portfolio! This repository showcases my work in software quality assurance across various testing disciplines.
The main goal is to simulate real QA tasks and showcase the skills required for a Software Development Engineer in Test role.

--- 

## Repository Structure

### 📂 manual-testing-luxor
Manual testing project based on the real e-commerce website **[Luxor.cz](https://www.luxor.cz/)**.  
Includes test documentation for functional and UI testing. All bug reports are fictional and created for demonstration purposes.
Artifacts for web testing:
- Test Plan (`test-plan.md`)
- Test Scenarios (`test-scenarios.md`)
- Test Cases (`test-cases.md`)
- Checklists (`checklist.md`)
- Bug Reports (`bug-report.md`)

---

### 📂 api-testing-luxor (Mock API)
Since there is no public API for **[Luxor.cz](https://www.luxor.cz/)**, all endpoints were designed based on assumptions and simulated using a **Postman Mock Server**.
API testing artifacts:
- Test Plan (`test-plan-api.md`)
- Test Cases (`test-cases-api.md`)
- Postman Collection (`postman-collection-api.json`) with pre-configured mock examples
- Bug Reports (`bug-report-api.md`)

---

### 📂 api-testing-restful_booker (Data-Driver Testing)
This project includes automated API tests using [RESTful Booker API](https://restful-booker.herokuapp.com/).
API testing artifacts:
- Postman Collection (`restful_booker-postman-collection-api.json`) full set of requests and scripts
- CSV Test Data (`bookings_data.csv`) 20 rows of booking data generated via [Mockaroo](https://mockaroo.com)
- Environment file (`Restful-Booker_env.json`) stores base URL and dynamic token
- Newman HTML Report (`newman-report/Restful-Booker-Report.html`) automatically generated report after test execution

---

### 📂 performance-testing-restful_booker
This project includes automated API tests using [RESTful Booker API](https://restful-booker.herokuapp.com/).
API testing artifacts:
- Postman Collection (`Restful-Booker_API_Postman_Collection.postman_collection.json`) full set of requests and scripts
- CSV Test Data (`bookings_data.csv`) 20 rows of booking data generated via [Mockaroo](https://mockaroo.com)
- Environment file (`Restful-Booker_env.json`) stores base URL and dynamic token
- Newman HTML Report (`newman-report/Restful-Booker-Report.html`) automatically generated report after test execution



**Key Features:**
- Token-based authentication (handled via scripts)
- Create / Update / Partial Update / Delete booking endpoints tested
- Data-driven testing using CSV as source
- Assertions for each API response
- Chained requests using environment variables
- Negative scenarios tested (e.g. unauthorized updates)
- HTML report for visual test results

---

## Tech Stack & Tools
- Manual Testing: TestRail, Jira, Excel
- API Testing: Postman, Swagger, Mock Servers
- Performance: JMeter
- Automation: Selenium, PyTest
- Databases: MySQL, PostgreSQL
- CI/CD: Jenkins, GitHub Actions
- Reporting: Allure

---

## Goal
> My goal is to grow into a full-fledged **SDET** – combining QA expertise with development and automation.  
This portfolio reflects that journey through documentation, hands-on practice, and real-world simulation.

---

## Contact
Let's connect!
- Email: tetiana.yachna@gmail.com
- LinkedIn: https://www.linkedin.com/in/tetiana-yachna
