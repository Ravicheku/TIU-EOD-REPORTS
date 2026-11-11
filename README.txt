TIU DC PWA — INSTALLABLE WEB APP

Files:
- index.html: your TIU DC EOD app
- manifest.webmanifest: app name, icon and standalone display settings
- sw.js: offline app shell cache
- icons/: home-screen icons

IMPORTANT:
A Progressive Web App can be installed from Chrome only when served from HTTPS (or localhost). A file:// HTML file opened from Downloads cannot register a service worker and cannot be installed as a PWA.

Easy hosting option — GitHub Pages:
1. Sign in to GitHub and create a new PUBLIC repository, e.g. tiu-dc-eod.
2. Upload all files and folders from this package (index.html, manifest.webmanifest, sw.js, icons folder) into the repository root.
3. In repository Settings > Pages, choose Deploy from a branch; select main and /(root), then Save.
4. Wait for GitHub Pages to publish the HTTPS website.
5. On Android, open the published https://...github.io/... link in Chrome.
6. Open Chrome menu (⋮) > Install app or Add to Home screen > Install/Add.
7. Open TIU DC from the phone home screen once while online. The service worker caches the app shell; after that it can reopen offline.

Five phones:
Repeat the install on each phone. Each phone keeps its own local browser storage. No cross-phone sync is included.

Data:
Reports remain in local browser storage on each device. Clearing Chrome site data or removing the installed app/site data may erase records. Export backups regularly from Settings.
