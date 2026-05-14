# 🔄 Google Drive Sync Setup Guide
## مدرسہ مینجمنٹ سسٹم — گوگل ڈرائیو سنک سیٹ اپ

This guide will walk you through setting up Google Drive backup & sync for your Madrasa Management System.

---

## 📋 Prerequisites

- A Google account (Gmail)
- Your app running on a URL (e.g., `http://localhost/testingspace/`)
- 10 minutes of time

---

## 🚀 Step-by-Step Setup

### Step 1: Go to Google Cloud Console

1. Open [https://console.cloud.google.com](https://console.cloud.google.com)
2. Sign in with your Google account

### Step 2: Create a New Project

1. Click the project dropdown at the top (next to "Google Cloud")
2. Click **"New Project"**
3. Enter a name: `Madrasa Management System`
4. Click **"Create"**
5. Make sure the new project is selected in the dropdown

### Step 3: Enable Google Drive API

1. In the left sidebar, go to **APIs & Services → Library**
2. Search for **"Google Drive API"**
3. Click on it, then click **"Enable"**

### Step 4: Configure OAuth Consent Screen

1. Go to **APIs & Services → OAuth consent screen**
2. Select **"External"** and click **"Create"**
3. Fill in the required fields:
   - **App name:** `Madrasa Management System`
   - **User support email:** your email
   - **Developer contact email:** your email
4. Click **"Save and Continue"**
5. On the **Scopes** page, click **"Add or Remove Scopes"**
   - Search and add: `https://www.googleapis.com/auth/drive.file`
   - Search and add: `https://www.googleapis.com/auth/drive.appdata`
   - Click **"Update"** then **"Save and Continue"**
6. On the **Test Users** page:
   - Click **"Add Users"**
   - Add your Gmail address (the one you'll use to sync)
   - Click **"Save and Continue"**
7. Click **"Back to Dashboard"**

> **⚠️ IMPORTANT:** While your app is in "Testing" mode, only the test users you added can use Google Sign-In. To allow anyone, you'll need to publish the app (Step 7).

### Step 5: Create OAuth 2.0 Credentials

1. Go to **APIs & Services → Credentials**
2. Click **"+ Create Credentials" → "OAuth client ID"**
3. Set **Application type:** `Web application`
4. **Name:** `Madrasa Web Client`
5. Under **Authorized JavaScript origins**, click **"+ Add URI"** and add:
   - `http://localhost` (for local development)
   - `http://localhost:80` (optional)
   - If hosted online, add your domain too (e.g., `https://yourdomain.com`)
6. Leave **Authorized redirect URIs** empty (not needed for this flow)
7. Click **"Create"**
8. **📋 Copy the Client ID** — it looks like:
   ```
   123456789-abcdefgh.apps.googleusercontent.com
   ```

### Step 6: Paste Client ID in Your App

1. Open `index.html` in your code editor
2. Search for this line (around line ~5461):
   ```javascript
   const CLIENT_ID = 'YOUR_CLIENT_ID.apps.googleusercontent.com';
   ```
3. Replace `YOUR_CLIENT_ID.apps.googleusercontent.com` with the Client ID you copied
4. Example:
   ```javascript
   const CLIENT_ID = '123456789-abcdefgh.apps.googleusercontent.com';
   ```
5. Save the file

### Step 7: (Optional) Publish Your App for All Users

If you want anyone (not just test users) to use Google Sign-In:

1. Go to **OAuth consent screen**
2. Click **"Publish App"**
3. Google may require a verification process for apps with sensitive scopes

> For personal/small madrasa use, keeping it in "Testing" mode and adding your users is fine.

---

## ✅ Testing

1. Open your app: `http://localhost/testingspace/`
2. Login as `admin` / `admin@123`
3. Go to **ترتیبات** (Settings — gear icon in sidebar)
4. Scroll down to **ڈیٹا بیک اپ و بحالی** section
5. Click **"گوگل ڈرائیو پر محفوظ کریں"** (Save to Google Drive)
6. A Google sign-in popup will appear — sign in with a test user account
7. You should see the progress bar fill up and a success message
8. To test restore: Click **"گوگل ڈرائیو سے بحال کریں"** (Restore from Google Drive)

---

## 🔧 Troubleshooting

| Problem | Solution |
|---------|----------|
| Google popup blocked | Allow popups for localhost in your browser |
| "Access blocked" error | Make sure your email is added as a Test User (Step 4.6) |
| "Not a valid origin" error | Make sure `http://localhost` is in Authorized JavaScript Origins (Step 5.5) |
| Google services not loading | Check internet connection, try refreshing the page |
| "idpiframe_initialization_failed" | Clear browser cookies/cache, or try incognito mode |
| Popup closes immediately | Try a different browser or disable ad-blockers |

---

## 📁 What Gets Synced

Everything in your database gets backed up as a single compressed ZIP file:

- ✅ Students (طلبا)
- ✅ Teachers (اساتذہ)
- ✅ Classes (جماعتیں)
- ✅ Fee Structures & Collections
- ✅ Salaries & Expenses
- ✅ Attendance (Student & Staff)
- ✅ Exams & Results
- ✅ Timetable
- ✅ Library & Hostel
- ✅ Donations & Fines
- ✅ Inventory
- ✅ Certificates
- ✅ Settings & Users
- ✅ Academic Years & Promotions

---

## 🔒 Security Notes

- Your data is stored in Google Drive's **hidden app folder** — only this app can access it
- The backup file is NOT visible in your regular Google Drive
- Google OAuth tokens are session-only (not stored permanently)
- No data is sent to any third-party server — it goes directly from your browser to Google Drive

---

## 📞 Support

Created by: **Yasin Ullah** — Bannu Software Solutions
- Website: [www.yasinbss.com](https://www.yasinbss.com)
- WhatsApp: 03361593533
