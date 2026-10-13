SETTINGS DEMO — iOS-inspired PWA
================================

This is an independent visual demo inspired by iOS Settings. It is not an Apple product and does not change the iPhone's actual battery, status bar, Wi-Fi, Bluetooth, privacy settings, or Apple's real Screen Time records. Battery and Screen Time values are fictional, editable demo data saved locally in the browser.

FILES
-----
index.html              App markup
style.css               Responsive iOS-inspired styling and dark mode
app.js                  Navigation, settings, demo data, local persistence
manifest.webmanifest    Installable web app metadata
sw.js                   Service worker for offline caching
icons/icon-192.png      App icon
icons/icon-512.png      Large app icon

INSTALL ON IPHONE WITHOUT A MAC
--------------------------------
The easiest path is to host the files on an HTTPS website. GitHub Pages is a free option.

1. Create or sign in to a GitHub account.
2. Create a new repository, for example: settings-demo. For the simplest setup, make it public.
3. Upload the project files and the icons folder to the repository root. Keep the file names and folder structure unchanged.
4. Open the repository's Settings → Pages.
5. Under “Build and deployment”, choose “Deploy from a branch”. Select the main branch and “/(root)”, then Save.
6. Wait for GitHub Pages to publish. GitHub will show a website address similar to https://YOUR-USERNAME.github.io/settings-demo/.
7. On the iPhone, open that HTTPS address in Safari.
8. Tap Share (the square with the upward arrow) → Add to Home Screen → Add. If available, enable “Open as Web App”.
9. Launch Settings Demo from the new Home Screen icon. Open it online once first so the offline cache can be installed.

NOTES
-----
- The service worker and PWA installation require HTTPS (or localhost for local development). Opening index.html directly from the Files app is not the full installation method.
- Local demo changes are saved in that browser's local storage on that device. Clearing website data may erase them.
- Safari/iOS may apply platform-specific restrictions to web apps. This project cannot replace Apple's Settings app or change native system data.
- The app is a starting version; some secondary settings are visual placeholders.
