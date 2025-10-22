# 🚀 Installation Guide

This document provides instructions for installing and setting up the **Deenseek** application, whether for immediate use or for local development.

-----

## 1\. Quick Start

### Browser Usage (Easiest)

This method requires no local setup or command line tools.

1.  **Download** the project files (e.g., as a ZIP archive).
2.  **Unzip** the archive.
3.  **Open** the file `index.html` in your web browser.
4.  **Start using** the application immediately.

### Live Demo

You can visit the live, publicly hosted version of the application here:
[https://umarbutteditz.github.io/Deenseek](https://umarbutteditz.github.io/Deenseek)

-----

## 2\. Local Development Setup

### Prerequisites

  * Modern web browser (**Chrome, Firefox, Safari, Edge**).
  * Basic understanding of web technologies (HTML, JavaScript) is recommended for development.
  * **Git** installed on your system.

### Step-by-Step Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/umarbutteditz/Deenseek.git
    ```

2.  **Navigate to project directory:**

    ```bash
    cd Deenseek
    ```

3.  **Open in browser (multiple methods):**

      * **Method A: Double-click** `index.html` (simplest, but may have limitations with certain browser security policies, like local file access).
      * **Method B: Use Python simple server** (Recommended for local testing):
        ```bash
        python -m http.server 8000
        # Then visit http://localhost:8000 in your browser
        ```
      * **Method C: Use Node.js http-server** (Requires Node.js/npm):
        ```bash
        npx http-server
        # Then visit the provided local address (e.g., http://127.0.0.1:8080)
        ```

### File Structure Overview

```
Deenseek/
├── index.html              # Main application entry point
├── meeqat_2025.json        # Prayer times database
├── desi_calendar_2025.json # Desi calendar data
├── jekyll-gh-pages.yml     # GitHub Pages configuration file
├── static.yml              # Static deployment configuration
└── README.md               # Project documentation
```

-----

## 3\. PWA (Progressive Web App) Installation

The application can be installed on your device to run like a native app.

### Mobile Devices

| Platform | Instructions |
| :--- | :--- |
| **Android (Chrome)** | 1. Open the app in the Chrome browser. <br> 2. Tap the menu (three dots) → **"Add to Home screen"**. <br> 3. Confirm the installation and launch from the home screen. |
| **iOS (Safari)** | 1. Open the app in Safari. <br> 2. Tap the share button (square with arrow). <br> 3. Scroll down and tap **"Add to Home Screen"**. <br> 4. Confirm and launch from the home screen. |

### Desktop PWA

1.  Open the application in Chrome or Edge.
2.  Look for the install prompt icon in the address bar.
3.  Click **"Install"** or use the browser menu.
4.  The app will open in a dedicated, frameless window.

-----

## 4\. Deployment Options

### GitHub Pages (Automatic)

  * The repository is already configured for **GitHub Pages**.
  * Deployment occurs **automatically** on every push to the `main` branch.
  * The application is accessible via: `https://username.github.io/Deenseek`

### Manual Web Hosting

1.  Upload all files from the project root to your web server.
2.  Ensure proper **MIME types** are configured for JSON files.
3.  Configure **HTTPS** (SSL/TLS) for geolocation features to work securely.
4.  Test all functionality thoroughly after upload.

### Local Network Deployment

For sharing within a local network (LAN) for testing:

| Tool | Command |
| :--- | :--- |
| **Python** | `python -m http.server 8080` |
| **Node.js** | `npx serve .` |
| **PHP** | `php -S localhost:8000` |

-----

## 5\. Configuration & Permissions

### Location Settings

  * **Automatic**: Uses device GPS (requires user permission).
  * **Manual**: Allows the user to set custom coordinates.
  * **Default**: Bunjwah, Kishtwar (**33.3167, 75.7667**) is used as a fallback.

### Application Permissions Required

| Permission | Purpose |
| :--- | :--- |
| **Location** | For accurate **Qibla** direction. |
| **Orientation** | For **compass** functionality. |
| **Storage** | For caching and user preferences. |
| **Audio** | For **Quran recitation** features. |

-----

## 6\. Troubleshooting

### Common Issues and Solutions

| Issue | Solution Steps |
| :--- | :--- |
| **Qibla Compass Not Working** | 1. Ensure location permissions are granted. <br> 2. Check if the device has a compass/magnetometer sensor. <br> 3. **Calibrate** the device by moving it in a figure-8 pattern. <br> 4. Try in a different location (avoid magnetic interference). |
| **Prayer Times Not Loading** | 1. Check internet connection for initial data load. <br> 2. Verify the JSON data files are accessible. <br> 3. Clear browser cache and reload the page. <br> 4. Check the browser console for errors. |
| **Audio Not Playing** | 1. Ensure device and browser volume is not muted. <br> 2. Check browser audio permissions. <br> 3. Try a different audio source or quality setting. <br> 4. Verify internet connection for audio streaming. |
| **Location Detection Failed** | 1. Enable location services on the device. <br> 2. Grant the browser location permission when prompted. <br> 3. Try in an area with a better GPS signal. <br> 4. Use manual location as a fallback. |

### Browser Compatibility

| Browser | Qibla Compass | Geolocation | Audio | PWA |
| :--- | :--- | :--- | :--- | :--- |
| **Chrome** | ✅ | ✅ | ✅ | ✅ |
| **Firefox** | ✅ | ✅ | ✅ | ✅ |
| **Safari** | ✅ | ✅ | ✅ | ✅ |
| **Edge** | ✅ | ✅ | ✅ | ✅ |

### Mobile Specific Performance Tips

  * Close other background apps for better compass accuracy.
  * Use the app in **landscape mode** for optimal compass view.
  * Keep the device flat and steady during Qibla calibration.
  * Allow all requested permissions for full functionality.

-----

## 7\. Development & Support

### For Contributors

1.  **Fork and clone** the repository:
    ```bash
    git clone https://github.com/your-username/Deenseek.git
    ```
2.  **Create a feature branch:**
    ```bash
    git checkout -b feature/your-feature
    ```
3.  **Make changes and test locally** (by opening `index.html` in your browser).
4.  **Commit and push** your changes:
    ```bash
    git add .
    git commit -m "Add your feature"
    git push origin feature/your-feature
    ```
5.  **Create a pull request** on the main repository.

### Testing Guidelines

  * Test on multiple devices and browsers.
  * Verify all prayer calculations are accurate.
  * Check compass accuracy in different physical locations.
  * Test offline (caching) functionality.
  * Validate the responsive design across screen sizes.

### Support

**Getting Help:**

  * Check this documentation first.
  * Review the browser console for specific JavaScript errors.
  * Test with different browsers to isolate the issue.
  * Verify file permissions if deploying on a server.

**Reporting Issues:**

1.  Describe the problem clearly and concisely.
2.  Include your device and browser information.
3.  Note any specific error messages shown in the console.
4.  Provide clear, numbered steps to reproduce the bug.

**Feature Requests:**

  * Suggest new features through **GitHub issues** with detailed descriptions of the desired functionality and user benefit.