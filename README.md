# 🔄 TallyConverter

### Professional Excel → Tally XML Converter for TallyPrime & Tally.ERP 9

**Designed and Made by Santhosh**

TallyConverter is a browser-based accounting utility that converts **Excel and CSV accounting data into Tally-compatible XML**, with built-in ledger mapping, bank statement classification, financial verification, and Tally import preparation.

🚀 **Live Application:**
[TallyConverter — Live on GitHub Pages](https://santhosh-sampath-kumar.github.io/tally-converter/?utm_source=chatgpt.com)

> **100% Client-Side • No Server Uploads • Fast • Private**

---

## ✨ Features

### 🏦 Bank Statement Formatter

Convert raw bank statements into structured Tally voucher data.

The Bank Statement Formatter can:

* Import `.xlsx`, `.xls`, and `.csv` bank statements
* Support multi-sheet Excel workbooks
* Automatically detect statement columns
* Map Date, Bank Account, Withdrawal, Deposit, Narration and Party/Transaction fields
* Classify transactions into:

  * 🟢 Receipts
  * 🔴 Payments
  * 🔄 Payment Contra
  * 🔄 Receipt Contra
* Identify inter-bank transfers automatically
* Generate a standardized **8-column Tally voucher format**
* Export the formatted data back to Excel
* Send the formatted data directly into the main converter

---

## 📊 Excel / CSV → Tally XML

Convert accounting spreadsheets into Tally-ready XML through a guided workflow.

### Step 1 — Upload

Upload your accounting spreadsheet using:

* Drag & Drop
* File Browser
* Excel `.xlsx`
* Excel `.xls`
* CSV
* Multiple files
* Direct Excel paste using `Ctrl + V`

The application also provides a **live spreadsheet preview** so you can verify your imported data before conversion.

---

### Step 2 — Column Mapping

TallyConverter automatically detects and maps spreadsheet columns.

You can review or manually adjust:

* Voucher Number
* Date
* Debit Ledger
* Debit Amount
* Credit Ledger
* Credit Amount
* Narration
* Other relevant accounting fields

It also provides optional Tally ledger defaults such as:

* Company Name
* Sales Ledger
* Purchase Ledger
* Bank Ledger
* CGST Ledger
* SGST Ledger
* IGST Ledger
* Round Off Ledger

---

### Step 3 — Ledger Matching

Extracted ledgers can be reviewed and matched against an existing **Tally Chart of Accounts**.

Features include:

* Import existing Tally ledger lists
* Smart ledger matching
* Ledger de-duplication
* Search and review
* Suggested ledger matches
* Existing vs. new ledger identification
* Opening balance handling
* Parent group assignment

The converter supports **28 official Tally groups** for ledger classification.

---

### Step 4 — Preview & Financial Verification

Before generating XML, review your transactions and verify the accounting impact.

The application provides:

* Voucher-level preview
* Receipt / Payment / Contra classification
* Debit and credit verification
* Inter-bank contra identification
* Contra filtering and deletion
* Ledger-wise financial audit
* Trial Balance review
* Profit & Loss review
* Balance Sheet ledger review
* Closing balance verification

This helps identify accounting issues **before importing the data into Tally**.

---

### Step 5 — Generate Tally XML

TallyConverter generates two XML files:

#### 1️⃣ Ledgers Master XML

Import this file **first** into Tally.

It creates the required ledgers and groups.

#### 2️⃣ Vouchers XML

Import this file **second** into Tally.

It posts the converted accounting transactions.

---

## 🧾 Compound Journal Entries

TallyConverter supports **multi-ledger / compound journal entries**.

For example:

```text
Office Rent                 Dr ₹20,000
Electricity Charges        Dr ₹5,000
       To HDFC Bank                   ₹25,000
```

Multiple debit or credit lines can belong to the same voucher.

You can also use **blank continuation rows** in Excel to visually group multiple lines under the same voucher.

Example:

| Voucher No | Date       | Debit Ledger    | Debit Amount | Credit Ledger | Credit Amount |
| ---------- | ---------- | --------------- | -----------: | ------------- | ------------: |
| JV-004     | 31-03-2026 | Stationery Exp  |       ₹3,200 |               |               |
|            |            | Courier Charges |         ₹800 |               |               |
|            |            |                 |              | Petty Cash    |        ₹4,000 |

The converter automatically associates blank continuation rows with the voucher above.

---

## 🔐 Privacy & Security

TallyConverter is designed with a **privacy-first architecture**.

### 100% Client-Side Processing

Your accounting files are processed directly inside your browser.

**Your Excel/CSV data is not uploaded to a backend server.**

There is:

* ❌ No accounting data server
* ❌ No cloud database
* ❌ No external file upload
* ❌ No server-side conversion

Your financial data remains in the browser during processing.

---

## 🔒 PIN Security

The application includes client-side PIN authentication using:

* SHA-256 hashing
* Unique cryptographic salt
* Native Web Crypto API

Authentication is handled locally within the application.

---

## 🎨 Modern Interface

TallyConverter includes a clean accounting-focused interface with:

* ☀️ Light Mode
* 🌙 Dark Mode
* 📊 Live spreadsheet preview
* 🖥️ Desktop-style application interface
* 📱 Responsive layout
* ⚡ Fast browser-side processing

---

## 🧮 Built-in Accountant Calculator

A floating calculator is available throughout the application.

Features include:

* Basic arithmetic
* GST shortcuts

  * +5%
  * +12%
  * +18%
* Percentage calculations
* Copy result
* Paste values
* Calculation tape/history

Designed for quick calculations while working through accounting data.

---

# 🔄 Conversion Workflow

```text
                 ┌─────────────────────┐
                 │   Excel / CSV File   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Upload & Preview  │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Column Mapping    │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │   Ledger Matching   │
                 │  & Group Mapping   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │ Preview & Verify    │
                 │ TB / P&L / Audit    │
                 └──
```
