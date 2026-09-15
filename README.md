# Sales Tracker in Google Sheets

## Project Overview

The Sales Tracker is a lightweight Google Sheets spreadsheet designed to record sales data and automatically calculate daily, weekly, and monthly sales totals.

This project was completed as part of the HI PALVAI – Data Analytics Track.

## Objective

To practice spreadsheet structuring, automated calculations, data validation, and sales data aggregation using Google Sheets.

## Tools Used

* Google Sheets
* Spreadsheet formulas
* Data validation and dropdown lists

## Spreadsheet Structure

### 1. Raw Data

The Raw Data sheet contains the following columns:

| Column      | Description             |
| ----------- | ----------------------- |
| Date        | Date of the sale        |
| Order ID    | Unique order identifier |
| Product     | Name of the product     |
| Category    | Product category        |
| Quantity    | Number of units sold    |
| Unit Price  | Price per unit          |
| Total Sales | Quantity × Unit Price   |

### 2. Summary

The Summary sheet displays:

* Overall total sales
* Daily sales totals
* Weekly sales totals
* Monthly sales totals

## Important Formulas

**Total Sales per Order**

```excel
=E2*F2
```

**Overall Total Sales**

```excel
=SUM('Raw Data'!G2:G)
```

**Daily Sales**

```excel
=SUMIF('Raw Data'!A:A,A7,'Raw Data'!G:G)
```

**Unique Dates**

```excel
=UNIQUE('Raw Data'!A2:A)
```

## Data Validation

Data validation was added to improve data accuracy:

* Quantity: Values greater than or equal to 1.
* Category: Dropdown options including Electronics, Accessories, and Furniture.

## Sample Results

The tracker contains 7 sample sales orders.

| Metric              |    Result |
| ------------------- | --------: |
| Overall Total Sales | ₹1,75,500 |
| Weekly Sales        | ₹1,75,500 |
| Monthly Sales       | ₹1,75,500 |

## Key Learnings

* Structuring raw sales data in a spreadsheet.
* Using formulas for automatic calculations.
* Creating daily, weekly, and monthly summaries.
* Applying data validation to prevent incorrect entries.
* Organizing a data analytics project for GitHub submission.

## Conclusion

The Sales Tracker demonstrates how Google Sheets can be used to organize sales records and generate automated summaries for ongoing sales tracking.

## Project Files

* `Sales_Tracker.xlsx` – Exported spreadsheet.
* `Sales_Tracker_Report.pdf` – Task report with screenshots, formulas, and results.
