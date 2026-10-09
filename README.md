# 🛒 DukaanPOS — Modern Retail, Garments & General Store POS

[![Latest Release](https://img.shields.io/github/v/release/sus4400/DukaanPOS-releases?color=blue&label=Latest%20Version)](https://github.com/sus4400/DukaanPOS-releases/releases/latest)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%20%2F%2011%20(64--bit)-0078D6?logo=windows)](https://github.com/sus4400/DukaanPOS-releases/releases)
[![Runtime](https://img.shields.io/badge/.NET-8.0%20(Self--Contained)-512BD4?logo=dotnet)](https://github.com/sus4400/DukaanPOS-releases/releases)
[![Database](https://img.shields.io/badge/Database-SQLite%20(Offline--First)-003B57?logo=sqlite)](https://github.com/sus4400/DukaanPOS-releases)
[![AI Assistant](https://img.shields.io/badge/AI%20Assistant-Google%20Gemini%20%7C%20OpenRouter-4285F4)](https://github.com/sus4400/DukaanPOS-releases)

**DukaanPOS** is an intelligent, high-speed, offline-first Point of Sale (POS) and inventory management software engineered specifically for **clothing boutiques, garment shops, retail outlets, footwear stores, and general merchants**. 

Built with modern .NET 8 WPF technology, it delivers lightning-fast counter billing, matrix inventory tracking (Size/Color/Design), automated customer & supplier ledgers (Khata), thermal receipt printing, and a built-in **AI Store Assistant**.

---

## 🚀 Key Features at a Glance

### 1. ⚡ Fast Point of Sale & Checkout
- **Instant Barcode Scanning:** Scan barcodes or design codes with zero latency.
- **Split Payments:** Accept payments across **Cash**, **Card**, and **Credit (Customer Khata / Udhar)** in a single transaction.
- **Item Returns & Exchanges:** Hassle-free return processing with automated stock restock and cash refund or credit adjustment.
- **Hold Carts:** Park transactions when a customer needs to pick additional items, and resume anytime.
- **Discounts & Custom Pricing:** Apply invoice-level or item-level percentage/flat discounts with manager authorization.

### 2. 👗 Garments & Retail Variant Inventory
- **Product Matrix Variants:** Manage clothing and retail items with flexible **Size, Color, Fabric, and Design Code** combinations.
- **Low Stock Alerts:** Automated warnings when items reach or drop below their minimum stock threshold.
- **Barcode Generation:** Integrated barcode label printing compatible with all standard barcode label printers.
- **Inventory Valuation:** Real-time valuation metrics showing **Total Active Units, Total Cost Value, Total Retail Value, and Expected Gross Margin**.

### 3. 📒 Customer Khata (Accounts Receivable)
- **Customer Credit Accounts:** Maintain complete credit profiles with credit limits and outstanding receivables.
- **Ledger Statement History:** Detailed transaction log of purchases, partial payments, and remaining balances.
- **Payment Collection:** Issue official payment receipts when customers clear their credit accounts.
- **Debtor Reports:** One-click debtor summary sorted by highest outstanding balance.

### 4. 🏢 Supplier & Party Khata (Accounts Payable)
- **Purchase Tracking:** Record stock purchases with cost prices, supplier invoice numbers, and payment terms.
- **Debit / Credit Party Ledger:** Full running balance ledger for fabric vendors and wholesale suppliers.
- **Payables Summary:** Real-time visibility into total supplier payables and due dates.

### 5. 🤖 Built-in AI Store Assistant (BYOK)
- **Bring Your Own Key:** Supports free **Google Gemini** keys and **OpenRouter** keys (GPT-4o, Claude 3.5 Sonnet, Llama 3.3).
- **Live Database Intelligence:** Ask natural business questions and receive live calculations directly from your store database:
  - *"Today's sales summary"*
  - *"Which items are currently low on stock?"*
  - *"How much profit did we make today?"*
  - *"Aaj ki total sale kitni hai?"* (Full support for English & Roman Urdu)
  - *"Who owes us the most money?"*
- **Privacy First:** Your API keys are encrypted locally using Windows DPAPI. Your database is never uploaded to third-party servers.

### 6. 👥 Staff, Cashiers & Attendance
- **Role-Based Access:** Granular permissions for **Admin**, **Cashier**, and **Salesperson**.
- **Attendance Logging:** Daily digital Check-In and Check-Out tracking.
- **Sales Commission Tracking:** Attribute sales receipts to specific salespeople to calculate daily performance and commissions.

### 7. 💸 Operating Expenses & Cash Drawer
- **Daily Petty Cash:** Log day-to-day store expenses (utilities, tea, transport, maintenance) by category.
- **Day-End Cash Reconciliation:** Compare physical cash in drawer against system sales before closing the day.

### 8. 🖨️ Thermal Printing & Hardware Support
- **ESC/POS Thermal Printers:** Native support for standard **58mm (2-inch)** and **80mm (3-inch)** thermal receipt printers.
- **Custom Receipt Layouts:** Print your custom store logo, address, phone number, and exchange policy notes.
- **Auto-Cut & Cash Drawer Kick:** Automatic receipt cutting and RJ11 cash drawer trigger on payment completion.
- **Peripherals:** Compatible with all standard USB, Bluetooth, and wireless 1D/2D barcode scanners.

---

## 🖥️ System Requirements

| Specification | Minimum | Recommended |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 (64-bit, Build 1809+) | Windows 11 (64-bit) |
| **Processor** | Intel Core i3 / AMD Ryzen 3 | Intel Core i5 / AMD Ryzen 5 or higher |
| **RAM** | 4 GB | 8 GB or more |
| **Storage** | 500 MB free disk space | High-speed SSD |
| **Display** | 1366 x 768 resolution | 1920 x 1080 (Full HD) |
| **Printers** | Any ESC/POS 58mm or 80mm USB Thermal Printer | Auto-cut 80mm Thermal Printer |
| **Barcode Scanner** | Any standard USB Plug-and-Play Scanner | Handheld 2.4G Wireless Barcode Scanner |

---

## 📥 Installation & Setup Guide

### Step 1: Download
Download the latest setup installer (`DukaanPOS-Setup-x.x.x.exe`) from the [**Releases Page**](https://github.com/sus4400/DukaanPOS-releases/releases/latest).

### Step 2: Install
1. Double-click `DukaanPOS-Setup-x.x.x.exe`.
2. Follow the on-screen wizard instructions to install DukaanPOS into `C:\Program Files\DukaanPOS`.
3. Check the box to **Create a Desktop Shortcut**.

### Step 3: First Launch & Configuration
1. Open **DukaanPOS** from your Desktop shortcut.
2. Go to **Settings > General**:
   - Enter your **Store Name**, **Address**, and **Phone Number**.
   - Set your **Currency Symbol** (e.g., `Rs`, `$`, `AED`).
   - Customize your **Receipt Policy Notes** (e.g., *No Cash Refund / Exchange within 7 days*).
3. Go to **Settings > Hardware & Printing**:
   - Select your installed Thermal Printer.
   - Choose paper size (**58mm** or **80mm**).
   - Test print a sample receipt.
4. Go to **Settings > AI Assistant** (Optional):
   - Choose **Google Gemini** or **OpenRouter**.
   - Paste your API key to activate the floating support bubble!

---

## 🛡️ Data Safety & Upgrade Policy

- **Offline-First Guarantee:** All store records, transactions, ledgers, and products are stored locally in `%LocalAppData%\DukaanPos\dukaan-pos.db`.
- **Zero Data Loss on Updates:** The installer is strictly configured to **NEVER** modify or delete your database during updates or uninstallation. Updating to newer releases is 100% safe.
- **Cloud Backup:** Optional Firebase cloud synchronization can be enabled for automated offsite backups.

---

## ❓ Frequently Asked Questions (FAQ)

#### Q: Does DukaanPOS require an active internet connection?
**No.** DukaanPOS is an offline-first desktop application. Counter billing, inventory lookup, customer khata, thermal printing, and day-end reports function 100% locally with zero internet dependency.

#### Q: How do size and color variants work for clothing and boutique items?
When adding a garment product, you can enable variants to define specific sizes (e.g., S, M, L, XL), colors, and design codes. Each variant has its own unique SKU barcode and inventory count, while sharing the parent style name and price.

#### Q: Can I use my existing USB thermal printer and barcode scanner?
**Yes.** DukaanPOS is plug-and-play compatible with all standard ESC/POS 58mm (2-inch) and 80mm (3-inch) thermal receipt printers, as well as all USB and wireless 1D/2D barcode scanners.

#### Q: How does the AI Store Assistant work?
DukaanPOS features a Bring-Your-Own-Key (BYOK) AI Assistant. You can provide a free Google Gemini API key or an OpenRouter key. The assistant runs live SQL calculations directly on your local database to answer store queries (e.g., today's sales, profit, top items, debtor lists) in plain English or Roman Urdu.

#### Q: Will updating to a new version delete my products or sales data?
**No.** Your database is stored safely in `%LocalAppData%\DukaanPos\dukaan-pos.db`, completely separated from program files. Running an update installer updates the application binaries and leaves your database 100% untouched.

---

## 📞 Support & Community

- **Releases & Downloads:** [github.com/sus4400/DukaanPOS-releases](https://github.com/sus4400/DukaanPOS-releases/releases)
- **Bug Reports & Inquiries:** [Open an Issue](https://github.com/sus4400/DukaanPOS-releases/issues)

*Developed with passion for modern business owners.*
