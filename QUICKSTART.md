# Quick Start Guide - GitHub Pages App Store

## Step-by-Step Setup (5 minutes)

### Step 1: Create GitHub Repository
1. Go to https://github.com/new
2. Repository name: `my-app-store` (or any name you like)
3. Check "Add a README file"
4. Click "Create repository"

### Step 2: Upload Files
1. Click "Add file" → "Upload files"
2. Drag and drop these files:
   - `index.html`
   - `apps.js`
   - `.gitignore`
3. Click "Commit changes"

### Step 3: Create Downloads Folder
1. Click "Add file" → "Create new file"
2. Type: `downloads/README.txt`
3. Add some text: "App files go here"
4. Click "Commit changes"

### Step 4: Upload Your Apps
1. Navigate to the `downloads` folder
2. Click "Add file" → "Upload files"
3. Upload your app files (ZIP, EXE, APK, etc.)
4. Click "Commit changes"

### Step 5: Update App Catalog
1. Click on `index.html`
2. Click the pencil icon (Edit)
3. Scroll down to find the `apps` array (inside the `<script>` tag)
4. Update the app information:
   - Change `name`, `description`, `icon`, etc.
   - Update `downloadUrl` to match your file names
   - Change `developer` to your name
5. Click "Commit changes"

### Step 6: Enable GitHub Pages
1. Go to repository Settings
2. Click "Pages" in the left sidebar
3. Under "Source":
   - Select branch: `main`
   - Select folder: `/ (root)`
4. Click "Save"
5. Wait 1-2 minutes

### Step 7: Visit Your App Store!
Your site will be live at:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

## Example: Adding a New App

Edit `index.html`, find the `apps` array in the `<script>` section, and add:

```javascript
{
    name: "My Awesome App",
    developer: "Your Name",
    category: "Productivity",
    description: "This app helps you stay organized and productive.",
    version: "1.0.0",
    size: "3.2 MB",
    rating: "5.0",
    downloads: "100",
    icon: "🎯",
    downloadUrl: "downloads/my-awesome-app.zip"
}
```

Then upload `my-awesome-app.zip` to the `downloads` folder!

## Tips
- Use emojis for icons (they're fun and work everywhere!)
- Keep file sizes under 100MB (GitHub limit)
- Use `.zip` files for easy distribution
- Update the README.md with your own information

## Need Help?
- Check that file paths are correct
- Wait a few minutes for GitHub Pages to update
- Try hard refresh (Ctrl+Shift+R)

That's it! Your app store is live! 🚀
