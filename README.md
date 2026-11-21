# Penny – Money Manager

Penny is a clean, offline expense tracker and personal finance manager for Android. It lets you track daily spending, monitor cash and bank account balances, and export your transaction ledger to Excel—with zero ads, no accounts to create, and no internet connection required.

### Download APK

Grab the latest Android APK directly from GitHub Releases:

- **[Download Penny-Money-Manager.apk (latest)](https://github.com/Abaymelethil/penny-money-manager/releases/latest/download/Penny-Money-Manager.apk)**
- All versions: [Releases](https://github.com/Abaymelethil/penny-money-manager/releases)

*(Note: If you're sideloading an APK on Android, tap "Allow from this source" when prompted by your browser or file manager.)*

---

## Why Penny?

- **100% Offline & Private**: No cloud sync, no tracking, and no logins. Your financial data stays strictly on your phone.
- **Multiple Accounts & Wallets**: Manage cash, bank accounts, and credit card balances in one place.
- **Quick Expense & Income Logging**: Categorize transactions, add notes and tags, and track transfers between accounts.
- **Full Excel Export (.xlsx)**: Generate multi-sheet spreadsheets with accounts summary, transaction logs, and individual account ledgers. Shares straight through the native Android share menu (Drive, email, WhatsApp, etc.).
- **Lightweight**: Fast, responsive UI with bundled offline fonts and zero background battery drain.

---

## Building from Source

If you want to build the APK locally or customize the app:

### Prerequisites
- Node.js 20+
- JDK 21
- Android Studio

### Setup

```bash
# Clone the repository
git clone https://github.com/Abaymelethil/penny-money-manager.git
cd penny-money-manager

# Install dependencies
npm install

# Sync web assets to the Android project
npx cap sync android

# Open in Android Studio
npx cap open android
```

In Android Studio, click **Run ▶** to test on a device/emulator, or select **Build > Build Bundle(s) / APK(s) > Build APK(s)** to generate the `.apk`.

---

## Tech Stack
- Frontend: Vanilla JavaScript, HTML5, CSS
- Mobile Container: [Capacitor](https://capacitorjs.com/) (Android)
- Spreadsheet Generation: SheetJS
