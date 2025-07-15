# Sunside QR Code Redirect

A simple, lightweight QR code redirect page that automatically sends users to the appropriate app store based on their device.

## Features

- **Auto-detection**: Automatically detects iOS and Android devices
- **Smart redirect**: Redirects iOS users to App Store, Android users to Google Play
- **Fallback interface**: Shows manual selection for desktop/unknown devices
- **Fast loading**: Optimized for quick QR code scanning experience
- **Mobile-first**: Designed specifically for mobile users scanning QR codes

## Setup

### 1. Update App Store URLs

Edit `index.html` and replace the placeholder URLs with your actual app store links:

```javascript
const APP_STORE_URL = 'https://apps.apple.com/app/your-app-id'; // Replace with your iOS app URL
const PLAY_STORE_URL = 'https://play.google.com/store/apps/details?id=your.package.name'; // Replace with your Android app URL
```

### 2. Deploy to qr.sunside.club

This project is designed to be hosted on the `qr.sunside.club` subdomain.

### 3. Generate QR Code

Once deployed, generate a QR code pointing to `https://qr.sunside.club`

## How it Works

1. User scans QR code with their mobile device
2. Page loads and detects device type using user agent
3. iOS users are automatically redirected to App Store
4. Android users are automatically redirected to Google Play
5. Desktop/unknown devices see a fallback page with manual selection
6. If auto-redirect fails, fallback interface is shown after 2 seconds

## File Structure

```
sunside_qrcode/
├── index.html          # Main redirect page
└── README.md          # This file
```

## Testing

Test on different devices:
- iPhone/iPad: Should auto-redirect to App Store
- Android phone/tablet: Should auto-redirect to Google Play
- Desktop: Should show manual selection interface

## Customization

You can customize the appearance by modifying the CSS in `index.html`:
- Change colors in the gradient background
- Update the logo (currently shows "S")
- Modify button styles and text
- Adjust animations and timing
