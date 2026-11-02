# ShelfLife — UPC Scanner & Expiration Tracker

A mobile-friendly web app for scanning product barcodes (UPC/EAN, Code 128, QR and more) with the phone camera and tracking expiration dates.

## Features
- Live camera barcode scanning (plus scan-from-photo, manual entry, and USB/Bluetooth scanner support)
- Automatic product name/photo lookup via Open Food Facts; names you enter are remembered per barcode
- Expiration date, quantity, location and lot tracking
- Dashboard: expired / urgent / soon / good, with search, location filter, and sorting
- "Save & scan next" for fast stocking, −1 / Done to use up stock, undo delete
- CSV export/import, adjustable warning windows, optional device alerts

## Hosting
It's a single static `index.html`. Enable **GitHub Pages** (Settings → Pages → Deploy from branch → `main` / root) and open `https://<user>.github.io/<repo>/` on your phone. The camera requires HTTPS, which GitHub Pages provides.

Data is stored in the browser on each device (localStorage). Use Export CSV for backups.
