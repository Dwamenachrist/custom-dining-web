# Custom Dining Website

A modern, responsive landing page for the Custom Dining mobile app - helping Nigerians with dietary restrictions find suitable meals at restaurants.

## 🌟 Features

- **Responsive Design**: Works perfectly on all devices
- **Modern UI/UX**: Clean, professional design with smooth animations
- **SEO Optimized**: Meta tags, sitemap, and robots.txt included
- **Fast Loading**: Optimized performance with minimal dependencies
- **Accessibility**: WCAG compliant for better user experience

## 🚀 Quick Start

### Local Development

1. **Clone the repository** (if using Git):
   ```bash
   git clone <repository-url>
   cd custom-dining-website
   ```

2. **Start local server**:
   ```bash
   # Option 1: Using Python (recommended)
   python -m http.server 8000
   
   # Option 2: Using Node.js http-server
   npx http-server -p 8000
   
   # Option 3: Using PHP
   php -S localhost:8000
   ```

3. **Open in browser**:
   Visit `https://custom-dining-web.vercel.app/`


## 📊 Google Search Console Setup

### 1. Add Property
1. Go to [Google Search Console](https://search.google.com/search-console/)
2. Click "Add Property"
3. Choose "URL prefix" and enter your domain
4. Verify ownership using one of these methods:
   - HTML file upload
   - HTML tag (already included in the `<head>`)
   - DNS record
   - Google Analytics
   - Google Tag Manager

### 2. Submit Sitemap
1. Once verified, go to "Sitemaps" in the left menu
2. Add your sitemap URL: `https://yourdomain.com/sitemap.xml`
3. Click "Submit"

### 3. Request Indexing
1. Use the URL inspection tool
2. Enter your main page URL
3. Click "Request Indexing"

## 🔧 Customization

### Update App Store Links
Replace the placeholder links in `script.js`:
```javascript
// Replace these with your actual app store URLs
window.open('https://play.google.com/store/apps/details?id=your.app.id', '_blank');
window.open('https://apps.apple.com/app/your-app-id', '_blank');
```

### Update Contact Information
- Email: Change `support@customdining.ng` in `index.html`
- Social media links in the footer section
- Phone number or additional contact methods

### Update Domain References
Update these files with your actual domain:
- `sitemap.xml`: Replace `https://customdining.ng/`
- `robots.txt`: Replace `https://customdining.ng/sitemap.xml`
- `package.json`: Update homepage URL

## 📱 Mobile App Integration

### Deep Linking
Add deep linking support to redirect users to your app:
```javascript
// Example deep link implementation
const openApp = () => {
    const isAndroid = /Android/i.test(navigator.userAgent);
    const isIOS = /iPhone|iPad|iPod/i.test(navigator.userAgent);
    
    if (isAndroid) {
        window.location = "intent://your-app-scheme#Intent;package=your.package.name;end";
    } else if (isIOS) {
        window.location = "your-app-scheme://";
    }
};
```

## 🎨 Design System

### Colors
- Primary: `#2563eb` (Blue)
- Secondary: `#1d4ed8` (Dark Blue)
- Text: `#1f2937` (Dark Gray)
- Background: `#ffffff` (White)
- Accent: `#f8fafc` (Light Gray)

### Typography
- Font Family: Inter (Google Fonts)
- Weights: 300, 400, 500, 600, 700

## 📈 SEO Features Included

- ✅ Meta descriptions and keywords
- ✅ Open Graph tags for social sharing
- ✅ Structured data (JSON-LD)
- ✅ Sitemap.xml
- ✅ Robots.txt
- ✅ Semantic HTML structure
- ✅ Alt tags for images
- ✅ Fast loading times

## 🔒 Security

- HTTPS only (configure in your hosting platform)
- Content Security Policy headers (add in hosting configuration)
- No external dependencies loaded from untrusted sources

## 📄 License

MIT License - feel free to use and modify as needed.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📞 Support

For technical support or questions:
- Email: support@customdining.ng
- Create an issue in this repository 