# 🧾 A.T Commodities – Monthly Profit & Loss (PNL) App

A responsive HTML-based web application for **A.T Commodities (Coal & Minerals Trading Company)** to manage monthly Profit & Loss reports with data entry, summary calculations, and export options (CSV & PDF).

---

## ⚙️ Features

1. **Monthly Purchases Tracker**

   * Record all coal or mineral purchases.
   * **Inputs:** Date, Vehicle Number, Supplier Name, Quantity (MT), Price per Ton.

2. **Monthly Sales Tracker**

   * Record all monthly sales.
   * **Inputs:** Date, Vehicle Number, Customer Name, Quantity (MT), Price per Ton.

3. **Gross Profit Calculator**

   * Automatically computes **Gross Profit = Total Sales − Total Purchases** for the selected month.

4. **Monthly Expenses Manager**

   * Record all expenses via vouchers.
   * **Inputs:** Voucher No, Date, Narration, Amount.
   * Displays all vouchers for the month with **total expense**.

5. **Net Profit Summary**

   * Calculates **Net Profit = Gross Profit − Total Expenses.**

6. **Report Management**

   * Save all records in browser **Local Storage**.
   * Export data to **JSON file** to continue later or share between systems.
   * Import previously saved JSON files.
   * Export the full monthly report to **CSV** or **PDF**.
   * Generate a clean **Printable View** for physical records.

---

## 🖥️ How to Use

### 1. Open the App

* Simply open the HTML file in your browser (`AT_Commodities_Monthly_PNL_App.html`).
* Works offline once loaded.

### 2. Select the Month

* Use the **Month Selector** at the top (e.g., 2025-10).
* All entries will be stored separately per month.

### 3. Add Data

* Use the **Purchases**, **Sales**, and **Expenses** sections to enter data.
* Click **Add Entry** after filling the required fields.
* Entries appear instantly in the tables below.

### 4. View Summaries

* The app automatically calculates:

  * Total Purchases
  * Total Sales
  * Gross Profit
  * Total Expenses
  * Net Profit

### 5. Save & Continue Later

* Click **Save (Local)** to store data in browser storage.
* You can close and reopen the file anytime — data remains saved.

### 6. Export / Import Data

* **Export JSON:** Download current month’s data for backup or transfer.
* **Import JSON:** Load previously saved report file to continue editing.

### 7. Generate Reports

* **Export CSV:** Download a spreadsheet version (for Excel).
* **Download PDF Report:** Generates a formatted PDF (includes all tables and totals).
* **Print Report:** Opens a printer-friendly view (you can save as PDF from print dialog too).

---

## 🧩 PDF Report

* The **“Download PDF Report”** button creates a ready-to-print **A4 PDF file** using `html2pdf.js`.
* The PDF includes:

  * Company name and report month.
  * Purchases, Sales, Expenses, and Profit summaries.
* File is automatically named like:

  ```
  AT_Commodities_PNL_YYYY-MM.pdf
  ```

  Example: `AT_Commodities_PNL_2025-10.pdf`

---

## 💾 File Handling Tips

* Always export a backup JSON file monthly for records.
* Data is saved per month and isolated (you can manage multiple months separately).
* If using on multiple systems, import/export JSON for portability.

---

## 🛠️ Technical Info

* Built with **HTML, CSS, JavaScript**.
* Uses **html2pdf.js** for PDF export and **LocalStorage** for saving data.
* Works entirely offline — no server required.
* Mobile and desktop responsive design.
