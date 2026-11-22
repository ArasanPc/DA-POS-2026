# DA POS

Fast, offline-ready Point of Sale & billing app (single-page, no build step).

- Works **online and offline** (service worker + local libraries)
- All data (menu, bills, settings, staff) is saved in the browser's **localStorage**
- Settings → Order Settings:
  - **Enable Discount Input %**
  - **Enable Discount Input Amount (₹ Flat)** – both can be used together

## Host on GitHub Pages
1. Create a new GitHub repository and upload **all files** in this folder (keep the `lib` folder).
2. Repo **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Choose branch `main` and folder `/ (root)` → Save.
4. Open `https://<your-username>.github.io/<repo-name>/` — open it once online, then it works offline.
5. On mobile use *Add to Home Screen* / *Install app*.

When you upload a new version, change `CACHE_VERSION` in `sw.js` (e.g. `da-pos-v2`) so devices update.
