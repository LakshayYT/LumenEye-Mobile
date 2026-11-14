LUMEN — THE LIVING EYE (ANDROID / MOBILE BUILD)

WHAT YOU NEED
- Android phone with a recent Chrome browser
- Internet connection for the first load (MediaPipe library, WASM files and face model load from CDNs)
- Front camera permission

IMPORTANT
Camera access in browsers requires a secure page (HTTPS) and explicit permission. Opening index.html directly from a file manager may not allow the camera. Host this folder on HTTPS first.

EASIEST PC-FREE METHOD: GITHUB PAGES USING YOUR PHONE
1. Open https://github.com in Chrome and sign in (or create an account).
2. Create a new PUBLIC repository named LumenEye-Mobile.
3. Extract this ZIP using your phone's Files app. You need the files INSIDE the LumenEye-Mobile folder, not the ZIP itself.
4. In the repository, choose Add file > Upload files.
5. Upload index.html, manifest.webmanifest, sw.js, README-MOBILE.txt, and the icons folder (with both PNGs). Keep the folder structure exactly as shown.
6. Commit the uploaded files to the main branch.
7. Open repository Settings > Pages.
8. Under Build and deployment, choose Deploy from a branch; select main and /(root), then Save.
9. Wait for the Pages deployment to finish. In Settings > Pages, open Visit site.
10. Open the HTTPS site in Chrome on Android. Tap INITIALIZE CAMERA and allow camera permission.
11. In Chrome's three-dot menu, choose Add to Home screen (or Install app if offered).

CAMERA / PERFORMANCE NOTES
- Use Chrome and the front-facing camera.
- Face tracking runs locally in the browser. The page does not intentionally record or upload camera video.
- Keep the face well-lit and phone steady. Close other camera apps if camera access fails.
- The app shell can be cached, but the AI library and face model need internet on first use and may still need internet again if browser cache is cleared.
- This is a web app/PWA, not a signed APK. It can be installed from Chrome's menu after hosting on HTTPS.

TROUBLESHOOTING
- If camera is unavailable: check Chrome site settings > Camera > Allow, reload the page, and try again.
- If the model does not load: switch to a stable internet connection and reload.
- If GitHub Pages gives a 404: check that index.html is in the repository root and Pages is set to main / (root).
