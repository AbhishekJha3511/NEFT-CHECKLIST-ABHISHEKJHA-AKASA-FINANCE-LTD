# NEFT Checklist & Verification System

## THIS IS A PART OFF MY SIDE PROJECTS

A web-based **NEFT Verification and Disbursement Management System** designed to simplify loan verification, D.O. data fetching, disbursement calculations, and NEFT preparation.

## Features

### 🔎 D.O. Sheet Fetch

- Fetch D.O. details directly from Google Sheets.
- Search using D.O. Number.
- Live Google Apps Script API integration.
- Fast D.O. lookup using server-side caching.
- Automatically populates required customer, dealer, loan, EMI, and registration information.

### 📋 File Data

Displays information fetched from the D.O. Sheet, including:

- D.O. Number
- Customer Name
- Lead Number
- Area
- Sales Executive
- Mobile Number
- Dealer
- Dealer Code
- Registration Type
- Vehicle Price
- Down Payment
- Loan Amount
- File Charge
- EMI
- Tenure
- Advance EMI
- Advance EMI Amount
- Advance Interest
- Guarantor
- Co-applicant
- Other required verification information

### 💰 Disbursement Amount Calculator

Automatically calculates the final disbursement amount using the fetched D.O. information.

Supports:

- Loan Amount
- File Charges
- Advance EMI Amount
- Advance Interest Amount
- Life Insurance
- Registration type
- Down payment
- Final disbursement amount

### 🏦 NEFT Verification

Provides a structured checklist for NEFT verification and preparation.

Includes:

- Dealer account information
- Dealer IFSC
- NEFT amount
- Disbursement information
- Verification fields
- Required documents
- Status indicators

### 📅 Automatic Dates

The system automatically calculates:

#### NEFT Send Date

The NEFT send date is calculated automatically based on the configured date rules.

#### First EMI Due Date

The first EMI date is automatically calculated based on the D.O. date rules.

### ⏱️ Fetch Timer

A fixed **15-minute timer** is available for each fetch session.

Behavior:

- Starts when the Fetch button is clicked.
- Timer duration: **15 minutes**
- At 10 minutes: background blinks 3 times.
- At 15 minutes: timer stops automatically.
- Reset button is available as an icon.

### 🗑️ Clear Fetched Data

The clear button only removes information fetched from the live Google Sheet.

It does **not** modify:

- HTML-stored data
- Embedded/local DO Sheet data
- Stored configuration
- Project files
- Google Sheet data

This allows the next D.O. to be fetched without modifying the application's stored data.

---

# Technology Stack

- HTML5
- CSS3
- JavaScript
- Google Sheets
- Google Apps Script
- Fetch API
- GitHub

---

# Project Structure

```text
NEFT-Checklist/
│
├── NEFT_Checklist_Updated.html
├── README.md
└── ...
