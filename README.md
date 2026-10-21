# Shine AI — mobile-first PWA demo

This is a responsive, installable Progressive Web App prototype. It includes a chat UI, prompt suggestions, browser speech input where supported, local chat history, local demo account UI, and a local admin demo screen.

## Important limitations
- Chat replies are scripted demo responses. No live AI model or API is connected.
- Account/admin controls are local-only and **not secure authentication**.
- Data is stored in the browser on this device. No server/database is configured.
- Voice input depends on browser support and permissions.
- The project is a PWA/site, not a compiled Android APK.

## Publish using GitHub Pages
1. Upload the extracted project contents to the repository root (including `.github/workflows/deploy-pages.yml`).
2. In repository Settings → Pages, set Source to **GitHub Actions** if asked.
3. Open Actions and run **Deploy Shine AI demo** or push a commit that changes one of the tracked files.
4. After success, the workflow summary shows the site URL. Usually it is `https://OWNER.github.io/REPOSITORY/`.
5. Open the URL in Chrome on Android → menu ⋮ → **Install app** or **Add to Home screen**.

## To turn this into a real AI product
A secure backend is needed to call an AI provider. Never place a private API key in `index.html` or commit it to a public repository. Add server-side authentication, database/storage, rate limits, privacy policy, and secure admin authorization before real use.
