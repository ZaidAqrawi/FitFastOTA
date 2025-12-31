# Fit Fast - Coach App

iOS app for fitness coaching and management.

## App Information

- **App Name:** Fit Fast
- **Bundle ID:** zaid.CoachApp
- **Version:** 1.0
- **Build:** 1
- **Minimum iOS Version:** 17.0
- **Team ID:** 6KFL26YA9E

## OTA (Over-The-Air) Installation Setup

This repository contains all necessary files for OTA distribution of the iOS app.

### Files Included

- `CoachApp.ipa` - The iOS application package
- `manifest.plist` - Installation manifest for OTA distribution
- `index.html` - Web page for OTA installation
- `DistributionSummary.plist` - Distribution information
- `ExportOptions.plist` - Export configuration

### Setup Instructions

1. **Deploy Files to Web Server**
   - Upload `CoachApp.ipa`, `manifest.plist`, and `index.html` to your web server
   - Ensure the server supports HTTPS (required for iOS OTA installation)

2. **Update Domain URLs**
   - Open `manifest.plist` and replace `YOUR_DOMAIN.com` with your actual domain
   - Open `index.html` and replace `YOUR_DOMAIN.com` with your actual domain

3. **Configure MIME Types**
   Ensure your web server is configured with the following MIME types:
   - `.ipa` → `application/octet-stream`
   - `.plist` → `application/x-plist` or `text/xml`

4. **Access Installation Page**
   - Users can visit your `index.html` page on their iOS device
   - Tap the "Install App" button to begin installation

### Important Notes

- The app is signed with an **Ad Hoc** provisioning profile
- Only devices registered in the provisioning profile can install the app
- Users may need to trust the developer certificate in Settings → General → VPN & Device Management
- The provisioning profile expires on: **27/12/2026**

### Distribution Method

- **Method:** Ad Hoc Distribution
- **Signing:** Automatic
- **Certificate:** Apple Distribution (expires 27/12/2026)

## Git Repository

This project is version controlled with Git. The repository includes:
- Source distribution files
- OTA installation configuration
- Documentation

---

**Team:** Osama Jassim (6KFL26YA9E)

