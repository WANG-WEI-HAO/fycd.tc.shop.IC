# Google Site PWA Wrapper

🚀 This is a **Progressive Web App (PWA)** wrapper that redirects users to a Google Sites page. It allows the site to be installed on home screens like a native app, while avoiding iframe restrictions imposed by Google Sites.

## 🧩 Features

- ✅ Installable on mobile and desktop (via Chrome, Edge, Safari, etc.)
- ✅ Custom app name, icon, and splash screen
- ✅ Auto-redirect to your Google Site URL
- ✅ Deployable via GitHub Pages or any static hosting
- ⚠️ Cannot use offline caching for Google Sites content (due to browser restrictions)

## 📁 Project Structure

```
google-site-pwa/
├── index.html              # Redirects to your Google Site
├── manifest.json           # PWA configuration
├── service-worker.js       # Basic service worker registration
├── .nojekyll               # Disables Jekyll processing on GitHub Pages
└── icons/
    ├── icon-192.png
    └── icon-512.png
```

## 🔧 Setup Instructions

### 1. Replace Your Google Sites URL

Open `index.html` and update the redirect URL:

```html
<meta http-equiv="refresh" content="0; URL='https://sites.google.com/view/your-site'" />
```

Replace `your-site` with the actual path to your published Google Site.

---

### 2. Upload to GitHub

```bash
git init
git add .
git commit -m "Initial commit - Google Site PWA"
git remote add origin https://github.com/YOUR_USERNAME/google-site-pwa.git
git push -u origin main
```

---

### 3. Enable GitHub Pages

- Go to your GitHub repository
- Settings → Pages
- Select `main` branch and root (`/`)
- GitHub will provide a public URL like:  
  `https://your-username.github.io/google-site-pwa/`

---

### 4. Test PWA Installation

Open the site on Chrome or Edge. You should see an install prompt:

- 💻 Desktop: address bar → install icon
- 📱 Mobile: Chrome menu → "Add to Home screen"

---

## 📦 Credits

Built using [PWABuilder](https://www.pwabuilder.com) principles with manual customization.

---

## 📬 Questions?

If you'd like to support offline caching, add additional features, or build a more dynamic app, feel free to contact me or open an issue!
