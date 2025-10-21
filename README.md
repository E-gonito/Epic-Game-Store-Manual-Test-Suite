# Epic Game Store Manual Test Suite

## Table of Contents

1. [Introduction](#10-introduction)

   * [Project Deliverables](#11-project-deliverables)
   * [Skills Demonstrated](#12-skills-demonstrated)
2. [Scope](#20-scope)

   * [In-Scope Features](#21-in-scope-features)
   * [Out-of-Scope Features](#22-out-of-scope-features)
3. [Objectives](#30-objectives)
4. [Test Strategy](#40-test-strategy)

   * [Methodologies](#41-methodologies)
   * [Tools](#42-tools)
5. [Entry & Exit Criteria](#50-entry--exit-criteria)

   * [Entry Criteria](#51-entry-criteria)
   * [Exit Criteria](#52-exit-criteria)
6. [Results Summary](#60-results-summary)
7. [Learning Reflection](#70-learning-reflection)

## 1.0. Introduction
This README contains the test plan for a comprehensive manual test suite of the [Epic Game Store web client](https://store.epicgames.com/en-US), a complex, real-world video game digital distribution service. The objective is to verify the functionality of the web client's core user-facing features and professionally document the whole process. 

### 1.1. Project Deliverables
- Test Case Suite: 
- Defect Management Board: 
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
  
- **Library Management:**
  - Viewing and managing owned games in the user's web-based library.

### 2.2. Out-of-Scope Features
This plan will not cover the following:

- **Paid Transactions:**
  - The final step of any checkout flow that requires a real payment instrument is explicitly out-of-scope to avoid incurring costs.

- **Native Desktop Client:**
  - The downloadable Epic Games Launcher, its installation, performance, and features are not under test.
  
- **Developer/Creator Portal:**
  - All sections related to the Unreal Engine, creator portals, and game development are out-of-scope.

- **Specific Game Content:**
  - In-game functionality and community/news sections are not part of this test.

- **Non-Functional Testing:**
  - All forms of non-functional testing, including load, stress, performance, and backend server testing, are out-of-scope.

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

## 6.0. Results Summary

## 7.0. Learning Reflection


