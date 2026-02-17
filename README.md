# When you need a reminder

A small iOS-friendly web app for when she’s feeling down. One tap shows a random comforting reminder (things you’ve said or general affirmations).

## How to use

1. **On iPhone**: Open `index.html` in Safari (from a link, or by hosting the folder). Tap **Share** → **Add to Home Screen** so it works like an app and opens full-screen.
2. Tap **“I need a reminder”** to see a random message. Use **“Another one”** for a different one, or **“← Back”** to return.

## Make it personal

Open `index.html` in any text editor and find the `reminders` array in the `<script>` section. Replace or add your own lines, for example:

- Things you’ve actually said to her
- Inside jokes or nicknames
- Promises or reasons you love her
- Short, kind affirmations

Keep each reminder in quotes and separated by commas. Example:

```javascript
const reminders = [
  "You're the reason I smile every morning.",
  "Remember when we said we'd always have each other's back? Still true.",
  "I love your laugh.",
  // add as many as you want
];
```

## Share without hosting

You can send her the app as files—no server or account needed.

**What you do**

1. Put these in one folder: `index.html`, `icon.png` (and your edited version is already there).
2. Zip that folder (right‑click → “Compress” on Mac, or “Send to → Compressed folder” on Windows).
3. Send her the zip however you like: **AirDrop**, **WhatsApp**, **email**, **Google Drive**, **iCloud**, **Dropbox**, etc.

**What she does (on iPhone)**

1. Open the zip (tap it) so it unpacks. She’ll see a folder with `index.html` and `icon.png`.
2. Tap **index.html**. If it opens in a preview or another app, tap **Share** → **Open in Safari**.
3. In **Safari**, tap the Share button (square with arrow) → **Add to Home Screen** → name it if she wants → **Add**. The heart icon will show on her home screen.

She has to open **index.html in Safari** (step 2) so “Add to Home Screen” is available. The app and icon work from the downloaded folder; nothing needs to be online.

---

## Host on GitHub (free link for her)

This gives you a link like `https://yourusername.github.io/carolina-reminder/` that she can open in Safari and add to her home screen.

**1. Create a new repo on GitHub**

- Go to [github.com](https://github.com) and sign in (create a free account if needed).
- Click **New** (green “New repository”).
- Name it something like **carolina-reminder** (or any name—no spaces).
- Leave it **Public**, don’t add a README or .gitignore.
- Click **Create repository**.

**2. Push this folder from your computer**

In a terminal (PowerShell or Command Prompt), go to this project folder and run:

```bash
cd "c:\Users\nacho\Desktop\Cursor Projects\App 3 Carolina"
git init
git add index.html icon.png README.md
git commit -m "Add reminder app"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/carolina-reminder.git
git push -u origin main
```

Replace **YOUR_USERNAME** with your GitHub username and **carolina-reminder** with your repo name if it’s different.

**3. Turn on GitHub Pages**

- On the repo page, go to **Settings** → **Pages** (left sidebar).
- Under **Source**, choose **Deploy from a branch**.
- Under **Branch**, select **main** and **/ (root)** → **Save**.
- Wait a minute or two. The link will be: **https://YOUR_USERNAME.github.io/carolina-reminder/**

**4. Send her the link**

She opens that URL in **Safari** on her iPhone, then **Share** → **Add to Home Screen**. Done.

No account or backend required—everything runs in the browser.
