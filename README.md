# Fusion Security Lab

## What I did today (Day 1)
- Opened Security Console successfully
- Inspected my user roles:
  - Application Implementation Consultant
  - IT Security Manager
  - Employee
- Explored seeded role: Employee
  - Interesting Duty: Employee Self-Service Duty
  - Notable Function Security Policy: View Person Profile → allows employee to view their own profile
  - Notable Data Security Policy: Access to Person Records → restricts access so user sees only their own data

## Notes to self
- Role Hierarchy shows which duties a role inherits
- Function Security Policies control **what tasks/actions** a user can perform in UI
- Data Security Policies control **what data** a user can access (e.g., only their own department)
- Missing roles: none for now (I already have IT Security Manager + AIC)

## Next up
- Create a small custom role and assign it to a test user

## Screen shots
- <img width="1919" height="949" alt="Screenshot 2025-08-22 141310" src="https://github.com/user-attachments/assets/07642829-55b2-4eb9-9262-0a6d93ba7336" />
- <img width="1911" height="947" alt="Screenshot 2025-08-22 141346" src="https://github.com/user-attachments/assets/eebbf2f7-3143-4038-ab28-3bbbab95a2bb" />
- <img width="1919" height="950" alt="Screenshot 2025-08-22 142104" src="https://github.com/user-attachments/assets/ec120118-aad2-44d3-830d-ee4068dddace" />
- <img width="1919" height="949" alt="Screenshot 2025-08-22 142134" src="https://github.com/user-attachments/assets/5907d462-a82e-4bc9-82ef-1fabb9158203" />


## Day 1 (Part 2) – Custom Role and Test User

- Created custom role: XX_CUSTOM_EMPLOYEE_ROLE
  - Added Function Security: View Person Profile
  - Added Data Security: View own Person record
 
- Created new test user: TEST_EMPLOYEE1
 
- Assigned custom role to the test user

## Screen shots
- <img width="1916" height="937" alt="Screenshot 2025-08-22 151823" src="https://github.com/user-attachments/assets/02a4cdf7-1235-4387-a9e9-622d8ce40a71" />
- <img width="1826" height="989" alt="Screenshot 2025-08-22 161330" src="https://github.com/user-attachments/assets/85196f08-e5f8-423c-8471-e79f21a5ee6e" />
- <img width="1650" height="828" alt="Screenshot 2025-08-22 155658" src="https://github.com/user-attachments/assets/28e11640-4f22-4667-a864-6c09edb3482e" />



# 📅 Day 1 – Oracle Fusion BI Publisher Basics & First Report

## 🎯 Objective
- Understand BI Publisher (BIP) in Fusion Applications.
- Create a **Data Model** using SQL.
- Build **two layouts** → RTF (Word) and Excel.
- Run and export the report in **PDF, Excel, HTML**.
- Save work in GitHub as part of my learning portfolio.

---

## 📝 Key Concepts
- **BI Publisher = Data Model + Layout**
  - Data Model → Defines the data (SQL, Subject Areas, Web Services).
  - Layout → Defines how it looks (RTF, Excel, HTML, PDF).
- **Real-World Use Cases**:
  - Invoices, PO, Payslips, Employee Reports.
  - Bursting outputs to Email, FTP, UCM.
  - Automating scheduled reports for Finance/HR teams.

---

# 📅 Day 1 – Oracle Fusion BI Publisher (BIP) Basics

## 🎯 Objective
Learn BI Publisher fundamentals in Fusion with **hands-on practice**:
- Create a **Data Model** using SQL.
- Build **RTF (Word)** and **Excel** layouts.
- Export reports in **PDF, Excel, HTML**.
- Document and upload all artifacts to GitHub.

---

## 📝 Key Concepts
- **BI Publisher (BIP)** = Data Model + Layout.
  - **Data Model** → Defines what data you fetch (SQL, subject areas, web service).
  - **Layout** → Defines how the data is presented (RTF, Excel, PDF, HTML).
- **Why companies use BIP**:
  - To build/customize Invoices, POs, Payslips, Financial Reports.
  - To automate report delivery (Email, FTP, UCM).
  - To customize layouts according to client needs.

---

## 🛠️ Practical Work

### 1️⃣ Create Data Model
1. Navigate → **Reports and Analytics → Browse Catalog → New → Data Model**.
2. Add Data Set → Choose **SQL Query**.
3. Paste SQL:

```sql
SELECT INVOICE_ID,
LAST_UPDATE_DATE,
LAST_UPDATED_BY,
VENDOR_ID,
INVOICE_NUM
FROM ap_invoices_all
where ROWNUM <= 10

<img width="1914" height="1004" alt="Screenshot 2025-08-29 143823" src="https://github.com/user-attachments/assets/3935b101-2185-4a3c-835d-334e3279c25e" />

### 2️⃣ RTF Layout

**Steps:**

1. From Data Model → **Create Report → RTF Layout**  
2. Export sample XML → Open in **MS Word + BI Publisher plugin**  
3. Insert a table → Map fields:  
   - Invoice Num  
   - Invoice Date  
   - Supplier Name  
   - Amount  
4. Save as: `RPT_InvoiceList_RTF.rtf`  
5. Upload in Fusion Catalog → `/Custom/Training/RPT_InvoiceList_RTF.xdo`
<img width="1785" height="923" alt="Screenshot 2025-08-29 144902" src="https://github.com/user-attachments/assets/dd9721b5-415a-45fc-836d-c367efef2d77" />

### 3️⃣ Excel Layout

**Steps:**

1. From Data Model → **Create Report → Excel Layout**  
2. In Excel → Add headers:  
   - Invoice Num  
   - Invoice Date  
   - Supplier Name  
   - Amount  
3. Map fields to columns  
4. Save as: `RPT_InvoiceList_Excel.xlsx`  
5. Upload in Fusion Catalog → `/Custom/Training/RPT_InvoiceList_Excel.xdo`
<img width="1919" height="1074" alt="Screenshot 2025-08-29 145352" src="https://github.com/user-attachments/assets/33b674cb-58b1-4cbb-bae7-2b7dbf6a89ee" />

### 4️⃣ Run Report & Export Outputs

**Steps:**

1. Run the report in Fusion  
2. Export outputs:  
   - 📄 **PDF** → `report-output-pdf.png`  
   - 📊 **Excel** → `report-output-excel.png`  
   - 🌐 **HTML** → `report-output-html.png`


<img width="1847" height="996" alt="image" src="https://github.com/user-attachments/assets/f548cf74-42ec-4abb-a073-f5f0cdf18dd6" />



