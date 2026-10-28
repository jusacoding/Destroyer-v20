# Matches Deriv

A static GitHub Pages dashboard that subscribes to public Deriv tick data and displays the frequency of the final digit in recent quotes.

## Files
- `index.html` — dashboard structure
- `style.css` — responsive sky-blue / purple styling
- `app.js` — public WebSocket tick connection and frequency calculations

## Publish on GitHub using an Android phone
1. Download and extract `matches-deriv-github.zip` on your phone.
2. Open your repository: `Jusa2.0matcheskillerbot`.
3. Go to the **Code** tab (not Settings).
4. Tap **Add file** → **Upload files**. If you do not see it, first return to the Code tab and look for the `+` menu or `Add file` menu.
5. Upload `index.html`, `style.css`, and `app.js` from the extracted folder. You can also upload this README.
6. Commit the changes to the repository's default branch.
7. Open **Settings** → **Pages**. Under Build and deployment, choose **Deploy from a branch**, select the default branch and `/ (root)`, then save.
8. Wait for GitHub Pages to publish, then open the URL shown in Settings → Pages.

## Notes
- This dashboard uses public tick data and does not ask for or store a Deriv account token.
- `APP_ID` in `app.js` is a public application ID used for the public data connection, not a user's personal API token.
- If the WebSocket connection closes, check the browser console or try again later; network restrictions or API changes can affect connections.
- Frequencies describe the sample that has already appeared. They do not guarantee the next digit and this page does not place trades.
