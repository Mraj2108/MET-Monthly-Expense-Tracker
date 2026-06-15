# Ledger — Monthly Expense Tracker

A single-page expense tracker with budgets (per-category caps shown as gauge bars), month switching, month-over-month comparison chart, and JSON/CSV export-import. Currency is INR (₹). All data is stored in your browser's `localStorage` — nothing is sent anywhere.

## Run it locally
Just open `index.html` in any browser. No build step, no server.

## Host it on GitHub Pages

1. Create a new repository on GitHub (e.g. `expense-tracker`).
2. Upload `index.html` to the repo (drag-and-drop on the GitHub web UI works, or use git):
   ```bash
   git init
   git add index.html
   git commit -m "Add expense tracker"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to "Deploy from a branch", branch `main`, folder `/ (root)`. Save.
5. After a minute, your app will be live at:
   ```
   https://<your-username>.github.io/<repo-name>/
   ```

## Notes
- Data is per-browser (localStorage). Use **Export JSON** regularly to back up, and **Import JSON** to move data between devices/browsers.
- **Export CSV** gives you the current month's transactions for use in Excel/Sheets.
- Add categories and set monthly budget caps in the "Manage budgets & categories" panel — budgets show as horizontal gauges with a tick marking current spend.
