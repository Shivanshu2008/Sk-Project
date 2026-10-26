SkStudyhub icons package
========================

Upload these files into the SAME ROOT FOLDER as index.html in your GitHub repository.
For this project, the root is the folder where index.html currently lives.

Included:
- icon-192.png             Android / PWA icon
- icon-512.png             Android / PWA icon
- icon-maskable-512.png    Maskable PWA icon
- apple-touch-icon.png     iPhone / iPad home-screen icon (180x180)
- favicon-32.png           Browser tab icon
- favicon-16.png           Small browser tab icon
- favicon.ico              Browser favicon
- manifest.webmanifest     PWA manifest

IMPORTANT:
1. This package assumes index.html is in the repository root.
2. Existing image files are not deleted or replaced by this package except if you choose to overwrite same-named icon files.
3. If index.html already links to manifest.json instead of manifest.webmanifest, update the HTML link to the manifest file you choose to use. Avoid keeping two conflicting manifests.

Add/confirm these lines inside <head> in index.html:

<link rel="icon" href="./favicon.ico" sizes="any">
<link rel="icon" type="image/png" sizes="32x32" href="./favicon-32.png">
<link rel="apple-touch-icon" href="./apple-touch-icon.png">
<link rel="manifest" href="./manifest.webmanifest">
<meta name="theme-color" content="#003b3b">

Use relative paths beginning with ./ because the GitHub Pages site is hosted under /Sk-Project/.
Do not use paths like /icon-192.png; those may point to the domain root instead of this project.

After uploading:
- Commit changes to GitHub.
- Wait for GitHub Pages deployment to finish.
- Test the live site and install prompt on Android/Windows.
- On iPhone/iPad, open the site in Safari and use Share > Add to Home Screen.
- A PWA does not automatically become a signed native APK/IPA/MSIX package. Store publishing and native packaging may need separate steps.
