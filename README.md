# LinkPlay — Android starter

This is a starter project, not a finished TeraBox resolver. It contains:
- Flutter Android app UI
- Paste-from-clipboard
- TeraBox share-link validation
- Video player for an authorized stream URL
- Node.js backend endpoint scaffold

## Requirements
- Flutter SDK
- Android Studio / Android SDK
- Node.js 18+

## Run the Flutter app
1. Install Flutter and Android Studio.
2. In this folder run:
   ```bash
   flutter create .
   flutter pub get
   flutter run
   ```
3. Deploy the backend over HTTPS.
4. In `lib/main.dart`, replace `https://YOUR-BACKEND-DOMAIN` with your backend URL.

## Run the backend locally
```bash
cd backend
npm install
npm start
```
The backend listens on port 3000.

## Important: TeraBox integration
A TeraBox sharing URL is not automatically a direct video stream URL. The `/resolve` endpoint intentionally returns HTTP 501 until an official, authorized TeraBox API integration is configured. Obtain the appropriate API access and confirm its terms before implementing this part. Do not put API secrets in the Flutter app. Do not bypass passwords, DRM, or access restrictions.

## Current status
The UI and player scaffold are provided. Real TeraBox link resolution, API credentials, production hosting, testing, and Play Store publishing remain to be completed.
