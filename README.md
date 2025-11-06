# Epic Game Store Manual Test Suite

![Status](https://img.shields.io/badge/status-in_progress-orange)
![Tools](https://img.shields.io/badge/tools-Jira%20|%20Postman%20|%20GitHub-blue)


## Table of Contents

1. [Introduction](#10-introduction)
2. [Scope](#20-scope)
3. [Objectives](#30-objectives)
4. [Test Strategy](#40-test-strategy)
5. [Entry & Exit Criteria](#50-entry--exit-criteria)
6. [Product Risk Analysis](#60-product-risk-analysis)
7. [Test Environment & Configuration Management](#70-test-environment-&-configuration-management)
8. [Defect Management Process](#80-defect-management-process)
9. [Results Summary](#90-results-summary)


## 1.0. Introduction
This README contains the test plan for a comprehensive manual test suite of the [Epic Game Store web client](https://store.epicgames.com/en-US), a complex, real-world video game digital distribution service. The objective is to verify the functionality of the web client's core user-facing features and professionally document the whole process. 

### 1.1. Project Deliverables
- User Journeys: [Google Doc](https://docs.google.com/document/d/1CsofyqlI14Gm3ax4vr-Kgai7sXDXK0kzQkvHo1TPodE/edit?usp=sharing)
- Test Case Suite: 
- Defect Management Board: [Jira Board](https://errolgonito.atlassian.net/jira/software/projects/EGS/boards/1?atlOrigin=eyJpIjoiNzRkZWQ1MWJmZDBhNGRiN2JkZjIzOTVhNWIxOWVkZTciLCJwIjoiaiJ9) 
- API Test Collection: 

### 1.2. Skills Demonstrated
- Test Planning & Strategy
- Test Case Design (including Black-Box Techniques)
- Defect Reporting & Triage (Jira)
- Foundational API Validation (Postman)
- Static & Dynamic Testing Methodologies
- Functional & Exploratory Testing
- Git & GitHub for Documentation Version Control

## 2.0. Scope
### 2.1. In-Scope Features
This test plan covers the following features on the Epic Game Store website:

- **Account Management:**
  - User registration, login, logout, profile updates, and viewing purchase history.
  
- **Storefront Navigation:**
  - Browsing the store, searching for products, and applying search filters.
  
- **Product Discovery:**
  - Viewing individual game product pages and system requirements.
  
- **Purchase Flow:**
  - Managing the Wishlist, adding items to the Cart, and completing the checkout process using only free-to-play games.

### 2.2. Out-of-Scope Features
This plan will not cover the following:

- **Paid Transactions:**
  - The final step of any checkout flow that requires real payment to avoid incurring costs.

- **Native Desktop Client:**
  - The downloadable Epic Games Launcher (its installation, performance, and features).
  
- **Library Management:**
  - Viewing and managing owned games is launcher-exclusive.
  
- **Developer/Creator Portal:**
  - All sections related to the Unreal Engine, creator portals, and game development.

- **Specific Game Content:**
  - In-game functionality and community/news sections.

- **Non-Functional Testing:**
  - All forms of non-functional testing, including load, stress, performance, and backend server testing.

## 3.0. Objectives

- **Account Management:** To ensure a user can securely authenticate, manage their account details, and that all data changes are reflected accurately.

- **Storefront Navigation:** To validate that a user can easily discover products through browsing, searching, and filtering.

- **Purchase Flow:** To verify that a user can successfully acquire a free game, and that the game is correctly granted to their account.

## 4.0. Test Strategy 

### 4.1. Methodologies
This project will employ a hybrid testing approach:

- Scripted Testing: A comprehensive suite of formal test cases will be designed and executed to ensure full coverage of all in-scope functional requirements.

- Exploratory Testing: Unscripted, time-boxed testing sessions will be conducted to investigate high-risk areas to find defects that scripted tests may miss.

### 4.2. Tools
- **GitHub:** Used for version control of all test documentation, including this plan and the manual test cases.

- **Jira**: Used as the primary tool for defect management, including writing, tracking, and prioritising all bug reports.

- **Postman:** Used to conduct foundational API validation by inspecting GET requests to validate data fetched by the storefront.

### 4.3. Prioritisation Strategy
The project will employ a Risk-based prioritsation strategy. Test cases identified during the risk analysis to cover the highest risk will be tested and priortised first. Tests will be broken down into 3 categories, "High", "Medium" and "Low". All test cases labelled as "High" must be executed and pass as part of the test cycle.

## 5.0. Entry & Exit Criteria  

### 5.1. Entry Criteria
Test execution may not begin until the following criteria are met:

- This Test Plan document has been written and formally reviewed.

- All manual test cases for the in-scope features have been written and reviewed for clarity, accuracy, and coverage.

### 5.2. Exit Criteria
This manual testing project (Portfolio Project 1) will be considered complete when the following criteria are met:

- 100% of all planned manual test cases have been executed.

- All discovered defects have been documented and reported in the Jira project board.

- There are no open defects with a 'Critical' priority.

## 6.0. Product Risk Analysis

## Product Risk Analysis

This test plan is guided by a risk-based strategy. The following table identifies potential product risks, assesses their risk level, and defines the mitigation strategy for each.

| Risk Area | Potential Risk | Likelihood | Impact | Risk Level | Test Priority | Mitigation Strategy |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
|User Authentication |User with Valid Credentials is denied authentication |Medium |High |High Risk |P1 (Critical) |Design & execute positive/negative test cases |
|Game Search |User searches for a valid game and it does not appear in the results |Medium |High |High Risk |P1 (Critical) |Create Test cases that search with exact name and spelling errors.  |
|Search Filtering |User applies filters and results return the wrong games |Medium |Medium |Medium Risk |P2 (High) |Create Tests covering multiple filters at the same time and idependantly, then verify correct games are being returned |
|Wishlist |User adds a game to wishlist, but game does not save |Medium |Medium |Medium Risk |P2 (High) |Test adding and removing products to wishlist, and check for persistence before and after logging in |
|Purchasing Product |User with valid payment option is denied |Medium |High |High Risk |P1 (Critical) |Test the E2E flow. Verify all checkout page elements load correctly and payment options are displayed. |

## 7.0. Test Environment & Configuration Management

### 7.1. Test Environment
All manual test execution will be performed against the live production environment of the Epic Game Store.

- **URL:** `https://store.epicgames.com/`
- **Target Browsers:**
    - Google Chrome (latest stable version)
    - Mozilla Firefox (latest stable version)
- **Screen Resolution:** 1920x1080
- **Test Accounts:** One valid user account will be used to test persistence and user-specific data.

### 7.2. Configuration Management
To ensure traceability and reproducibility, all testware is version-controlled:

- **Test Plan:** This README, Versioned in this GitHub repository.
- **Test Cases:** Versioned in this GitHub repository in the `/test-cases` folder.
- **Defect Reports:** Managed and versioned by the [Jira Project Board](https://errolgonito.atlassian.net/jira/software/projects/EGS/boards/1).
- **API Collection:** Versioned as a JSON file in this repository and as a shared Postman collection.

## 8.0. Defect Management Process

### 8.1. Defect Workflow
All defects will be logged in the [Jira Project Board](https://errolgonito.atlassian.net/jira/software/projects/EGS/boards/1) and will follow this simple workflow:

1.  **To Do:** A new bug is identified and reported. It has not been reviewed.
2.  **In Progress (Mock Triage):** The bug has been reviewed, confirmed as a valid defect, and is ready for a developer (hypothetically).
3.  **Done (Closed):** The bug has been (hypothetically) fixed and verified, or has been closed as `Won't Fix`, `Duplicate`, or `Not a Bug`.

### 8.2. Triage Definitions (Severity vs. Priority)
To triage defects professionally, this project will use the following standard definitions:

| **Severity** (Impact on the system) | **Priority** (Urgency to fix) |
| :--- | :--- |
| **S1 (Critical):** Blocks core functionality; no workaround. | **P1 (Urgent):** Must be fixed immediately. |
| **S2 (High):** Major functionality impacted; difficult workaround exists. | **P2 (High):** Must be fixed for the next release. |
| **S3 (Medium):** Minor functionality impacted; easy workaround exists. | **P3 (Medium):** Fix if time allows. |
| **S4 (Low):** Cosmetic or UI issue. | **P4 (Low):** Fix at a later date. |

## 9.0. Results Summary




