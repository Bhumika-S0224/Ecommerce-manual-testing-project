# 🛒 E-Commerce Website Testing

<p align="center">
  <h2 align="center">Manual Testing Project</h2>
  <p align="center">
    Test Cases • Bug Reports • SQL Validation • Test Execution
  </p>
</p>

---

## 📌 About the Project

A personal manual testing project created to practically apply
software testing concepts to an E-Commerce web application.

### 🎯 Project Details

| | |
|---|---|
| **Domain** | E-Commerce |
| **Project Type** | Manual Testing |
| **Duration** | 2 Weeks |
| **Tools** | Excel, SQL, Jira |
| **Methodology** | Agile Scrum |

---

# 🧪 What I Tested

### 🔐 Login
- Valid username and password
- Invalid username
- Invalid password
- Blank username
- Blank password
- Blank username and password

### 🔎 Product Search
- Search existing product
- Search unavailable product
- Blank search
- Partial product search

### 🛒 Shopping Cart
- Add product
- Remove product
- Update quantity
- Verify cart total
- Verify empty cart

### 💳 Checkout
- Valid address
- Mandatory field validation
- Invalid postal code
- Order summary
- Order placement

### 📦 Order Management
- Order confirmation
- Order history
- Order details
- Order total

---

# 📋 My Actual Test Cases

I designed and executed manual test cases using Excel.

### Example

| TC ID | Module | Test Scenario | Expected Result | Status |
|---|---|---|---|---|
| TC_001 | Login | Login with valid credentials | User should login successfully | ✅ Pass |
| TC_002 | Login | Login with invalid password | Error message should display | ✅ Pass |
| TC_003 | Search | Search existing product | Relevant product should display | ✅ Pass |
| TC_004 | Cart | Add product to cart | Product should be added | ✅ Pass |
| TC_005 | Cart | Update product quantity | Quantity should update correctly | ✅ Pass |
| TC_006 | Checkout | Checkout with valid details | Order should be placed | ✅ Pass |

### 📸 Test Case Sheet

<p align="center">
  <img src="Screenshots/test-cases.png"
       alt="Actual Test Cases"
       width="950">
</p>

> 📁 Complete test cases: `Test-Cases/Ecommerce_Test_Cases.xlsx`

---

# 🐞 Defect Reporting

I documented defects with:

- Bug ID
- Summary
- Module
- Severity
- Priority
- Steps to Reproduce
- Expected Result
- Actual Result
- Status

### Example Defect

**BUG-001 — Cart quantity is not updated correctly**

| Field | Details |
|---|---|
| Module | Shopping Cart |
| Severity | Medium |
| Priority | High |
| Status | Closed |

### 📸 Bug Report

<p align="center">
  <img src="Screenshots/bug-report.png"
       alt="Bug Report"
       width="950">
</p>

> 📁 Complete bug reports: `Bug-Reports/Bug_Reports.xlsx`

---

# 🗄️ SQL Database Validation

I used SQL queries to validate application data.

### Example Queries

```sql
-- Verify customer data
SELECT * FROM customers;

-- Verify product data
SELECT * FROM products;

-- Verify customer orders
SELECT *
FROM orders
WHERE customer_id = 101;

-- Verify low-stock products
SELECT product_id, product_name, stock
FROM products
WHERE stock < 10;

-- Verify completed orders
SELECT *
FROM orders
WHERE status = 'Completed';
