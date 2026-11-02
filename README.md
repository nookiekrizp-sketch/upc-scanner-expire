# ShelfLife — Barcode Expiration Tracker

Live app: https://nookiekrizp-sketch.github.io/upc-scanner-expire/

Scan product barcodes with your phone camera (or a USB/Bluetooth scanner), record expiration dates, and know what to pull before it expires. All data stays on the device (browser storage). Use Settings → Backup to save a copy.

## Features
- Live camera scanning (UPC, EAN, Code 128/39, QR, and more), with flashlight, zoom, beep and vibration
- USB / Bluetooth barcode scanners work too: just scan on the main screen
- Product name and description: from your JSS item list first, then Open Food Facts / Beauty / Products / Pet Food
- Quick dates, quantity, location, lot, cost, "Save & scan next"
- **Pull list**: expired and soon-to-expire items grouped by location, printable, with Mark down and "Pull all expired as waste"
- **Remove**: sold/used or wasted/expired, partial quantities, undo
- **Reports**: units wasted, waste $, waste rate, most-wasted items, activity export
- Installable app (Add to Home Screen) that works offline; expiry alerts

## Working with JSS (POS / inventory)
1. **Import your item list**: in JSS, export your item/product list as CSV (or open it in Excel and Save As CSV). In ShelfLife, open **JSS / POS → Import item list**, check the column matching (UPC, description, SKU/Item #, department, cost, price), and tap Import. Scanned barcodes now show your own names, SKUs, departments and prices. Leading zeros and missing check digits are handled.
2. **Send adjustments back**: **JSS / POS → Download new adjustments** creates a CSV with `date, upc, sku, item_name, quantity, adjustment_qty, reason, unit_cost, extended_cost, location, lot, expiration`. Import it into JSS's inventory adjustment / shrink screen. Reasons are `Spoilage/Expired` or `Sold/Used`.
3. **Full inventory export/import** for counts and reconciliation.
