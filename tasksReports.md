#  ERP System — Software Quality Control (SQC) Bug Report Documentation

This document contains all identified **issues**, **bugs**, **vulnerabilities**, and **improvement opportunities** across all portals of the **ERP System**.
It is formatted as a **professional README.md** suitable for submission or repository documentation.


---

---

#  Management Portal

This section lists all identified bugs in the **Management Portal**.
Each bug includes a dedicated Bug ID (starting from MP-1), severity, priority, description, and reproducible steps.

---

## 📋 Summary of Reported Bugs (Management Portal)

| Bug ID    | Bug No. | Title                                   | Module        | Severity | Priority |
|-----------|--------:|-----------------------------------------|---------------|----------|----------|
| **MP-1**  |       1 | No Duplicate ID Validation              | SKUs          | Medium   | P3       |
| **MP-2**  |       2 | No Sanitization for Input Fields        | SKUs          | High     | P2       |
| **MP-3**  |       3 | SKU Action Elements Not Clickable       | SKUs          | Medium   | P3       |
| **MP-4**  |       4 | Missing Delete Success Message          | SKUs          | Low      | P4       |
| **MP-5**  |       5 | Missing Authentication (No Login Check) | Portal Access | Critical | P1       |
| **MP-6**  |       6 | Console Logs Present in Production      | Global/Portal | High     | P2       |
| **MP-7**  |       7 | Unable to Submit Feedback               | Feedback      | Low      | P4       |
| **MP-8**  |       8 | Store Section Buttons Not Clickable     | Stores        | High     | P2       |
| **MP-9**  |       9 | Sign Out Not Working                    | Portal Access | High     | P1       |
| **MP-10** |      10 | Update Not Working in Promodizers       | Promodizers   | Medium   | P3       |
| **MP-11** |      11 | Export Button Not Working               | Stores        | Low      | P4       |
| **MP-12** |      12 | Duplicate Phone & Email Allowed         | Promodizers   | High     | P2       |
| **MP-13** |      13 | Phone Number Not Auto-Formatted         | Promodizers   | Low      | P4       |
| **MP-14** |      14 | Sort Field Not Working in SKUs          | SKUs          | Low      | P3       |
| **MP-15** |      15 | Sort Icon Visible Only on Hover         | Stores        | Low      | P4       |
| **MP-16** |      16 | Country Field Prefilled with “USA”      | Stores        | Low      | P3       |


---

## 🔧 Priority Scale

* **P1 — Critical**
* **P2 — High**
* **P3 — Medium**
* **P4 — Low**


---

#  Promodizer Portal

---

## 📋 Summary of Reported Bugs (Promodizer Portal)

| Bug ID   | Bug No. | Title                                     | Module        | Severity | Priority |
|----------|--------:|-------------------------------------------|---------------|----------|----------|
| **PP-1** |       1 | Promodizer Can Access Pages Without Login | Entire Portal | Critical | P1       |
| **PP-2** |       2 | Console Logs Expose Internal Information  | All Modules   | High     | P2       |
| **PP-3** |       3 | Barcode Number Not Visible When Scanning  | Record Sales  | High     | P2       |
| **PP-4** |       4 | Sales History Not Visible                 | Sales History | High     | P2       |
| **PP-5** |       5 | All Dates Display Under Sunday            | Attendance    | High     | P2       |


---

#  Supervisor Portal

---

## 📋 Summary of Reported Bugs (Supervisor Portal)

| Bug ID   | Bug No. | Title                                            | Module         | Severity | Priority |
|----------|--------:|--------------------------------------------------|----------------|----------|----------|
| **SP-1** |       1 | Supervisor Accesses Promodizers Not Assigned     | My Team        | High     | P1       |
| **SP-2** |       2 | Sales Record Not Loading                         | Dashboard      | High     | P1       |
| **SP-3** |       3 | Name & Phone Fields Accept Invalid Characters    | Add Promodizer | High     | P1       |
| **SP-4** |       4 | Invalid Inputs Not Validated                     | Add Promodizer | High     | P1       |
| **SP-5** |       5 | No Edit/Delete Option After Adding Promodizer    | My Team        | Medium   | P3       |
| **SP-6** |       6 | Console Logs Leak Internal Data                  | Dashboard      | Medium   | P3       |
| **SP-7** |       7 | Console Logs Expose Internal Debug Messages      | Dashboard      | Medium   | P3       |
| **SP-8** |       8 | No Authentication Required                       | Entire Portal  | Critical | P1       |


---

#  Sales Analytics Dashboard

This section outlines all bugs identified inside the **Sales Analytics Dashboard**.
Bug IDs start from **SA-1**.

---

## 📋 Summary of Reported Bugs (Sales Analytics Dashboard)

| Bug ID    | Bug No.  | Title                                            | Module            | Severity | Priority |
|-----------|----------|--------------------------------------------------|-------------------|----------|----------|
| **SA-1**  | BUG-01   | Console Logs Exposing Internal Data              | SKU Performance   | High     | P1       |
| **SA-2**  | BUG-02   | Filters Accept Invalid Inputs                    | SKU Performance   | High     | P2       |
| **SA-3**  | BUG-03   | No Authentication Required                       | Entire Portal     | High     | P2       |
| **SA-4**  | BUG-04   | Data Mismatch Between Modules & Dashboard Charts | Dashboard         | High     | P2       |
| **SA-5**  | BUG-05   | Chart Preference Not Reflected in Dashboard      | Dashboard         | High     | P2       |
| **SA-6**  | BUG-06   | Staff Not Found                                  | Staff Performance | High     | P1       |
| **SA-7**  | BUG-07   | UI Elements Overlap                              | Store Performance | Medium   | P3       |
| **SA-8**  | BUG-08   | Data Keeps Loading                               | Staff Performance | Medium   | P3       |
| **SA-9**  | BUG-09   | Cannot Cancel Applied Filters                    | Transaction Hist. | High     | P2       |
| **SA-10** | BUG-10   | Invalid Date Range Accepted                      | Multiple Modules  | High     | P2       |
| **SA-11** | BUG-11   | Dashboard Preferences Not Reflected              | Settings          | Medium   | P3       |
| **SA-12** | BUG-12   | Date/Time Format Change Not Applied              | Settings          | Medium   | P3       |
| **SA-13** | BUG-13   | Sort Not Working for City/State Columns          | Store Performance | Medium   | P3       |
| **SA-14** | BUG-14   | City Dropdown Not Working                        | Store Performance | Medium   | P3       |
| **SA-15** | BUG-15   | Sales Volume Accepts Negative Values             | Store Performance | High     | P3       |
| **SA-16** | BUG-16   | UI Fluctuation During Sorting                    | Transaction Hist. | Low      | P4       |
| **SA-17** | BUG-17   | Data Leakage in of Stores                        | Store Performance | Critical | P1       |



---

---

#  **Management Portal —  Report**

This document lists all known issues identified in the **Management Portal**, including modules, severity, priorities, and clear reproducible steps.

---

## **BUG-001 — No Duplicate ID Validation**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Navigate to **SKUs → Add New SKU**.
3. Enter an already existing SKU Code.

### **Expected Result**

System should display: **“SKU Code already exists.”**

### **Actual Result**

* Duplicate SKU codes are accepted.
* Creates risk of data inconsistency.

### **Screenshots**

1. Existing SKU Code <img width="1502" src="https://github.com/user-attachments/assets/3f4af317-e7a1-45b9-98c3-febf1b7e9381" />

2. New Product Created with the Same SKU Code <img width="1526" src="https://github.com/user-attachments/assets/d876d68f-f803-4221-8b1c-3b2993009576" />

---

## **BUG-002 — No Sanitization for Input Fields**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open the Management Portal.
2. In **SKUs → Search**, enter special characters.
3. In **Add New SKU**, enter special characters in the Product Name.

### **Expected Result**

Input fields should validate and restrict unsafe characters.

### **Actual Result**

Special characters are accepted without sanitization.

### **Screenshot**

<img width="1512" src="https://github.com/user-attachments/assets/68c92846-5c0f-4ff2-be39-529f55188c13" />

---

## **BUG-003 — SKU Action Elements Not Clickable**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Navigate to **SKUs**.
3. Try clicking **View**, **Edit**, or **Delete** icons.

### **Expected Result**

Action icons should be clickable and responsive.

### **Actual Result**

Icons only respond when clicking slightly off-target.

---

## **BUG-004 — Missing Delete Success Message**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Navigate to **SKUs → View Details → Delete**.

### **Expected Result**

Message: **“Deleted successfully.”**

### **Actual Result**

Success message does not appear.

---

## **BUG-005 — Missing Authentication (No Login Required)**

**Portal:** Management Portal  
**Module:** Portal Access  
**Severity:** Critical  
**Priority:** P1  

### **Steps to Reproduce**

1. Open the Management Portal URL directly.

### **Expected Result**

User must be required to log in.

### **Actual Result**

Portal loads without authentication.

---

## **BUG-006 — Console Logs Visible in Production**

**Portal:** Management Portal  
**Module:** Global / Console  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Press **F12** to open DevTools.
3. Browse through various modules.

### **Expected Result**

No console logs should appear in production builds.

### **Actual Result**

Debug messages appear, such as:

* “This page is not reloaded”
* “App data already initialized”
* “[Stage1] Helpbot initialized successfully”

### **Screenshot**

<img width="1905" src="https://github.com/user-attachments/assets/1ef2d7b2-cfa5-409f-a658-9051e0c4d30b" />

---

## **BUG-007 — Unable to Submit Feedback**

**Portal:** Management Portal  
**Module:** Feedback  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Open the **Feedback** side panel.
3. Enter input and click **Submit Feedback**.

### **Expected Result**

Feedback should be submitted successfully.

### **Actual Result**

Message shown: **“Failed to submit feedback. Please try again.”**

### **Screenshot**

<img width="936" src="https://github.com/user-attachments/assets/547563d1-0474-4e17-a872-fd9ad42af064" />

---

## **BUG-008 — Store Section Buttons Not Clickable**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Navigate to the **Stores** module.
3. Attempt to click **View**, **Edit**, or **Delete**.

### **Expected Result**

Buttons should execute their respective actions.

### **Actual Result**

Buttons are not responsive.

---

## **BUG-009 — Sign Out Not Working**

**Portal:** Management Portal  
**Module:** Portal Access  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Click the admin username (top-right).
3. Select **Sign Out**.

### **Expected Result**

User should be logged out and redirected.

### **Actual Result**

Logout does not work.

---

## **BUG-010 — Update Not Working in Promodizers Section**

**Portal:** Management Portal  
**Module:** Promodizers  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Promodizers**.
2. Click **Edit** for any user.
3. Modify the **Last Name**.
4. Click **Update Supervisor**.

### **Expected Result**

Changes should save and a success message should appear.

### **Actual Result**

Validation error:
**“Please enter a valid phone number (e.g., +1-555-0123).”**

### **Screenshot**

<img width="1254" src="https://github.com/user-attachments/assets/33d63f63-b6e6-4f10-85a3-8c31aab8040e" />

---

## **BUG-011 — Export Button Not Working in Stores Module**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Open the Management Portal.
2. Go to **Stores**.
3. Click **Export**.

### **Expected Result**

A file containing store details should download.

### **Actual Result**

Export button is unresponsive.

### **Screenshot**

<img width="1566" src="https://github.com/user-attachments/assets/a7e976d6-36c3-46e7-965f-6d3c49ccd98d" />

---

## **BUG-012 — Duplicate Phone & Email Allowed for Promodizers**

**Portal:** Management Portal  
**Module:** Promodizers  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Go to **Promodizers**.
2. Copy an existing user’s phone number and email.
3. Click **Add New Promodizer**.
4. Enter the same phone and email values.

### **Expected Result**

System should not allow duplicate email or phone numbers.

### **Actual Result**

Promodizer is created with duplicate contact information.

### **Screenshot**

[https://github.com/user-attachments/assets/e5b6c314-1711-420f-9429-6e0093a86bab](https://github.com/user-attachments/assets/e5b6c314-1711-420f-9429-6e0093a86bab)

---

## **BUG-013 — Phone Number Should Auto-Format**

**Portal:** Management Portal  
**Module:** Promodizers  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Go to **Promodizers**.
2. Click **Add New Promodizer**.
3. Enter a phone number.

### **Expected Result**

Phone number should auto-format as user types.

### **Actual Result**

Formatting must be entered manually.

---

## **BUG-014 — Sort Function Not Working in SKUs**

**Portal:** Management Portal  
**Module:** SKUs  
**Severity:** Low  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **SKUs**.
2. Click the sort icon next to any column header.

### **Expected Result**

Sorting should work in ascending/descending order.

### **Actual Result**

Sorting does not work.

### **Screenshot**

<img width="1877" height="590" alt="image" src="https://github.com/user-attachments/assets/d858d507-f45f-4b66-b28a-1de7554b2bb2" />

---

## **BUG-015 — Sort Icon Visible Only on Hover**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Go to **Stores**.
2. Hover over columns such as Store Name or Store Code.

### **Expected Result**

Sort icon should remain visible at all times.

### **Actual Result**

Sort icon only appears on hover.

### **Video**

[https://github.com/user-attachments/assets/4a5fd5a1-35dc-4a3d-ab65-b39175e7a7da](https://github.com/user-attachments/assets/4a5fd5a1-35dc-4a3d-ab65-b39175e7a7da)

---

## **BUG-016 — Country Field Prefilled with “USA”**

**Portal:** Management Portal  
**Module:** Stores  
**Severity:** Low  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Stores**.
2. Click **Add New Store**.
3. Check the **Country** field.

### **Expected Result**

Country should be blank.

### **Actual Result**

Country is prefilled with **USA**.

### **Video**

[https://github.com/user-attachments/assets/7d864aba-5a68-4bd0-bea1-0bf8abf26fa6](https://github.com/user-attachments/assets/7d864aba-5a68-4bd0-bea1-0bf8abf26fa6)


---

---

# **Promodizer Portal — Bug Report Documentation**

---

## **BUG-01 — Promodizer Can Access All Pages Without Login**

**Portal:** Promodizer Portal  
**Module:** Entire Portal   
**Severity:** Critical  
**Priority:** P1  

### **Steps to Reproduce**

1. Open the Promodizer Portal URL directly.
2. Attempt to access any page.

### **Expected Result**

User should be redirected to the **Login** page.

### **Actual Result**

All pages are accessible **without authentication**.

---

## **BUG-02 — Console Log Leaks Internal Information**

**Portal:** Promodizer Portal  
**Module:** All Modules  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open **DevTools → Console**.
2. Navigate through any page in the Promodizer Portal.

### **Expected Result**

No sensitive or internal logs should appear in the console.

### **Actual Result**

Internal system logs are printed in the console.

### **Screenshot**

<img width="1912" height="442" alt="image" src="https://github.com/user-attachments/assets/bc9734ff-b44d-42f4-baf9-754326f3c00c" />

---

## **BUG-03 — Barcode Number Not Visible While Scanning**

**Portal:** Promodizer Portal  
**Module:** Record Sales  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open **Record Sales**.
2. Select a store from the **Select Store Location** dropdown.
3. Enter or scan the **barcode number**.

### **Expected Result**

The barcode number should be visible while entering or scanning.

### **Actual Result**

Barcode number is submitted directly without being visible to the user.

### **Video**

[https://github.com/user-attachments/assets/2fe10518-6fcc-4b57-b37a-8e44bddb3a04](https://github.com/user-attachments/assets/2fe10518-6fcc-4b57-b37a-8e44bddb3a04)

---

## **BUG-04 — Sales History Not Visible**

**Portal:** Promodizer Portal  
**Module:** Sales History  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open **Record Sales**.
2. Select a store using the **Select Store Location** dropdown.
3. Enter or scan a barcode, add products, then click **Submit Sales**.
4. Go to **Sales History**.
5. Click on the most recent sales entry.

### **Expected Result**

The recorded sales details should be displayed.

### **Actual Result**

System displays **“Sales record not found.”**

### **Video**

[https://github.com/user-attachments/assets/a687b5e6-9213-494d-8dce-a877125e1554](https://github.com/user-attachments/assets/a687b5e6-9213-494d-8dce-a877125e1554)

---

## **BUG-05 — All Dates Displayed Under Sunday in Calendar View**

**Portal:** Promodizer Portal  
**Module:** Attendance History  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open **Attendance History**.
2. Navigate to **Calendar View**.

### **Expected Result**

Each date should appear under its correct weekday.

### **Actual Result**

All dates are displayed under **Sunday**.

### **Screenshot**

<img width="1882" height="734" alt="image" src="https://github.com/user-attachments/assets/09101779-b520-46a5-8b20-fd3772ef8747" />



---  

---

# **Supervisor Portal — Bug Report Documentation**


---

## **BUG-01 — Supervisor Can Access Promodizers Not Assigned to Them**

**Portal:** Supervisor Portal  
**Module:** My Team  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Open the **Management Portal**.
2. Go to the **Supervisor** section → select *Sarah Mitchell* → open the store assigned to her → remove a promodizer.
3. Now open the **Supervisor Portal → My Team** module.
4. Under the store section, observe the assigned promodizers.

### **Expected Result**

Supervisor should only see and manage promodizers assigned to their specific store.

### **Actual Result**

Supervisor can access **all promodizers** due to hardcoded data.

### **Screenshots**

**Management Portal** <img width="1885" height="850" src="https://github.com/user-attachments/assets/a5f8e5fa-7b27-48da-8797-49197d889bc4" />

**Supervisor Portal** <img width="1891" height="859" src="https://github.com/user-attachments/assets/6efb1810-c2a2-47af-aa07-aebcd351cd10" />

---

## **BUG-02 — Sales Record Not Loading**

**Portal:** Supervisor Portal  
**Module:** Dashboard  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Go to **Record Sales** and enter barcode numbers for 2–3 products.
2. Navigate to **Dashboard → Quick Actions → Sales History**.
3. Click the generated **batch_...** record.

### **Expected Result**

Sales record details should load properly.

### **Actual Result**

The interface displays **“Loading sales record…”** indefinitely.

### **Screenshot**

<img width="1885" height="481" src="https://github.com/user-attachments/assets/a433941d-f338-492d-b2fc-95b7550df5dc" />

---

## **BUG-03 — Add Promodizer Accepts Alphabets & Special Characters in Numeric Fields**

**Portal:** Supervisor Portal  
**Module:** Add Promodizer  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Open **Add Promodizer**.
2. Enter:

   * Special characters in **First Name** and **Last Name**
   * Alphabets & special characters in **Phone Number**

### **Expected Result**

Fields should only accept **valid input** (e.g., numbers for phone fields).

### **Actual Result**

Fields accept alphabets and special characters.

### **Screenshot**

<img width="1887" height="693" src="https://github.com/user-attachments/assets/5cb22359-5ce0-4d92-8557-2781858ed00e" />

---

## **BUG-04 — Add Promodizer Accepts Invalid Form Inputs (Duplicate of Bug 03)**

**Portal:** Supervisor Portal  
**Module:** Add Promodizer  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

Same steps as **BUG-03**.

### **Expected Result**

Validation should restrict invalid inputs.

### **Actual Result**

System allows invalid inputs.

### **Screenshot**

<img width="1887" height="693" src="https://github.com/user-attachments/assets/5cb22359-5ce0-4d92-8557-2781858ed00e" />

---

## **BUG-05 — Missing Edit/Delete Options for Promodizers**

**Portal:** Supervisor Portal  
**Module:** My Team  
**Severity:** Low  
**Priority:** P3  

### **Steps to Reproduce**

1. Open **My Team**.
2. Click on any promodizer profile.

### **Expected Result**

Profile page should display **Edit** and **Delete** options.

### **Actual Result**

No edit/delete options appear.

### **Screenshot**

<img width="1887" height="693" src="https://github.com/user-attachments/assets/5cb22359-5ce0-4d92-8557-2781858ed00e" />

---

## **BUG-06 — Console Logs Expose Internal Data**

**Portal:** Supervisor Portal  
**Module:** Dashboard / Record Sales  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Open **Dashboard** or **Record Sales**.
2. Press **F12 → Console**.
3. Inspect the logs.

### **Expected Result**

No internal or sensitive data should be logged in production.

### **Actual Result**

Console shows SKU lists, promodizer details, and other internal data.

### **Screenshot**

<img width="1914" height="584" src="https://github.com/user-attachments/assets/cc07ff65-2be7-417c-b500-e0c6fdeadb29" />

---

## **BUG-07 — Console Logs Display Internal Debug Messages**

**Portal:** Supervisor Portal  
**Module:** Dashboard / Record Sales  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

Same as **BUG-06**.

### **Expected Result**

No debug statements or internal messages should be printed.

### **Actual Result**

Internal console statements are printed.

### **Screenshot**

<img width="1914" height="584" src="https://github.com/user-attachments/assets/cc07ff65-2be7-417c-b500-e0c6fdeadb29" />

---

## **BUG-08 — No Login Required to Access Portal**

**Portal:** Supervisor Portal  
**Module:** Entire Portal  
**Severity:** Critical  
**Priority:** P1  

### **Steps to Reproduce**

1. Open the Supervisor Portal URL directly.

### **Expected Result**

System should require login and redirect to the login page.

### **Actual Result**

All pages are accessible without authentication.


----

----


#  Sales Analytics Dashboard — Consolidated Bug Report

---

## **BUG-01 — Console Logs Exposing Internal Data**

**Portal:** Sales Analytics Dashboard  
**Module:** SKU Performance  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Navigate to **SKU Performance** under the Sales Analytics Dashboard.
2. Open **DevTools → Console** and observe the logs.

### **Expected Result**

No internal data should be printed in the console.

### **Actual Result**

Internal data is being printed in the console.

### **Screenshot**

<img width="1884" height="680" alt="image" src="https://github.com/user-attachments/assets/1f120509-ce86-4163-b6fb-515dae326ca2" />

---

## **BUG-02 — Filters Accept Invalid Inputs**

**Portal:** Sales Analytics Dashboard  
**Module:** SKU Performance  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Navigate to **SKU Performance**, click on the search box in the filter.
2. Enter special characters.

### **Expected Result**

Special characters should not be accepted.

### **Actual Result**

Filter input accepts invalid characters.

### **Screenshot**

<img width="1885" height="616" alt="image" src="https://github.com/user-attachments/assets/18eefcff-faa7-42d1-bd4f-18482c76a196" />

---

## **BUG-03 — No Authentication Required**

**Portal:** Sales Analytics Dashboard  
**Module:** Entire Portal  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open the Sales Dashboard directly via its URL.

### **Expected Result**

User should be redirected to the login page.

### **Actual Result**

Dashboard loads without authentication.

---

## **BUG-04 — Data Mismatch Between Promodizer/Supervisor Sales and Charts**

**Portal:** Sales Analytics Dashboard  
**Module:** Dashboard  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. In the Supervisor/Promodizer portal, record some product sales.
2. Open Sales Analytics → Dashboard.
3. Select the date on which the sales were recorded.

### **Expected Result**

Charts should display the updated sales values.

### **Actual Result**

Charts show outdated static values only.

---

## **BUG-05 — Changing Chart Preference Does Not Update Dashboard Chart**

**Portal:** Sales Analytics Dashboard  
**Module:** Dashboard  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Go to **Settings → Dashboard Preferences**.
2. Change **Default Chart Type** to **Bar Chart** and save.
3. Open the Dashboard (date range: *1/10/2024 – 27/11/2025*).

### **Expected Result**

Dashboard should display a **Bar Chart**.

### **Actual Result**

Dashboard still displays a **Line Chart**.

---

## **BUG-06 — Staff Not Found**

**Portal:** Sales Analytics Dashboard  
**Module:** Staff Performance  
**Severity:** High  
**Priority:** P1  

### **Steps to Reproduce**

1. Navigate to **Staff Performance** and click any staff name.

### **Expected Result**

Staff performance details should be displayed.

### **Actual Result**

Displays **“Staff Not Found”**.

### **Screenshot**

<img width="1901" height="638" alt="image" src="https://github.com/user-attachments/assets/25ab7c8e-9a18-43ca-bcdb-a59421e83cbd" />

---

## **BUG-07 — UI Elements Overlap**

**Portal:** Sales Analytics Dashboard  
**Module:** Store Performance  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Open **Store Performance** and observe the UI under **Store Performance Data**.

### **Expected Result**

A scroll bar should appear to allow proper viewing.

### **Actual Result**

The **Table View** is not fully visible.

### **Screenshot**

<img width="1914" height="731" alt="image" src="https://github.com/user-attachments/assets/1b3a0b4b-ef2d-4e34-95ca-4e56f1db856f" />

---

## **BUG-08 — Data Loading Indefinitely**

**Portal:** Sales Analytics Dashboard  
**Module:** Staff Performance  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Staff Performance** and click any staff name.
2. Observe **Store Coverage** and **SKU Performance** sections.

### **Expected Result**

Data should load correctly.

### **Actual Result**

Sections remain stuck on **“Loading store coverage data…”**.

### **Screenshot**

<img width="1891" height="749" alt="image" src="https://github.com/user-attachments/assets/a1342488-52de-472d-9950-129a3d6e16fd" />

---

## **BUG-09 — Applied Filters Cannot Be Cancelled**

**Portal:** Sales Analytics Dashboard  
**Module:** Transaction History  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Open **Transaction History**.
2. Apply filters and attempt to cancel them.

### **Expected Result**

Filters should be removed.

### **Actual Result**

Filters remain applied.

### **Video**

[https://github.com/user-attachments/assets/9817077f-14ea-4683-aabd-c3ba8d6a7ea4](https://github.com/user-attachments/assets/9817077f-14ea-4683-aabd-c3ba8d6a7ea4)

---

## **BUG-10 — Validation Allows ‘Till’ Date Earlier Than ‘From’ Date**

**Portal:** Sales Analytics Dashboard   
**Module:** Transaction History, Staff Performance  
**Severity:** High  
**Priority:** P2  

### **Steps to Reproduce**

1. Go to **Transaction History**.
2. Enter a current date as the **From** date, then enter an earlier date as the **Till** date.

### **Expected Result**

Should show **“Enter Valid Date Range”**.

### **Actual Result**

Invalid date range is accepted.

### **Screenshot**

<img width="1909" height="447" alt="image" src="https://github.com/user-attachments/assets/ff041412-0b70-4bfe-aba3-8f23dfc47eb8" />

---

## **BUG-11 — Dashboard Preferences Not Reflected on Dashboard**

**Portal:** Sales Analytics Dashboard  
**Module:** Settings  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Settings → Dashboard Preferences**.
2. Unselect all **KPI Cards to Display on Dashboard**.
3. Open Dashboard.

### **Expected Result**

Unselected KPI cards should not be displayed.

### **Actual Result**

All KPI cards still appear.

### **Screenshot**

<img width="1574" height="579" alt="image" src="https://github.com/user-attachments/assets/a773c854-678d-4f70-b122-ca9c1b061842" />

---

## **BUG-12 — Changing Date/Time Format Does Not Reflect in UI**

**Portal:** Sales Analytics Dashboard  
**Module:** Settings  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Settings → Dashboard Preferences**.
2. Modify **Date Range Defaults** and **Date/Time Display Format**.
3. Open **Transaction History** and observe date formats.

### **Expected Result**

Updated formats should be applied across the UI.

### **Actual Result**

Old formats continue to display.

### **Screenshots**

<img width="1887" height="743" alt="image" src="https://github.com/user-attachments/assets/10f59bd5-5246-4352-8b7e-eddd5aa52cc4" />  
<img width="1891" height="775" alt="image" src="https://github.com/user-attachments/assets/d9966d88-072a-47b5-acc7-9816b76e9b51" />

---

## **BUG-13 — Sort Function Not Working for City and State Columns**

**Portal:** Sales Analytics Dashboard  
**Module:** Store Performance  
**Severity:** Medium  
**Priority:** P3  

### **Steps to Reproduce**

1. Navigate to **Store Performance**.
2. Click the sort button next to **City** or **State**.

### **Expected Result**

Data should sort in ascending/descending order.

### **Actual Result**

No action occurs.

### **Screenshot**

<img width="1543" height="577" alt="image" src="https://github.com/user-attachments/assets/0861e0a3-4d0c-49b3-86df-e219615f9457" />

---

## **BUG-14 — City Dropdown Does Not Respond**

**Portal:** Sales Analytics Dashboard  
**Module:** Store Performance  
**Severity:** Medium  
**Priority:** P3   

### **Steps to Reproduce**

1. Go to **Store Performance**.
2. Click the **City** filter dropdown.

### **Expected Result**

A list of cities should appear.

### **Actual Result**

No dropdown opens.

### **Screenshot**

<img width="1593" height="449" alt="image" src="https://github.com/user-attachments/assets/29a058b8-8b43-4caf-8478-182c13c0d45e" />

---

## **BUG-15 — Sales Volume Accepts Negative Values**

**Portal:** Sales Analytics Dashboard  
**Module:** Store Performance  
**Severity:** High  
**Priority:** P3  

### **Steps to Reproduce**

1. Go to **Store Performance** under **Sales Volume**.
2. Enter negative values in **Min** or **Max** fields.

### **Expected Result**

Negative input values should be rejected.

### **Actual Result**

Negative values are allowed.

### **Screenshot**

<img width="1538" height="421" alt="image" src="https://github.com/user-attachments/assets/7682188f-17ad-4ab5-8767-c836584b8ef5" />

---

## **BUG-16 — UI Fluctuates When Sorting**

**Portal:** Sales Analytics Dashboard  
**Module:** Transaction History  
**Severity:** Low  
**Priority:** P4  

### **Steps to Reproduce**

1. Navigate to **Transaction History**.
2. Sort different fields on the right panel.

### **Expected Result**

Sorting should occur smoothly.

### **Actual Result**

UI shifts **up and down** during sorting.

### **Video**

[https://github.com/user-attachments/assets/ca224b52-569e-40e2-934f-2bb0b14fd86c](https://github.com/user-attachments/assets/ca224b52-569e-40e2-934f-2bb0b14fd86c)

## **BUG-17 — Data Leakage Of Stores**

**Portal:** Sales Analytics Dashboard   
**Module:** Store Performance  
**Severity:** Critical  
**Priority:** P1  

### **Steps to Reproduce**

1. Navigate to **Store Performance**.
2. In sales volume enter values (eng:  1000, 2000, 3456789)

### **Expected Result**

Should not show any Store information.

### **Actual Result**

Shows all stores information.

### **Screenshot**

<img width="1869" height="830" alt="image" src="https://github.com/user-attachments/assets/eb7be879-305a-4cb5-a31b-9325b14dfdfb" />




