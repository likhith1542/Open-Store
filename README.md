# Open Store - GitHub Pages

A beautiful, responsive app store hosted on GitHub Pages where you can publish and share your applications for download.

## 🚀 Features

- **Modern Design**: Beautiful gradient UI with smooth animations
- **Search & Filter**: Find apps easily with search and category filters
- **Downloadable Apps**: Direct download links for your applications
- **Responsive**: Works perfectly on desktop, tablet, and mobile
- **Easy to Update**: Simple JavaScript file to add/edit apps
- **Free Hosting**: Powered by GitHub Pages

## 📦 Setup Instructions

### 1. Fork or Clone This Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git
cd YOUR-REPO-NAME
```

### 2. Create the Downloads Folder

Create a `downloads` folder in your repository to store your app files:

```bash
mkdir downloads
```

### 3. Add Your Apps

Place your application files (ZIP, EXE, APK, DMG, etc.) in the `downloads` folder:

```
downloads/
├── task-manager-pro.zip
├── photo-editor.zip
├── code-snippets.zip
└── your-app.zip
```

### 4. Update the App Catalog

Edit the `index.html` file and find the `apps` array (near the bottom, inside the `<script>` tag):

```javascript
const apps = [
    {
        name: "Your App Name",
        developer: "Your Name",
        category: "Productivity",  // Categories: Productivity, Graphics, Developer Tools, Health, Entertainment, Finance, etc.
        description: "A brief description of your app",
        version: "1.0.0",
        size: "2.5 MB",
        rating: "4.8",
        downloads: "1.2K",
        icon: "🚀",  // Use any emoji
        downloadUrl: "downloads/your-app.zip"  // Path to your file
    },
    // Add more apps here...
];
```

**Alternative:** You can keep the apps in a separate `apps.js` file if you prefer, but make sure it loads before the main script.

### 5. Enable GitHub Pages

1. Go to your repository on GitHub
2. Click **Settings** → **Pages**
3. Under **Source**, select `main` branch
4. Click **Save**
5. Your site will be live at: `https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/`

### 6. Customize (Optional)

- **Change Colors**: Edit the CSS gradient in `index.html` (search for `#667eea` and `#764ba2`)
- **Update Title**: Change the `<h1>` and `<title>` tags
- **Add Your GitHub Link**: Update the footer link to point to your repository

## 📝 Adding New Apps

To add a new app:

1. Upload your app file to the `downloads/` folder
2. Edit `index.html` and find the `apps` array in the `<script>` section
3. Add a new entry to the array
4. Commit and push your changes:

```bash
git add .
git commit -m "Added new app: Your App Name"
git push origin main
```

Your app store will update automatically!

## 🎨 App Categories

Available categories (you can add more):
- Productivity
- Graphics
- Developer Tools
- Health
- Entertainment
- Finance
- Education
- Games
- Utilities
- Business

## 📱 File Structure

```
your-repo/
├── index.html          # Main app store page (contains app catalog inside)
├── downloads/          # Your app files go here
│   ├── app1.zip
│   ├── app2.zip
│   └── ...
└── README.md           # This file
```

**Note:** The app catalog is now embedded in `index.html` to avoid loading issues. You can optionally use a separate `apps.js` file if you configure it correctly.

## 🌟 Tips

- **File Size**: Keep app files under 100MB for faster downloads
- **File Formats**: Use `.zip` for cross-platform apps, or platform-specific formats (`.exe`, `.dmg`, `.apk`)
- **Descriptions**: Write clear, concise descriptions (1-2 sentences)
- **Icons**: Use emojis for icons - they're simple and work everywhere
- **Versions**: Use semantic versioning (major.minor.patch)

## 🔧 Troubleshooting

**Apps won't download?**
- Make sure files are in the `downloads/` folder
- Check that the `downloadUrl` path is correct
- Verify files are committed and pushed to GitHub

**Site not updating?**
- GitHub Pages can take a few minutes to update
- Try hard refresh (Ctrl+Shift+R or Cmd+Shift+R)
- Clear browser cache

**Large files?**
- GitHub has a 100MB file size limit
- Consider using external hosting (Google Drive, Dropbox) for large files
- Update the `downloadUrl` to the external link

## 📄 License

Free to use for personal and commercial projects.

## 🤝 Contributing

Feel free to customize this app store for your needs!

---

Made with ❤️ using GitHub Pages
