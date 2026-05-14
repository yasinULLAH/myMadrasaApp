# 🔐 GitHub Deployment — Remaining Manual Steps
## مدرسہ مینجمنٹ سسٹم — گٹ ہب پر محفوظ طریقے سے اپلوڈ کرنے کی ہدایات

---

## ✅ Already Done For You (By AI Assistant)

These steps have been **completed automatically** — no action needed:

| # | Task | Status |
|---|---|---|
| 1 | ✅ Created `.gitignore` — blocks `client_secret_*.json`, `.env`, `.zip`, `.pyw` files | Done |
| 2 | ✅ Set your `CLIENT_ID` in `index.html` (line ~5461) | Done |
| 3 | ✅ Moved `client_secret_*.json` to safe location: `C:\Users\Yasin\Documents\google_oauth_secrets\` | Done |
| 4 | ✅ Scanned code — zero secrets found in `index.html` | Done |
| 5 | ✅ Initialized Git repo, committed `.gitignore` first, then all project files | Done |
| 6 | ✅ Renamed branch to `main` | Done |

> **Note:** Your Client ID (`323091985122-...`) is embedded in `index.html`. **This is safe** — in OAuth implicit flow (browser-only apps), the Client ID is designed to be public. Google verifies requests by matching the origin URL, not by the Client ID alone.

---

## 📋 What YOU Need To Do (4 Steps)

### Step 1: Create a GitHub Repository

1. Go to [github.com/new](https://github.com/new)
2. Fill in:
   - **Repository name:** `madrasa-management-system` (or any name you prefer)
   - **Description:** `مدرسہ مینجمنٹ سسٹم — Madrasa Management System with Google Drive Sync`
   - **Visibility:** Choose **Public** (free GitHub Pages) or **Private** (needs GitHub Pro for Pages)
3. ⚠️ **Do NOT** check "Add a README" or "Add .gitignore" — we already have these
4. Click **Create repository**

### Step 2: Push Your Code to GitHub

After creating the repo, GitHub will show you commands. Open **PowerShell** in your project folder and run:

```powershell
git remote add origin https://github.com/YOUR_USERNAME/madrasa-management-system.git
git push -u origin main
```

> Replace `YOUR_USERNAME` with your actual GitHub username.

GitHub will ask for your **credentials**. If you don't have a Personal Access Token (PAT):
1. Go to [github.com/settings/tokens](https://github.com/settings/tokens)
2. Click **"Generate new token (classic)"**
3. Give it a name, select **repo** scope
4. Copy the token and use it as your password when pushing

### Step 3: Enable GitHub Pages (Free Hosting)

1. Go to your repo on GitHub → **Settings** → **Pages**
2. Under **Source**, select **Deploy from a branch**
3. Select **main** branch and **/ (root)** folder
4. Click **Save**
5. Wait 1-2 minutes — your app will be live at:
   ```
   https://YOUR_USERNAME.github.io/madrasa-management-system/
   ```

### Step 4: Update Google Cloud Console

This is the **most important step** — without this, Google Drive sync won't work on your live site.

1. Go to [Google Cloud Console → Credentials](https://console.cloud.google.com/apis/credentials)
2. Click on your OAuth Client ID (`Madrasa Web Client`)
3. Under **Authorized JavaScript origins**:

   | Action | URL |
   |---|---|
   | ✅ **Keep** | `http://localhost` |
   | ❌ **Remove** | `https://github.com` ← This is wrong, it's GitHub's website not yours |
   | ✅ **Add** | `https://YOUR_USERNAME.github.io` ← Your actual app URL |

4. Click **Save**

> ⚠️ **اہم:** `https://github.com` آپ کی ایپ نہیں ہے — یہ GitHub کی ویب سائٹ ہے۔ اسے ہٹا کر اپنا GitHub Pages URL شامل کریں۔

---

## 🛡️ Bonus: Recommended Security Settings

### A. Reset Your Client Secret (Recommended)

Since the `client_secret` value has been visible in this working session, it's good practice to reset it:

1. Go to [Google Cloud Console → Credentials](https://console.cloud.google.com/apis/credentials)
2. Click on your OAuth Client ID
3. Click **"Reset Secret"**
4. A new secret will be generated — this doesn't affect your app since we don't use the secret in browser code anyway

### B. Restrict API Access

1. In Google Cloud Console → **Credentials** → click your OAuth Client
2. Under **API restrictions** → select **Restrict key**
3. Only allow: **Google Drive API**

### C. Publish OAuth App (If Others Will Use It)

If your app is in **"Testing"** mode, only test users can sign in. To allow everyone:

1. Go to **OAuth consent screen**
2. Click **"Publish App"**
3. Google may review your app for sensitive scopes

> For personal/small madrasa use, keeping "Testing" mode and adding users manually is fine.

---

## 📞 Support

Created by: **Yasin Ullah** — Bannu Software Solutions
- Website: [www.yasinbss.com](https://www.yasinbss.com)
- WhatsApp: 03361593533
