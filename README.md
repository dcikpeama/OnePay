Short Description

- Local, privacy-first OnePay statement parser that restores powerful filtering and CSV export directly in your browser. Drop in PDFs, filter by date/account/type/amount/description, and export results — no backend, no data leaves your machine.

Long Description

- This project processes OnePay PDF statements entirely on your device to give you rich filtering and export capabilities that the native OnePay UI doesn’t provide. It uses robust text parsing and dynamic column detection to reliably extract transactions (including multi-line and cross-page descriptions), supports multi-file processing, and lets you export filtered results to CSV.
  
Key Features

- Advanced filtering by date, account, transaction type, amount, and free-text description.
- CSV export of filtered transactions with a date-stamped filename.
- Multi-statement processing (select multiple PDFs at once).
- Privacy-first: parsing runs in your browser only; no data is sent anywhere.
- Resilient parsing for OnePay PDFs: dynamic column detection and nearest-neighbor clustering to handle split lines and layout shifts.

How It Works

- Load one or more OnePay PDF statements.
- The app extracts transaction lines and normalizes columns (Date, Account, Description, Type, Amount).
- Use search and account filters to narrow results.
- Click Export CSV to save the current filtered view.

Tech Stack

- JavaScript, HTML, CSS
- PDF.js (client-side PDF text extraction)
- No backend services or external data storage

Why

- OnePay’s UI lacks filtering by several useful fields; this tool restores those capabilities and adds CSV export for analysis and bookkeeping, while keeping your data local.
  
Limitations

- Optimized for OnePay statement formats; major template changes may require parser updates.
- Heuristic parsing can occasionally need tuning for edge-case layouts.
