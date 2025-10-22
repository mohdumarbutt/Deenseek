# 🚀 Installation Guide

## Quick Start

### Browser Usage (Easiest)
1. **Download** the project files
2. **Open** `index.html` in your web browser
3. **Start using** the application immediately

### Live Demo
Visit the live application at:  
[https://umarbutteditz.github.io/Deenseek](https://umarbutteditz.github.io/Deenseek)

## Local Development Setup

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Basic understanding of web technologies (for development)

### Step-by-Step Installation


# 1. Clone the repository
git clone https://github.com/umarbutteditz/Deenseek.git

# 2. Navigate to project directory
cd Deenseek

# 3. Open in browser (multiple methods)

# Method A: Double-click index.html
# Method B: Use Python simple server
python -m http.server 8000
# Then visit http://localhost:8000

# Method C: Use Node.js http-server
npx http-server
# Then visit the provided local address

### File Structure Overview

``` bash
Deenseek/
├── index.html              # Main application
├── meeqat_2025.json        # Prayer times database
├── desi_calendar_2025.json # Desi calendar data
├── jekyll-gh-pages.yml     # GitHub Pages config
├── static.yml             # Static deployment config
└── README.md              # Documentation
```

## PWA Installation

### Mobile Devices

#### Android (Chrome)
1. Open the app in Chrome browser
2. Tap the menu (three dots) → "Add to Home screen"
3. Confirm the installation
4. Launch from home screen like a native app

#### iOS (Safari)
1. Open the app in Safari
2. Tap the share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Confirm and launch from home screen

### Desktop PWA
1. Open in Chrome/Edge
2. Look for install prompt in address bar
3. Click "Install" or use browser menu
4. App will open in dedicated window

## Deployment Options

### GitHub Pages (Automatic)
- Repository is configured for GitHub Pages
- Automatic deployment on push to main branch
- Access via: `https://username.github.io/Deenseek`

### Manual Web Hosting
1. Upload all files to web server
2. Ensure proper MIME types for JSON files
3. Configure HTTPS for geolocation features
4. Test all functionality

### Local Network Deployment

# Using Python
python -m http.server 8080

# Using Node.js
npx serve .

# Using PHP
php -S localhost:8000


## Configuration

### Location Settings
- **Automatic**: Uses device GPS (requires permission)
- **Manual**: Set custom coordinates
- **Default**: Bunjwah, Kishtwar (33.3167, 75.7667)

### Prayer Calculation
- Based on provided prayer time data
- Automatic timezone detection
- Local time conversion
- Seasonal adjustments

### Permissions Required
- **Location**: For accurate Qibla direction
- **Orientation**: For compass functionality
- **Storage**: For caching and preferences
- **Audio**: For Quran recitation

## Troubleshooting

### Common Issues

#### Qibla Compass Not Working
- Ensure location permissions are granted
- Check device has compass/magnetometer
- Calibrate device by moving in figure-8 pattern
- Try in different location (avoid magnetic interference)

#### Prayer Times Not Loading
- Check internet connection for initial load
- Verify JSON files are accessible
- Clear browser cache and reload
- Check browser console for errors

#### Audio Not Playing
- Ensure volume is not muted
- Check browser audio permissions
- Try different audio source
- Verify internet connection for audio streaming

#### Location Detection Failed
- Enable location services on device
- Grant browser location permission
- Try in area with better GPS signal
- Use manual location as fallback

### Browser Compatibility

| Browser | Qibla Compass | Geolocation | Audio | PWA |
|---------|---------------|-------------|--------|-----|
| Chrome | ✅ | ✅ | ✅ | ✅ |
| Firefox | ✅ | ✅ | ✅ | ✅ |
| Safari | ✅ | ✅ | ✅ | ✅ |
| Edge | ✅ | ✅ | ✅ | ✅ |

### Mobile Specific

#### Performance Tips
- Close other apps for better compass accuracy
- Use in landscape mode for better compass view
- Keep device flat and steady for calibration
- Allow all requested permissions

#### Battery Optimization
- App is lightweight and battery-friendly
- No background processes when closed
- Efficient sensor usage
- Minimal data consumption

## Development Setup

### For Contributors

# Fork and clone
git clone https://github.com/your-username/Deenseek.git

# Create feature branch
git checkout -b feature/your-feature

# Make changes and test locally
# Open index.html in browser

# Commit and push
git add .
git commit -m "Add your feature"
git push origin feature/your-feature

# Create pull request

### Testing
- Test on multiple devices and browsers
- Verify all prayer calculations
- Check compass accuracy in different locations
- Test offline functionality
- Validate responsive design

## Support

### Getting Help
- Check this documentation first
- Review browser console for errors
- Test with different browsers
- Verify file permissions on server

### Reporting Issues
1. Describe the problem clearly
2. Include device and browser information
3. Note any error messages
4. Provide steps to reproduce

### Feature Requests
Suggest new features through GitHub issues with detailed descriptions of desired functionality.