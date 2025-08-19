# QuantumLeap E-Commerce Test Automation Framework 🚀

A comprehensive **test automation framework** built to validate both UI and API functionality of an e-commerce application.  
This project demonstrates **end-to-end automation**, **BDD practices**, **API testing**, and covers conceptual **performance** and **security** testing strategies.  
It is designed as a **professional, portfolio-ready project** to showcase modern QA automation practices.

---

## 🔹 Applications Under Test (AUT)

- **Web Application:** [Sauce Labs Demo E-Commerce Site](https://www.saucedemo.com/)  
- **REST API:** [ReqRes - A Hosted REST-API](https://reqres.in/)  

---

## 🔹 Features

### 1. UI Test Automation (Selenium + TestNG)
- Automated critical **user flows**:
  - Login with multiple datasets (standard user, locked-out user, glitch user).
  - End-to-End Purchase Flow (login → add item → cart → checkout → confirm order).
- **Stability Enhancements**:
  - Explicit waits for synchronization.
  - Screenshots captured automatically on test failure.
  - JavaScriptExecutor for advanced UI actions (scroll, hidden elements, etc.).

### 2. Behavior-Driven Development (BDD with Cucumber)
- **Feature File** written in Gherkin syntax for readability.  
- Step Definitions call UI methods for **reusability & maintainability**.  
- Test Runner integrated with **TestNG**.

### 3. API Test Automation (REST Assured)
- Automated tests for CRUD operations:
  - `GET` – Fetch users & validate status/response.
  - `POST` – Create user & validate response body.
  - `PUT` – Update user & verify update success.

### 4. Reporting
- Integrated **Extent Reports** for rich HTML reporting.  
- Includes pass/fail logs, screenshots on failure, and detailed execution summary.

---

## 🔹 Performance Test Plan (Conceptual)

**Objective:** Validate performance of the **Login functionality** under load.  

- **Scope:**  
  - Measure system behavior with multiple concurrent users accessing login.  

- **Workload Model:**  
  - 50 virtual users simultaneously attempting login.  

- **Key Metrics:**  
  - Response Time (avg, p95)  
  - Throughput (requests/sec)  
  - Error Rate (%)  

- **Tools (suggested):** JMeter / Gatling / Locust  

---

## 🔹 Security Testing Scenarios (Conceptual)

1. **Authentication Bypass**  
   - Attempt to access a protected page (e.g., inventory) without logging in.  
   - Expected: Redirect to login page, no access granted.  

2. **Cross-Site Scripting (XSS)**  
   - Inject `<script>alert('XSS')</script>` in login input fields.  
   - Expected: Input sanitized, script not executed, safe error handling.  

---

## 🔹 Project Structure

```

QuantumLeap/
│── src/test/java
│   ├── ui/        # Selenium UI tests
│   ├── api/       # REST Assured API tests
│   ├── bdd/       # Feature files & step definitions
│   └── utils/     # Helpers, listeners, configs
│
│── reports/       # Extent Reports output
│── resources/     # Test data, config files
│── README.md      # Project documentation
│── pom.xml        # Maven dependencies & plugins

````

---

## 🔹 Setup & Execution

### Prerequisites
- Java 11+
- Maven
- ChromeDriver (latest version)
- Internet connection (for AUT & API)

### Steps
```bash
# Clone repo
git clone https://github.com/your-username/QuantumLeap-Automation.git

# Navigate to project
cd QuantumLeap-Automation

# Run UI & API tests with TestNG
mvn clean test

# Run Cucumber BDD tests
mvn test -Dcucumber.options="classpath:features"

# Generate Extent Report
# Open report from: /reports/extent-report.html
````

---

## 🔹 Sample Report

After test execution, a detailed **Extent Report** (`extent-report.html`) will be generated.
The report includes:

* Pass/Fail summary
* Execution logs
* Screenshots for failures

---

## 🔹 Tech Stack

* **Java 11**
* **Selenium WebDriver**
* **TestNG**
* **Cucumber (BDD)**
* **REST Assured**
* **Maven**
* **Extent Reports**

---

## 📌 Final Deliverables

1. Complete source code hosted on GitHub.
2. Professional **README.md** (this file).
3. Conceptual docs integrated for **Performance** & **Security** testing.
4. Example **Extent Report** included under `/reports`.

---

> ⚡ This project demonstrates a **full QA automation framework** across functional, API, BDD, performance, and security testing concepts.

```

---
