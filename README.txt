MASALA COUNTER — PHONE-ONLY SETUP

WHAT IS INCLUDED
- index.html: the calculator app
- manifest.webmanifest: Android install/app details
- sw.js: offline caching
- icon-192.png and icon-512.png: app icons

IMPORTANT
A PWA must be served from HTTPS to install as an app and use its service worker.
Opening index.html directly from Downloads will let you test the calculator, but it will not install as a PWA or work offline as an installed app.

FREE PHONE-ONLY HOSTING WITH GITHUB PAGES
1. On your phone, open https://github.com and create a free account or sign in.
2. Create a new repository named masala-counter. Set it to Public. Do not add a README, license, or .gitignore.
3. Download and extract masala-counter-pwa.zip on your phone.
4. Open the new repository on GitHub in Chrome. Choose Add file > Upload files.
5. Upload the CONTENTS of the extracted folder, not the ZIP itself. Select and upload these six files together: index.html, manifest.webmanifest, sw.js, README.txt, icon-192.png and icon-512.png. All six must be at the repository's top level.
6. Commit the upload.
7. In the repository, open Settings > Pages.
8. Under Build and deployment, choose Deploy from a branch. Select branch main and folder /(root), then Save.
9. Wait a minute or two. GitHub Pages will show your website address, usually https://YOUR-USERNAME.github.io/masala-counter/
10. Open that address in Chrome on Android. Wait for the page to finish loading. Use Chrome menu (three dots) > Install app or Add to Home screen. Confirm.
11. Open Masala Counter from your home screen once while online. Then test Airplane mode. The app should still open and calculate offline.

IF UPDATES ARE NEEDED
After uploading changed files, reopen the app online. If an older version remains, close the app fully and reopen it. The service worker cache name can be changed in sw.js (CACHE='masala-counter-v2') to force a fresh cache on the next visit.

PRIVACY
Entries are saved in local storage on this device only. They are not sent to a server. Clearing Chrome site data can erase saved entries. The app is a calculator, not a payment terminal or accounting system.

CALCULATION
Each item price = weight in grams × price per kg ÷ 1000.
The total is the sum of item prices. Change is payment minus total.
