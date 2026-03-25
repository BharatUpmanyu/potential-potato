# Flour Mill Sack Manager

A browser-based app to manage customer wheat sacks in your flour mill.

## What it solves

Instead of tracking sacks in a notebook, this app lets you store each entry digitally and update delivery/payment states in a few clicks.

## Features

- Add sack entries with:
  - Customer name
  - Weight (kg)
  - Purpose (`Aatta` or `Daliya`)
- Automatic payable calculation:
  - `Aatta`: ₹3 per kg
  - `Daliya`: ₹1.5 per kg
  - Payable amount is shown in the entry form and next to each customer entry
- Track and update status clearly:
  - `Pending Delivery`
  - `Delivered`
  - `Paid`
  - `Payment Pending` (delivered but unpaid)
- Edit existing entries
- Delete entries with confirmation
- Search by customer name
- Filter by status
- Export visible entries to CSV
- Dashboard counters:
  - Visible entries
  - Delivered
  - Paid
  - Payment pending
  - Total visible weight (kg)
- Data persistence using browser `localStorage`

## Run

No installation required.

1. Open `index.html` in a modern browser.
2. Add and manage customer sack entries.

> Note: Data is stored only in the browser/device where you use the app.
