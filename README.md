# VWO JSLIB Testing Demo Site

A simple demo website designed for testing VWO (Visual Website Optimizer) JSLIB functionality.

## Features

- **Header**: Navigation bar with logo and menu links
- **Footer**: Footer with copyright and links
- **Interactive Buttons**: Multiple styled buttons for A/B testing
- **Content Sections**: Various content areas for testing modifications
- **Responsive Design**: Works on desktop and mobile devices

## Structure

```
Testsite/
├── index.html      # Main HTML file
├── styles.css      # CSS styling
├── script.js       # JavaScript functionality
└── README.md       # This file
```

## Getting Started

1. Clone or download this repository
2. Open `index.html` in a web browser
3. Or serve it using a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js (http-server)
   npx http-server
   ```

## VWO Integration

To integrate VWO JSLIB:

1. Sign up for a VWO account at [vwo.com](https://vwo.com)
2. Get your VWO account ID
3. Add the VWO script to `index.html` before the closing `</head>` tag:
   ```html
   <script type="text/javascript">
     window._vwo_code = window._vwo_code || (function(){
       var account_id=YOUR_ACCOUNT_ID,
       settings_tolerance=2000,
       library_tolerance=2500,
       use_existing_jquery=false,
       // ... rest of VWO code
     })();
   </script>
   ```

## Testing Elements

The site includes several testable elements:

- **Buttons**: Primary, Secondary, Success, and Danger buttons with unique IDs
- **Navigation Links**: Header navigation links
- **Content Sections**: Hero section, button section, and content cards
- **Footer Links**: Privacy and Terms links

## Deployment to GitHub Pages

1. Create a new repository on GitHub
2. Push this code to your repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: VWO testing demo site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```
3. Go to repository Settings > Pages
4. Select the `main` branch and `/ (root)` folder
5. Your site will be available at `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

This is a demo project for testing purposes.

