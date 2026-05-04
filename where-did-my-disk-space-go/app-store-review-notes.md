# App Store Review Notes

App name: Where Did My Disk Space Go?

Website URL: https://offyotto-sl3.github.io/where-did-my-disk-space-go/

Privacy Policy URL: https://offyotto-sl3.github.io/where-did-my-disk-space-go/privacy.html

Support URL: https://offyotto-sl3.github.io/where-did-my-disk-space-go/support.html

## Review Summary

Where Did My Disk Space Go? is a macOS utility that scans permitted local folders to show disk usage, large files, old downloads, developer caches, package caches, build artifacts, and duplicates.

The app processes scan results locally on the user's Mac. It does not use accounts, analytics SDKs, advertising SDKs, tracking SDKs, or network connections.

Cleanup uses `FileManager.trashItem`, moving selected items to Trash. The app does not permanently erase files as part of its normal cleanup workflow.

## Privacy And Permissions

- App Sandbox is enabled for Mac App Store distribution.
- Network access entitlements are disabled.
- The app includes `PrivacyInfo.xcprivacy`.
- Required-reason API declarations:
  - `NSPrivacyAccessedAPICategoryDiskSpace` with reason `E174.1`
  - `NSPrivacyAccessedAPICategoryFileTimestamp` with reason `DDA9.1`
- App Store Connect privacy answer should be "Data Not Collected" if the submitted binary remains as currently implemented.
- The app includes clear folder usage descriptions for Desktop, Documents, and Downloads.

## Suggested App Review Note

This macOS app scans local folders that the user has allowed the app to access so it can display local disk usage and cleanup suggestions. File names, file paths, file sizes, timestamps, duplicate results, and disk-space information remain on device and are not transmitted to the developer or third parties. The app does not use analytics, ads, tracking SDKs, accounts, or network connections. Cleanup moves selected items to Trash so the user can recover them before emptying Trash.
