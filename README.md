# Next Chapter: private retirement planner

Static browser-only retirement planner for North Carolina teachers. This public package contains **no individual salary, service record, leave balances, medical history, scenarios, or private profile**. The starting figures are a fictional demo.

## Publish on GitHub Pages

1. Create a **new repository** for this project.
2. Upload only `index.html` (and this `README.md` if desired). **Never upload your private profile or an exported scenario.**
3. Under repository Settings → Pages choose Deploy from a branch → `main` / (root), and save.
4. After publishing, open the HTTPS Pages address. Set a private passphrase (12+ characters) and use **Load private profile** with the separate `.json` file held on your own device.
5. Download an encrypted backup from Settings and keep it in Files; do not place the backup in the GitHub repository.

## Privacy design

- No third-party libraries, scripts, CSS, analytics, cookies, advertising, logins, fetch, XHR, or API calls.
- A restrictive CSP disallows outbound JavaScript network connections. Following the optional official-source hyperlinks leaves the website.
- Personal inputs and future scenarios are saved only as PBKDF2 (250,000 iterations) + AES-256-GCM encrypted data in this browser's localStorage.
- Nothing private is shipped with this package. The private profile is manually imported on-device; no uploading to a web server occurs.
- Browser storage can be cleared by Safari, and malware/extensions/device administrators may still access information displayed or typed. Use a strong device passcode and keep an encrypted backup.
- The separately supplied private-profile JSON is **not encrypted** until imported. Keep it in a safe location, then delete the plaintext copy after verifying your encrypted backup.

The app provides illustrative TSERS projections, not official benefit determinations.
