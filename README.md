# Task Reminder - Voice to Calendar Sync

A mobile-first web app for iPhone that captures voice commands and syncs them to your Calendar with automatic reminders.

## Features

✅ **Voice Input** - Just speak your task naturally
✅ **Calendar Sync** - Automatically generates .ics files for iPhone Calendar
✅ **Smart Reminders** - Set custom reminder times (1-7 days before)
✅ **Branch Tracking** - Assign tasks to specific branches/employees
✅ **Native iOS Feel** - Optimized for iPhone, installable as app
✅ **Local Storage** - All data saved on your phone
✅ **Zero Backend** - Works completely offline

## Quick Start

### 1. **For Testing (Development)**

#### Option A: Quick Local Test
```bash
# Navigate to the project folder
cd task-reminder-app

# Start a simple Python server
python3 -m http.server 8000

# Open in browser: http://localhost:8000
```

#### Option B: Using Node.js
```bash
# Install http-server globally (if not already installed)
npm install -g http-server

# Run from the project directory
http-server

# Open in browser: http://localhost:8080
```

---

### 2. **Deploy to Free Hosting**

#### **Option A: GitHub Pages (Recommended - FREE)**

1. **Create a GitHub account** (if you don't have one)
   - Go to https://github.com and sign up

2. **Create a new repository**
   - Click "+" → New repository
   - Name it: `task-reminder` (or any name)
   - Make it **Public**
   - Click "Create repository"

3. **Upload the app files**
   - Click "Upload files"
   - Drag & drop the `index.html` file
   - Commit changes

4. **Enable GitHub Pages**
   - Go to Settings → Pages
   - Under "Source", select `main` branch
   - Click Save
   - Wait 2-3 minutes

5. **Access your app**
   - Your app will be at: `https://yourusername.github.io/task-reminder`
   - Share this link with others

---

#### **Option B: Netlify (FREE - Easiest)**

1. **Go to** https://netlify.com and sign up (use GitHub login)

2. **Deploy**
   - Drag & drop your project folder onto Netlify
   - It deploys instantly
   - You get a URL like: `https://random-name.netlify.app`

3. **Custom Domain** (Optional)
   - Go to Site Settings → Custom Domain
   - Add your domain

---

#### **Option C: Vercel (FREE)**

1. **Go to** https://vercel.com

2. **Sign in with GitHub**

3. **Import your repository**
   - Click "New Project"
   - Select your GitHub repo
   - Deploy (automatic)

4. **Share your live URL**

---

#### **Option D: Traditional Web Hosting (Paid - ~$5-15/month)**

- **Bluehost**: https://bluehost.com (easiest)
- **NameCheap**: https://namecheap.com (cheapest)
- **GoDaddy**: https://godaddy.com
- **SiteGround**: https://siteground.com (best support)

**Upload via FTP:**
1. Buy hosting plan
2. Use FTP client (FileZilla, Cyberduck)
3. Upload `index.html` to public folder
4. Access at your domain

---

### 3. **Add to Your iPhone Home Screen**

Once hosted online:

1. **Open your app URL in Safari** on your iPhone
2. **Tap Share** (bottom center)
3. **Tap "Add to Home Screen"**
4. **Name it** (e.g., "Task Reminder")
5. **Tap Add**
6. **Icon appears on your home screen!**

Now it works like a native app.

---

## Testing Checklist

- [ ] Voice recording works
- [ ] Date/time picker works
- [ ] Branch dropdown works
- [ ] "Add to Calendar" button works
- [ ] .ics file downloads (check Downloads)
- [ ] Calendar app opens with the event
- [ ] Reminder notification appears
- [ ] Tasks persist after refresh
- [ ] Delete tasks works

---

## Customize for Your Company

### Add your branches:
Edit these lines in `index.html`:
```html
<select id="taskBranch">
    <option value="">Select branch...</option>
    <option value="Dubai">Dubai</option>
    <option value="Abu Dhabi">Abu Dhabi</option>
    <option value="Doha">Doha</option>
    <option value="Head Office">Head Office</option>
</select>
```

### Change app name/logo:
- Edit `<title>` tag
- Edit `<h1>` in header
- Change Apple icon (base64 SVG in meta tag)

### Change colors:
Find these and change:
- `#007AFF` → Your brand blue
- `#34C759` → Your brand green
- `#FF3B30` → Your warning red

---

## How It Works

1. **User speaks** → Speech API captures audio
2. **Transcript appears** → User confirms/edits
3. **Sets date & branch** → Picks when/where
4. **Clicks "Add to Calendar"** → Generates .ics file
5. **Calendar app opens** → Event added automatically
6. **Reminder triggers** → On the scheduled date/time

---

## File Structure

```
task-reminder-app/
├── index.html          # Complete app (all-in-one file)
├── README.md          # This file
└── DEPLOYMENT.md      # Detailed deployment guide
```

---

## Browser Support

- ✅ Safari (iOS 14+) - **Best**
- ✅ Chrome (Desktop & Android)
- ✅ Firefox
- ✅ Edge
- ⚠️ Internet Explorer - Not supported

---

## FAQ

**Q: Does it work offline?**
A: Yes! Tasks save locally. Calendar sync needs internet for download.

**Q: Can I backup my tasks?**
A: Yes. Tasks are in browser's localStorage. Export via developer console or add export feature.

**Q: How do I delete the app?**
A: On iPhone, press & hold app icon → Remove App → Delete

**Q: Does it use my location?**
A: No. No tracking, no analytics, no permissions needed.

**Q: Can multiple people use it?**
A: Yes, if they visit the same URL. Each phone stores tasks separately.

---

## Support

Need help?
1. Check the testing checklist above
2. Clear browser cache (Safari Settings → Websites)
3. Try a different browser
4. Check iPhone Settings → Safari → Allow Cross-Site Tracking

---

## Version History

- **v1.0** (May 2026) - Initial release
  - Voice input
  - Calendar sync
  - Task management
  - iPhone optimization

---

## License

Free to use and modify for your business.

**Created**: May 2026
