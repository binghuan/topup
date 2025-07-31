# Orange Top-Up PWA

A Progressive Web App (PWA) that provides a convenient way to add the Orange Top-Up service to your iOS device's home screen as a native-like app shortcut.

## Features

- **Easy Installation**: Simple one-tap installation to iOS home screen
- **Native App Experience**: Behaves like a native app when launched from home screen
- **Multiple Icon Sizes**: Comprehensive icon set for different device resolutions
- **Automatic Redirection**: Seamlessly redirects to Orange Top-Up service
- **Mobile Optimized**: Designed specifically for mobile devices

## How It Works

This PWA works in two modes:

1. **Installation Mode**: When accessed via the pin-to-start link, it displays installation instructions
2. **Launch Mode**: When launched from the home screen icon, it automatically redirects to the Orange Top-Up service

## Installation

### Method 1: QR Code
Scan the QR code below with your iOS device:

<img src="pictures/QRCode.png" alt="QR Code for installation">

### Method 2: Direct Link
Visit the installation page: [http://binghuan.github.io/topup/pin2start.html](http://binghuan.github.io/topup/pin2start.html)

### Installation Steps
1. Open the link in Safari on your iOS device
2. Tap the Share button <img src="images/ic_share.png" alt="Share icon" style="display: inline; height: 16px;">
3. Select "Add to Home Screen" <img src="images/ic_add2home.png" alt="Add to home screen icon" style="display: inline; height: 16px;">
4. Customize the name if desired and tap "Add"

## Technical Details

### Files Structure
- `index.html` - Main PWA interface with installation instructions
- `pin2start.html` - Entry point that sets installation state
- `main.js` - JavaScript logic for state management and redirection
- `icons/` - Complete icon set for various device resolutions (16px to 1024px)
- `images/` - UI instruction images (share and add-to-home icons)

### Key Features
- **Session Storage**: Uses `sessionStorage.PIN_TILE_STAY` to track installation state
- **Responsive Icons**: Supports multiple icon sizes from 16x16 to 1024x1024 pixels
- **Apple-Specific Meta Tags**: Optimized for iOS Safari with proper web app capabilities
- **Automatic Redirection**: Redirects to `https://topup.orange.com/en/` after installation

### Browser Compatibility
- Optimized for iOS Safari
- Supports Apple Touch Icons
- Mobile viewport optimized
- PWA-ready with proper meta tags

## Development

The app uses vanilla HTML, CSS, and JavaScript with no external dependencies. It's hosted on GitHub Pages and can be easily modified or deployed to other static hosting services.