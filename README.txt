DAILY BUDGET SPLITTER - ANDROID WEBVIEW PROJECT

What is included:
- Your supplied Daily Budget Splitter HTML, bundled as an Android app asset.
- Your supplied budget.sqlite file, bundled for first launch.
- SQL.js is already embedded in the HTML.
- Google Fonts network dependency removed for offline operation.
- Android WebViewAssetLoader provides a stable HTTPS-like local origin.
- IndexedDB is used by the existing app to persist database changes between launches.

Database inspection:
- The supplied SQLite file passed PRAGMA integrity_check.
- It contains the expected tables: settings, plans, plan_items, day_logs,
  day_item_spend, day_extra_spend.
- All six tables are currently empty (zero saved plans/logged days).

Build:
1. Open this folder in Android Studio (not the ZIP itself).
2. Let Gradle sync and install the requested Android SDK 35 if prompted.
3. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
4. Android Studio will show the APK output path.

Package:
- Application ID: com.example.budgetsplitter
- App label: Daily Budget Splitter
- Minimum Android: 6.0 (API 23)

Notes:
- This is an Android Studio source project, not a compiled APK.
- The build environment used to prepare this project did not have Android SDK /
  Android Gradle build tools installed, so a signed APK could not be compiled here.
- The app stores edits in WebView IndexedDB. The bundled SQLite file is the
  first-launch starting database; edits are persisted in the app's private
  WebView storage. Use the app's Data > Download a copy function for backups.
