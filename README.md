# Family Finance App

A mobile-friendly PWA for tracking family budgets, bills, and cash flow. Works offline and can be installed on both iPhone and Android home screens.

---

## Setup Instructions (one time, ~10 minutes)

### Step 1 — Create a GitHub account
Go to [github.com](https://github.com) and sign up for a free account if you don't have one.

### Step 2 — Create a new repository
1. Click the **+** icon in the top right → **New repository**
2. Name it `family-finance` (or anything you like)
3. Set it to **Public** (required for free GitHub Pages)
4. Click **Create repository**

### Step 3 — Upload the files
1. On your new repo page, click **uploading an existing file**
2. Drag and drop **all files** from this folder into the upload area:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - The `icons/` folder (both PNG files inside it)
3. Scroll down and click **Commit changes**

### Step 4 — Enable GitHub Pages
1. Go to your repo **Settings** tab
2. Click **Pages** in the left sidebar
3. Under "Source", select **Deploy from a branch**
4. Choose branch: **main**, folder: **/ (root)**
5. Click **Save**
6. Wait 1–2 minutes, then your app will be live at:
   `https://YOUR-USERNAME.github.io/family-finance`

### Step 5 — Install on your phone (iPhone)
1. Open Safari and go to your GitHub Pages URL
2. Tap the **Share** button (box with arrow)
3. Tap **Add to Home Screen**
4. Tap **Add** — done!

### Step 5 — Install on Android
1. Open Chrome and go to your GitHub Pages URL
2. Tap the **⋮** menu → **Add to Home screen**
3. Tap **Add** — done!

### Step 6 — Share with your wife
Send her the same URL (`https://YOUR-USERNAME.github.io/family-finance`).
She follows the same "Add to Home Screen" steps.

---

## How data works

Each phone stores its own data locally. When you mark a bill paid on your phone, your wife won't see it update automatically — **yet**. This is Option 1 (local storage).

For real-time sync between both phones, we can upgrade to Option 2 (Firebase) — just ask Claude to add Firebase sync to the project. It takes about 30 minutes and is free.

---

## Updating the app

When you get a new version of `index.html` from Claude:
1. Go to your GitHub repo
2. Click on `index.html`
3. Click the pencil ✏️ edit icon
4. Select all, paste the new content
5. Click **Commit changes**

The app updates automatically on both phones within a minute.

---

## Files in this package

| File | What it does |
|------|-------------|
| `index.html` | The entire app (HTML + React + your data) |
| `manifest.json` | Makes it installable as a home screen app |
| `sw.js` | Service worker — enables offline mode |
| `icons/icon-192.png` | App icon for home screen |
| `icons/icon-512.png` | App icon (larger, for splash screens) |
