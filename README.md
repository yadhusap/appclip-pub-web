# SuccessFactors App Clip Website

A clean, streamlined website designed for GitHub Pages hosting to support iOS App Clip functionality.

## 🚀 Features

- **App Clip Ready**: Configured with proper meta tags for iOS App Clip integration
- **Responsive Design**: Works on all devices and screen sizes
- **GitHub Pages Optimized**: Minimal, fast-loading single page
- **Apple App Site Association**: Properly configured for App Clip universal links

## 📁 Structure

```
├── index.html                    # Main landing page
└── apple-app-site-association    # App Clip configuration
```

## 🔧 GitHub Pages Setup

1. **Fork/Upload** this repository to your GitHub account
2. **Enable GitHub Pages** in repository settings
3. **Update URLs** in `index.html`:
   - Replace `your-github-username` with your GitHub username
   - Replace `your-repo-name` with your repository name
4. **Configure Apple Developer**:
   - Update Team ID in `apple-app-site-association`
   - Configure App Store Connect for App Clips

## 🎯 App Clip Integration

The website supports these App Clip experiences:
- **Performance**: `/experience/performance`
- **Learning**: `/experience/learning` 
- **Career**: `/experience/career`
- **Recognition**: `/experience/recognition`

## 🔗 Universal Links

When hosted on GitHub Pages, the following URLs will trigger App Clip experiences:
- `https://your-username.github.io/your-repo/experience/performance`
- `https://your-username.github.io/your-repo/experience/learning`
- `https://your-username.github.io/your-repo/experience/career`
- `https://your-username.github.io/your-repo/experience/recognition`

## ⚙️ Configuration

### Update apple-app-site-association
Replace `BKLUW64YWG` with your Apple Developer Team ID:

```json
{
  "appclips": {
    "apps": ["YOUR_TEAM_ID.com.successfactors.mobile.SFTestAppClip"]
  },
  "applinks": {
    "details": [
      {
        "appID": "YOUR_TEAM_ID.com.successfactors.mobile.SFTestAppClip",
        "paths": ["/experience/*"]
      }
    ]
  }
}
```

### Update Open Graph Tags
In `index.html`, update the image URLs:

```html
<meta property="og:image" content="https://your-username.github.io/your-repo/preview.jpg">
<meta property="og:url" content="https://your-username.github.io/your-repo">
```

## 🧪 Testing

1. **Local Testing**: Use Python's built-in server
   ```bash
   python3 -m http.server 8000
   ```

2. **GitHub Pages**: Access your site at `https://your-username.github.io/your-repo`

3. **App Clip Testing**: Test on iOS device with your App Clip installed

## 📱 Requirements

- iOS 14+ for App Clip functionality
- Valid Apple Developer account
- App Store Connect configuration
- HTTPS hosting (GitHub Pages provides this)

---

Built for seamless App Clip experiences 🍎