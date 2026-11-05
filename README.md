# Next Chapter - iPad Home Screen icon fix

This archive is a public-safe static website. It does NOT contain personal profile data.
Do NOT upload the private retirement profile JSON to GitHub.

## GitHub Pages upload

1. Open the GitHub repository that already hosts the site.
2. Extract this ZIP first. Do not upload the ZIP file itself.
3. Upload *all the extracted files* into the same publishing directory as index.html.
   Usually this is the root of the `main` branch (if GitHub Pages is configured for main/(root)).
4. If GitHub offers to overwrite the old index.html or old icons, replace them.
5. Commit the changes, and wait for the Pages deployment to finish.
6. Open the live Pages URL in Safari. Before adding to Home Screen, visit
   `<your-site-url>/apple-touch-icon.png` to confirm the custom W icon is served.
7. If it loads, delete the old N Home Screen shortcut. Reopen the live page,
   refresh it, then Share > Add to Home Screen. Set the name to `Next Chapter`.

The icon files must be siblings of index.html, not in an additional folder.
If GitHub Pages is configured for `/docs`, put all site files in `/docs` instead.

Example for Pages using main/(root):

index.html
apple-touch-icon.png
apple-touch-icon-167x167.png
apple-touch-icon-152x152.png
icon-180.png
icon-192.png
icon-512.png
icon-32.png
manifest.webmanifest
.nojekyll
README.md

## Notes

Safari shows a single-letter monogram when it cannot use the declared Home Screen
icon. Changing the HTML alone does not upload the associated image assets.
Deleting the existing Home Screen icon and adding it again is required.

Data privacy: the public site code contains no personal starting balance or salary;
private profiles remain on the user's device after private import.
