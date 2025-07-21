# Reviews Dashboard

This is a static HTML dashboard for displaying customer reviews from a Google Sheet. It includes filtering, charting, and archived review support.

## 🚀 Features

- Live data from a public Google Sheet (CSV format)
- Rating-based filters
- Archived reviews toggle
- Average rating & total count
- Chart visualization with Chart.js
- Premium Apple-style design

## 📄 Google Sheet Setup

1. Ensure your sheet includes the following columns:
   - `Date`
   - `Customer Name` or `Customer`
   - `Rating`
   - `Customer Doma Content`
   - `Archived At` (optional)

2. File → Share → Publish to web → CSV format
3. Copy the public CSV URL and update this line in `index.html`:

```js
loadCSVFromGoogleSheet('https://docs.google.com/spreadsheets/d/e/your-export-link/pub?output=csv');
