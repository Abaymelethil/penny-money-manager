# Penny – Money Manager

A personal finance and expense tracking Android app built with Capacitor.

[![Download APK](https://img.shields.io/badge/Download-APK-brightgreen?logo=android&style=for-the-badge)](https://github.com/Abaymelethil/penny-money-manager/releases/latest/download/Penny-Money-Manager.apk)
[![Latest Release](https://img.shields.io/github/v/release/Abaymelethil/penny-money-manager?style=for-the-badge)](https://github.com/Abaymelethil/penny-money-manager/releases/latest)

## 📥 Download & Install

Pre-built APK is available directly via GitHub Releases:

👉 **[Download Penny-Money-Manager.apk](https://github.com/Abaymelethil/penny-money-manager/releases/latest/download/Penny-Money-Manager.apk)**

### Installation Instructions:
1. Download the `.apk` file above on your Android device.
2. Tap the file to install.
3. If prompted, allow **"Install unknown apps"** in your Android device settings.

---

## ✨ Features

- **Offline-First**: 100% offline and private. Bundled local fonts and assets.
- **Account Management**: Track bank accounts, cash, credit limits, and balances.
- **Transaction History**: Income, expense, and transfer tracking with tags and categories.
- **Export to Excel**: Generates full multi-sheet `.xlsx` workbooks (Accounts, Transactions, and individual Account Ledgers) with native Android share sheet integration.
- **Native Android Support**: Built-in Android back navigation, splash screens, and responsive UI.

---

## 🛠️ Development & Building

### Requirements
- Node.js 20+
- JDK 21
- Android Studio

### Quick Start
```bash
# Install dependencies
npm install

# Sync web assets into the Android native project
npx cap sync android

# Open in Android Studio
npx cap open android
```

In Android Studio:
- Click **Run ▶** to deploy to a connected device or emulator.
- Or select **Build > Build Bundle(s) / APK(s) > Build APK(s)** to generate an installable APK.
