# Epic Game Store Manual Test Suite

## 1.0 Introduction
This README contains the test plan for a comprehensive manual test suite of the [Epic Game Store web client](https://store.epicgames.com/en-US). The objective is to verify the functionality of the web client's core user-facing features and document the whole process. 

## 2.0 Scope
### 2.1. In-Scope Features
This test plan covers the following features on the Epic Game Store website:

- **Account Management:**
  - User registration, login, logout, profile updates, and viewing purchase history.
  
- **Storefront Navigation:**
  - Browsing the store, searching for products, and applying search filters (e.g., price, genre).
  
- **Product Discovery:**
  - Viewing individual game product pages and system requirements.
  
- **Purchase Flow:**
  - Managing the Wishlist, adding items to the Cart, and completing the checkout process using only free-to-play games.
  
- **Library Management:**
  - Viewing and managing owned games in the user's web-based library.
  
- **Support Interface:**
  - Navigating to and using the "Contact Support" flows.

### 2.2. Out-of-Scope Features
This plan will not cover the following:

- **Paid Transactions:**
  - The final step of any checkout flow that requires a real payment instrument (e.g., credit card, PayPal) is explicitly out-of-scope to avoid incurring costs.

- **Native Desktop Client:**
  - The downloadable Epic Games Launcher, its installation, performance, and features are not under test.
  
- **Developer/Creator Portal:**
  - All sections related to the Unreal Engine, creator portals, and game development are out-of-scope.

- **Specific Game Content:**
  - In-game functionality, specific game pages (e.g., Fortnite, Fall Guys), and community/news sections are not part of this test.

- **Non-Functional Testing:**
  - All forms of non-functional testing, including load, stress, performance, and backend server testing, are out-of-scope.

## 3.0 Objectives

- **Account Management:** To ensure a user can securely authenticate, manage their account details, and that all data changes are reflected accurately.

- **Storefront Navigation:** To validate that a user can easily discover products through browsing, searching, and filtering.

- **Purchase Flow:** To verify that a user can successfully acquire a free game, and that the game is correctly granted to their account (entitlement).

## Test Strategy 

## Entry & Exit Criteria  
