# Penny – Money Manager (Capacitor / Android)

Your `indexv11.html` packaged as a Capacitor Android project, with a new **Export to Excel** option.

## Build the app

Requirements: Node.js 22+, JDK 21, Android Studio (latest stable).

```bash
npm install            # installs Capacitor + plugins
npx cap sync android   # copies www/ into the Android project
npx cap open android   # opens Android Studio
```

In Android Studio: wait for the Gradle sync to finish, then
* **Run ▶** to install on a phone/emulator, or
* **Build > Build Bundle(s) / APK(s) > Build APK(s)** for an installable `.apk`.

The `android/` folder is already generated, so you do NOT need `npx cap add android`.

## Whenever you edit the app

Edit `www/index.html`, then run `npx cap sync android` and press Run again.

## Export to Excel

Open **More > Export to Excel** (also at the bottom of the **Accounts** screen).
The workbook contains:
* **Accounts** – each account's type, opening balance / credit limit, total in, total out, current balance, plus the totals shown in the app
* **Transactions** – every transaction (date & time, type, category, account, to-account, amount, note, tags)
* **One sheet per account** – a ledger with money in, money out and a running balance

On the phone, the Android share sheet opens so you can save the .xlsx to Drive / Files, or send it by email / WhatsApp.
(Receipt photos are not included in the export.)

## Changing the package name / app name

`capacitor.config.json` holds `appId` (`com.penny.moneymanager`) and `appName`.
If you change `appId` before your first build, also run: `npx cap sync android` and update `namespace`/`applicationId` in `android/app/build.gradle`
(or simply delete `android/` and run `npx cap add android`, then re-add the launcher icons).

## Notes
* Everything works offline: the fonts and the Excel library are bundled in `www/`.
* Data is stored in the app's WebView storage on the phone. Uninstalling the app or clearing its data erases it, so export to Excel or use **Backup** now and then.
* The Android back button now closes sheets / goes back a screen, and exits from Home.
