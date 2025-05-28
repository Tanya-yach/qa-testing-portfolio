# QA Testing Portfolio – Tetiana Yachna

Welcome to my testing portfolio! This repository showcases my work in software quality assurance across various testing disciplines.
The main goal is to simulate real QA tasks and showcase the skills required for a Software Development Engineer in Test (SDET) role.

--- 

## Repository Structure

### 📂 Manual Testing for Luxor
Manual testing project based on the real e-commerce website **[Luxor.cz](https://www.luxor.cz/)**.  
Includes test documentation for functional and UI testing. 
Artifacts for web testing:
- Test Plan (`Test_Plan_Luxor_Manual.md`)
- Test Scenarios (`Test_Scenarios_Luxor_Manual.md`)
- Test Cases (`Test_Cases_Luxor_Manual.md`)
- Checklists (`Check_list_Luxor_Manual.md`)
- Bug Reports (mock examples, coming soon)

---

### 📂 API Testing for Luxor (Mock API)
Since there is no public API for **[Luxor.cz](https://www.luxor.cz/)**, all endpoints were designed based on assumptions and simulated using a **Postman Mock Server**.
API testing artifacts:
- Test Plan (`Test_Plan_Luxor_API.md`)
- Test Cases (`Test_Cases_Luxor_API.md`)
- Postman Collection (`Luxor_API_Postman_Collection.json`) with pre-configured mock examples
- Bug Reports (coming soon)

---

### 📂 API Testing for Restful-Booker (Data-Driver Testing)
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
