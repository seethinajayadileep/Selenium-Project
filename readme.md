# 🛒 E-Commerce Website Automation Framework

A scalable UI Automation Framework built for an E-Commerce web application using **Selenium WebDriver**, **TestNG**, and **ExtentReports**, following the **Page Object Model (POM)** design pattern.

This framework demonstrates real-world automation architecture with reusable components, structured reporting, and maintainable test design.

---

## 🚀 Tech Stack

* Java
* Selenium WebDriver
* TestNG
* ExtentReports
* Maven
* Page Object Model (POM)
* JSON Data Handling
* Properties-based Configuration

---

## 📂 Project Structure

```
seleniumproject/
│
├── src/main/java
│   ├── AbstractComponents
│   ├── pageobjects
│   └── Utils
│
├── src/main/resources
│   └── GlobalData.properties
│
├── src/test/java
│   ├── data
│   │   └── PurchaseOrder.json
│   ├── stepDefinitions
│   ├── TestComponents
│   │   ├── BaseTest.java
│   │   ├── Listeners.java
│   │   └── Retry.java
│   └── tests
│
├── reports
├── testSuites
└── pom.xml
```

---

## 🏗 Framework Architecture

### 1️⃣ BaseTest

* Initializes WebDriver
* Handles browser setup (Chrome / Edge)
* Implements `@BeforeMethod` and `@AfterMethod`
* Manages driver lifecycle and cleanup
* Centralized configuration management

---

### 2️⃣ Page Objects

Implemented using the Page Object Model design pattern:

* LandingPage
* ProductCatalogue
* CartPage
* CheckoutPage
* ConfirmationPage
* OrderPage

Each page contains:

* WebElements
* Action methods
* Navigation logic
* Reusable wait handling

---

### 3️⃣ TestNG Features Used

* `@BeforeMethod`
* `@AfterMethod`
* DataProviders
* Retry Mechanism for flaky tests
* TestNG Listeners
* XML-based suite execution

---

### 4️⃣ ExtentReports Integration

* Custom `ExtentReporterNG` utility class
* TestNG Listener implementation
* Screenshot capture on test failure
* Thread-safe reporting for parallel execution

Reports are generated inside:

```
/reports
```

---

## 🔄 Test Scenarios Covered

* User Login
* Product Search & Selection
* Add to Cart
* Checkout Process
* Order Confirmation Validation
* Order History Validation

---

## 📊 Reporting Features

* HTML Extent Report generation
* Screenshots on failure
* Detailed step-level logging
* Pass / Fail / Skip status tracking

---

## 📦 Test Data Management

* JSON-based test data (`PurchaseOrder.json`)
* Configurable environment settings (`GlobalData.properties`)
* Reusable data utilities for dynamic test input

---

## ▶️ How To Run The Project

### Option 1 – Using TestNG XML

Run the suite file:

```
testng.xml
```

### Option 2 – Using Maven

```
mvn clean test
```

---

## 🎯 Key Automation Highlights

* Page Object Model implementation
* Reusable utility components
* Centralized WebDriver initialization
* Retry mechanism for unstable tests
* Screenshot capture on failure
* Config-driven browser selection
* Clean separation between test logic and framework logic
* Maintainable and scalable design

---

## 📌 Future Enhancements

* Docker integration
* CI/CD pipeline (GitHub Actions / Jenkins)
* Parallel execution optimization
* Selenium Grid integration
* API + UI combined automation

---

## 👨‍💻 Author

Jaya Dileep
Automation Engineer |
GitHub: https://github.com/seethinajayadileep

---

## 📜 License

This project is for learning and demonstration purposes.
