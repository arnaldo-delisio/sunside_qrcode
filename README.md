# Sunside QR Code Redirect

A simple, lightweight QR code redirect page that automatically sends users to the appropriate app store based on their device for **Sunside Club**.

## 🚀 Live Demo

- **Repository**: https://github.com/arnaldo-delisio/sunside_qrcode
- **Deployment**: Ready for Vercel deployment at `qr.sunside.club`

## ✨ Features

- **Auto-detection**: Automatically detects iOS and Android devices
- **Smart redirect**: Redirects iOS users to App Store, Android users to Google Play
- **Fallback interface**: Shows official app store badges for desktop/unknown devices
- **Fast loading**: Optimized for quick QR code scanning experience
- **Mobile-first**: Designed specifically for mobile users scanning QR codes
- **Italian localization**: All text in Italian for the target audience

## 🏪 App Store Links

- **iOS**: https://apps.apple.com/it/app/sunside-club/id6746264199
- **Android**: https://play.google.com/store/apps/details?id=com.sunside.app

## 🎯 How it Works

1. User scans QR code with their mobile device
2. Page loads and detects device type using user agent
3. **iOS users** are automatically redirected to App Store
4. **Android users** are automatically redirected to Google Play
5. **Desktop/unknown devices** see official app store badges for manual selection
6. If auto-redirect fails, fallback interface is shown after 2 seconds

## 📁 Project Structure

```
sunside_qrcode/
├── index.html          # Main redirect page with auto-detection
├── README.md           # This file
└── .git/              # Git repository
```

## 🚀 Deployment

### Vercel (Recommended)
1. Connect this GitHub repository to Vercel
2. Set up custom domain: `qr.sunside.club`
3. Deploy automatically on every push to main branch

### Manual Deployment
Simply upload `index.html` to any web server or hosting service.

## 🧪 Testing

Test the redirect functionality on different devices:
- **iPhone/iPad**: Should auto-redirect to App Store
- **Android phone/tablet**: Should auto-redirect to Google Play
- **Desktop**: Should show official app store badges

## 📱 QR Code Generation

After deployment, generate a QR code pointing to `https://qr.sunside.club` using:
- QRCode Monkey (qrcode-monkey.com) - recommended for customization
- QR Code Generator (qr-code-generator.com)
- Any other QR code generator service

### QR Code Best Practices:
- Use high resolution (300x300px minimum)
- Add Sunside Club logo in center
- Test on multiple devices before printing
- Use medium/high error correction level

## 🎨 Customization

The page uses a purple gradient background matching the Sunside Club brand. You can customize:
- Colors in the CSS gradient
- Logo (currently shows "S")
- App store badge styling
- Text and messaging

## 🔧 Development

```bash
# Clone the repository
git clone https://github.com/arnaldo-delisio/sunside_qrcode.git

# Make changes to index.html
# Commit and push to deploy automatically via Vercel
git add .
git commit -m "Your changes"
git push origin main
```

## 📊 Analytics

Once deployed on Vercel, you can enable:
- Vercel Analytics for traffic insights
- Custom tracking for QR code campaign effectiveness
- Geographic distribution of scans

## 🌐 Supported Languages

- **Italian**: Primary language for the target market
- Easy to extend for other languages by modifying text strings

---

**Built for Sunside Club** - Connecting users to the right app store, one scan at a time! 🌅