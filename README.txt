StudyHub PWA package

Files:
- index.html: your uploaded StudyHub website, configured as the app entry page
- manifest.json: installable app metadata
- service-worker.js: basic same-origin app-shell caching
- icons/: app icons

Publish the CONTENTS of this folder (not the ZIP itself) to the root of a GitHub repository. Keep index.html, manifest.json, service-worker.js, and icons/ at the repository root. Then enable GitHub Pages from Settings > Pages > Deploy from a branch > main > /(root).

Important: this front-end currently stores demo account details in browser localStorage. Do not use real passwords or private student data until a secure backend authentication system is added. Some external assets such as Google Fonts need internet access.
