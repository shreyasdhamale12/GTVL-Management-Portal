## **Day 2**

# 🐞 Management Portal — Bug Report Documentation

This document provides a consolidated list of identified bugs within the **Management Portal**.
Each bug includes its **Bug ID**, module reference, severity, priority, reproduction steps, expected results, and actual results.

---

## 📋 Summary of Reported Bugs

| Bug ID      | Bug No. | Title                                   | Module        | Severity | Priority |
| ----------- | ------: | --------------------------------------- | ------------- | -------- | -------- |
| **BUG-001** |       1 | No Duplicate ID Validation              | SKUs          | Medium   | **P3**   |
| **BUG-002** |       2 | No Sanitization for Input Fields        | SKUs          | High     | **P2**   |
| **BUG-003** |       3 | SKU Action Elements Not Clickable       | SKUs          | Medium   | **P3**   |
| **BUG-004** |       4 | Missing Delete Success Message          | SKUs          | Low      | **P4**   |
| **BUG-005** |       5 | Missing Authentication (No Login Check) | Portal Access | Critical | **P1**   |
| **BUG-006** |       6 | Console Logs Present in Production      | Global/Portal | High     | **P2**   |
| **BUG-007** |       7 | Unable to Submit Feedback               | Feedback      | Low      | **P4**   |
| **BUG-008** |       8 | Store Section Buttons Not Clickable     | Store         | High     | **P2**   |
| **BUG-009** |       9 | Sign Out Not Working                    | Portal Access | High     | **P1**   |
| **BUG-010** |      10 | Update Not Working in Promodizers Field | Promodizers   | Medium   | **P3**   |
| **BUG-011** |      11 | Export Button Not Working               | Stores        | Low      | **P4**   |

---

### 🔧 Priority Scale

* **P1 — Critical**
* **P2 — High**
* **P3 — Medium**
* **P4 — Low**

---

# 🐛 Detailed Bug Reports

---

## **BUG-001 — No Duplicate ID Validation**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Medium  
**Priority:** P3  

### Steps to Reproduce

1. Open the Management Portal.
2. Navigate to **SKUs → Add New SKU**.
3. Enter an already existing SKU Code.

### Expected Result

System displays: **“SKU Code already exists.”**

### Actual Result

* Duplicate SKU codes are accepted.
* Causes risk of data inconsistency.

### Screenshots

1. Existing SKU Code <img width="1502" src="https://github.com/user-attachments/assets/3f4af317-e7a1-45b9-98c3-febf1b7e9381" />

2. New Product Created with the Same SKU Code <img width="1526" src="https://github.com/user-attachments/assets/d876d68f-f803-4221-8b1c-3b2993009576" />

---

## **BUG-002 — No Sanitization for Input Fields**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** High  
**Priority:** P2  

### Steps to Reproduce

1. Open the Management Portal.
2. In **SKUs → Search**, enter special characters.
3. In **Add New SKU**, enter special characters in Product Name.

### Expected Result

Input fields should validate and restrict unsafe characters.

### Actual Result

Special characters are accepted without sanitization.

### Screenshot

<img width="1512" src="https://github.com/user-attachments/assets/68c92846-5c0f-4ff2-be39-529f55188c13" />

---

## **BUG-003 — SKU Action Elements Not Clickable**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Medium  
**Priority:** P3  

### Steps to Reproduce

1. Open the Management Portal.
2. Navigate to the **SKUs** section.
3. Attempt to click **View**, **Edit**, or **Delete**.

### Expected Result

Action icons should respond normally.

### Actual Result

Icons only respond when clicking off-target.

---

## **BUG-004 — Missing Delete Success Message**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Low  
**Priority:** P4  

### Steps to Reproduce

1. Open the Management Portal.
2. Go to **SKUs → View Details → Delete**.

### Expected Result

Success message: **“Deleted successfully.”**

### Actual Result

Message does not appear.

---

## **BUG-005 — Missing Authentication (No Login Required)**

**Portal:** Management Portal  
**Module:** Portal Access  
**Severity:** Critical  
**Priority:** P1  

### Steps to Reproduce

1. Directly open the Management Portal URL.

### Expected Result

User should be required to authenticate.

### Actual Result

Portal opens without any login required.

---

## **BUG-006 — Console Logs Present in Production**

**Portal:** Management Portal  
**Module:** Global / Console  
**Severity:** High  
**Priority:** P2  

### Steps to Reproduce

1. Open the Management Portal.
2. Press **F12**.
3. Browse across pages.

### Expected Result

No debug logs should appear in production.

### Actual Result

Console shows messages such as:

* “This page is not reloaded”
* “App data already initialized”
* “[Stage1] Helpbot initialized successfully”

### Screenshot

<img width="1905" src="https://github.com/user-attachments/assets/1ef2d7b2-cfa5-409f-a658-9051e0c4d30b" />

---

## **BUG-007 — Unable to Submit Feedback**

**Portal:** Management Portal  
**Module:** Feedback  
**Severity:** Low  
**Priority:** P4  

### Steps to Reproduce

1. Open the Management Portal.
2. Open the **Feedback** panel.
3. Enter details and click **Submit Feedback**.

### Expected Result

Feedback should submit and show a success message.

### Actual Result

System shows: **“Failed to submit feedback. Please try again.”**

### Screenshot

<img width="936" src="https://github.com/user-attachments/assets/547563d1-0474-4e17-a872-fd9ad42af064" />

---

## **BUG-008 — Store Section Buttons Not Clickable**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** High  
**Priority:** P2  

### Steps to Reproduce

1. Open the Management Portal.
2. Navigate to the **Stores** section.
3. Click **View**, **Edit**, or **Delete**.

### Expected Result

Buttons should trigger their respective actions.

### Actual Result

Buttons are not responsive.

---

## **BUG-009 — Sign Out Not Working**

**Portal:** Management Portal  
**Module:** Portal Access  
**Severity:** High  
**Priority:** P1  

### Steps to Reproduce

1. Open the Management Portal.
2. Click the admin username (top-right).
3. Select **Sign Out**.

### Expected Result

User should be logged out.

### Actual Result

Logout does not occur.

---

## **BUG-010 — Update Not Working in Promodizers Section**

**Portal:** Management Portal  
**Module:** Promodizers  
**Severity:** Medium  
**Priority:** P3  

### Steps to Reproduce

1. Navigate to the **Promodizers** section.
2. Click **Edit** on any user.
3. Modify the **Last Name**.
4. Click **Update Supervisor**.

### Expected Result

A success message should appear.

### Actual Result

Validation error:
**“Please enter a valid phone number (e.g., +1-555-0123).”**

### Screenshot

<img width="1254" src="https://github.com/user-attachments/assets/33d63f63-b6e6-4f10-85a3-8c31aab8040e" />

---

## **BUG-011 — Export Button Not Working in Stores Module**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** Low  
**Priority:** P4  

### Steps to Reproduce

1. Open the Management Portal.
2. Go to the **Stores** section.
3. Click **Export**.

### Expected Result

A file containing store data should download.

### Actual Result

The button is not clickable.

### Screenshot

<img width="1566" src="https://github.com/user-attachments/assets/a7e976d6-36c3-46e7-965f-6d3c49ccd98d" />

---


