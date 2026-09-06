4.) # Automating Payment Reconciliation for Non-Tech Savvy Mom

**Context & Challenge**

My mother runs a waste management business servicing commercial clients, with transactions logged through a payment portal. However, the platform had significant usability challenges:

- Displayed only 25 transactions at a time, crashing beyond 500 entries.
- Excessive technical jargon and unnecessary data fields (invoice numbers, payment gateways) cluttered the interface, complicating her reconciliation process.
- Navigating the website was cumbersome, especially for non-tech savvy users.

This required manual reconciliation efforts, consuming significant time and increasing the potential for human error.

**Approach**

- **Automated Web Scraping:**
    - Utilized Selenium and BeautifulSoup to systematically scrape transactions directly from the payment portal.
    - Bypassed the website’s inherent limitations by programmatically selecting transaction counts manageable by JSON responses.
- **Simplified Data Structuring:**
    - Extracted and cleaned essential transaction details only (dates, amounts, payer details), removing irrelevant technical fields to streamline reconciliation.
- **Google Sheets Integration:**
    - Automatically populated a structured, clear, and simplified Google Sheet.
    - Implemented automated sorting and date-based organization to enhance clarity and ease of use.

**Outcome**

The solution drastically simplified the reconciliation process, eliminating the need for navigating cumbersome web pages. This automation significantly reduced both my mother's stress and my own manual workload, providing a robust and user-friendly method of managing transaction records.
