# 📏 Screen Ruler Calibration Tool

A web-based screen measurement tool that provides accurate on-screen rulers in multiple units (cm, mm, meters, inches, and feet). Perfect for designers, developers, and anyone who needs to measure things on their screen with precision.

![Screen Ruler Demo](https://img.shields.io/badge/status-active-success.svg)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=flat&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E)

## ✨ Features

- **Easy Calibration**: Use any object with a known size (credit card, ruler, etc.) to calibrate your screen
- **Multiple Units**: Switch between centimeters, millimeters, meters, inches, and feet
- **Accurate Measurements**: Calculates precise pixels-per-millimeter ratio for your specific screen
- **Screen Information**: Displays your screen resolution, pixels per cm, and DPI
- **Responsive Design**: Works on any screen size or device
- **No Installation Required**: Pure HTML, CSS, and JavaScript - just open and use
- **Beautiful UI**: Modern gradient design with smooth animations

## 🚀 Quick Start

### Option 1: Direct Use
1. Download `index.html`
2. Open it in any modern web browser
3. That's it! No server or dependencies needed

### Option 2: Clone Repository
```bash
git clone https://github.com/samyakrajbayar/screen-ruler.git
cd screen-ruler
open index.html
```

## 📖 How to Use

### Step 1: Calibrate Your Screen
1. Find an object with a known size (recommended: credit card - 85.6mm wide)
2. Hold the object against the colored calibration bar on screen
3. Enter the exact size of your reference object
4. Select the unit (mm, cm, or inches)
5. Click "Calibrate"

### Step 2: Use the Rulers
- Switch between different units using the tabs
- The ruler will display accurate measurements for your screen
- Use the ruler to measure anything on your screen

### Step 3: View Screen Information
- Check your screen's resolution
- See pixels per centimeter
- View approximate DPI

## 💡 Calibration Tips

**Recommended Reference Objects:**
- **Credit Card**: 85.6mm (8.56cm or 3.37 inches) wide - most accurate
- **US Dollar Bill**: 156mm (6.14 inches) wide
- **Standard Ruler**: Use any marked measurement
- **A4 Paper**: 210mm (21cm or 8.27 inches) wide

**For Best Results:**
- Use a flat, rigid object
- Ensure your browser is at 100% zoom (not zoomed in/out)
- Hold the object directly against your screen
- Use the longest dimension possible for better accuracy

## 🛠️ Technical Details

### Technologies Used
- Pure HTML5
- Vanilla JavaScript (no frameworks or libraries)
- CSS3 with modern gradients and animations

### How It Works
1. User provides a reference measurement
2. JavaScript calculates the pixel width of the calibration bar
3. Determines pixels-per-millimeter ratio: `pixelsPerMM = barWidth / referenceSizeMM`
4. Renders rulers with accurate tick marks based on the calculated ratio
5. Supports unit conversion for all measurement systems

### Browser Compatibility
- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Opera
- ✅ Any modern browser with JavaScript enabled

## 📱 Use Cases

- **Designers**: Quickly measure UI elements and spacing
- **Developers**: Verify pixel-perfect implementations
- **E-commerce**: Display product sizes accurately
- **Education**: Teaching measurement and unit conversion
- **General Use**: Measure anything on your screen without a physical ruler

## 🎨 Customization

The tool is easy to customize. Key variables in the code:

```javascript
const units = {
    'mm': { multiplier: 1, major: 10, medium: 5, minor: 1, label: 'mm', maxLength: 300 },
    'cm': { multiplier: 10, major: 10, medium: 5, minor: 1, label: 'cm', maxLength: 30 },
    // ... add more units as needed
};
```

Modify colors in the CSS:
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

## ⚠️ Limitations

- Accuracy depends on proper calibration with a known reference object
- Browser zoom level must be at 100% for accurate measurements
- Different monitors have different pixel densities
- Screen scaling (Windows/Mac display settings) may affect accuracy

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

