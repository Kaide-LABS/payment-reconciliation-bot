# Payment Reconciliation Bot

## Problem

Operations teams at waste-management companies manually cross-referenced payment portal records with internal Google Sheets, a tedious and error-prone process that delayed reconciliation and increased the risk of missed or duplicate payments.

## Approach

- Automated headless browser login and session management using Selenium with Chrome, handling credential entry, wait conditions, and cookie extraction.
- Scraped paginated DataTable transaction records (up to 500 rows per page) from the TrackItPay portal, normalising dates and currency amounts for consistent matching.
- Integrated with Google Sheets via the gspread API and OAuth2 service-account credentials to clear and refresh the reconciliation sheet with sorted, deduplicated transaction data.

## Results

- Reduced a manual copy-paste reconciliation workflow to a single automated script execution.
- Scrapes, normalises, and uploads up to 500 transactions per run, sorted chronologically, with full logging and error handling.

## How to Run

```
pip install -r requirements.txt
python reconciliation_bot.py
```
