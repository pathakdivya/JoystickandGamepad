# 🎮 Joystick and Gamepad Visualizer

> Interactive browser-based visualizers for PlayStation and Xbox gamepads. Perfect for hardware testing, driver development, and gamepad debugging.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Live Demo](https://img.shields.io/badge/Demo-Live-success)](https://pathakdivya.github.io/JoystickandGamepad/)
[![Made with HTML5/CSS3/JS](https://img.shields.io/badge/Built%20with-HTML5%2FCSS3%2FJS-orange)](https://developer.mozilla.org/en-US/docs/Web/API/Gamepad_API)

## ✨ Features

### 📊 **Real-Time Button & Stick Visualization**
- Live display of all gamepad button states
- Thumbstick position tracking with visual feedback
- Trigger pressure/analog value monitoring
- D-Pad direction detection

### 🎯 **Dual Implementation Approaches**

> #### **PlayStation Visualizer**
> - Image-based controller outline (PNG diagram)
> - Complete button mapping for PS4/PS5 controllers
> - Visual feedback for all input types
> - Optimized for accurate hardware testing

> #### **Xbox Visualizer**
> - Pure SVG-based rendering
> - No external image dependencies
> - Self-contained and lightweight
> - Full support for Xbox wireless controllers

### 🔧 **Beginner Developer Friendly**
- Single HTML files — no build step required
- Works immediately in any modern browser
- Uses Browser Gamepad API for hardware detection
- Console logging for debugging

---

## 🚀 Getting Started

### **Quick Start (No Installation)**

Both visualizers are **fully self-contained**. Simply open them in your browser:

1. **PlayStation Visualizer** (image-based)
   - Open [`Playstation visualizer/playstation-gamepad-visualiser.html`](https://pathakdivya.github.io/JoystickandGamepad/Playstation%20visualizer/playstation-gamepad-visualiser.html)
   - Requires image assets in the `images/` folder

2. **Xbox Visualizer** (SVG-based)
   - Open [`Xbox Visualizer/xbox-visualiser.html`](https://pathakdivya.github.io/JoystickandGamepad/Xbox%20Visualizer/xbox-visualiser.html)
   - Completely self-contained, no dependencies

### **Local Testing**

If you clone this repository, simply open the html files with a double click for full functionality. 

## 📖 Usage

### **Connecting Your Gamepad**

1. **Plug in or pair your gamepad** via Bluetooth or USB
2. **Press any button** to activate it in the browser
3. **Watch the visualization** respond to all your inputs in real-time

### **What You'll See**

- **Button States** – Individual button presses highlighted with color changes
- **Stick Positions** – Left and right analog sticks tracked with crosshair indicators
- **Trigger Values** – Analog pressure displayed as progress bars or color intensity
- **Status Panel** – Controller connection state, vibration support, raw axis/button values

### **Troubleshooting**

| Issue | Solution |
|-------|----------|
| Controller not detected | Press a button or move a stick to "wake up" the gamepad. Some devices require initial input. |
| Buttons seem reversed | Check your gamepad model; Xbox and PlayStation use different button mappings (intentional). |
| Stick drift visible | This is normal for controller aging. You can test calibration by centering the sticks. |
| In case page served via `file://` not working | Use a local server (Python, Node, Live Server) instead and raise an issue in the repo. |

---

## 🏗️ Architecture

### **File Structure**

```
JoystickandGamepad/
├── README.md                                    # Main documentation
├── LICENSE                                      # GNU GPLv3
│
├── Playstation visualizer/
│   ├── playstation-gamepad-visualiser.html     # Standalone HTML file (56 KB)
│   ├── playstation_readme.md                   # Feature summary
│   └── images/                                 # Controller diagram assets
│       └── Controller_2d.png
│
└── Xbox Visualizer/
    ├── xbox-visualiser.html                    # Standalone HTML file (35 KB)
    ├── xbox_readme.md                          # Feature summary
    └── (no external dependencies)
```

### **Technology Stack**

- **Frontend** – HTML5, CSS3, Vanilla JavaScript (no frameworks)
- **Hardware API** – [W3C Gamepad API](https://w3c.github.io/gamepad/) for controller input
- **Rendering** – DOM manipulation (PlayStation) and SVG (Xbox)
- **Styling** – CSS Grid, Flexbox, CSS variables

## 🧪 Testing & Validation

### **Supported Controllers**

✅ PlayStation 4/5 DualShock 4 & DualSense  
✅ Xbox One & Xbox Series X/S  
✅ Logitech F310 / F710  
✅ Generic HID gamepads (depends on OS support)  

### **Browser Support**

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome/Edge | ✅ Full | Recommended; best Gamepad API support |
| Firefox | ✅ Full | Excellent compatibility |
| Safari | ⚠️ Partial | Gamepad API support varies by version |
| Internet Explorer | ❌ None | Not supported; use modern browser |

### **Use Cases**

- **Game Development** – Test controller input during game development
- **Driver Debugging** – Verify hardware mapping and calibration
- **Accessibility Testing** – Confirm button/stick responsiveness
- **Hardware Validation** – Quick spot-check for gamepad functionality
- **Educational** – Learn how the Gamepad API works

---

## 📝 License

This project is licensed under the **GNU General Public License v3.0**. See [`LICENSE`](LICENSE) for details.

**Summary:** You are free to use, modify, and distribute this software, provided you include this license and make any modifications open source under the same license.

---

## 🤝 Contributing

Found a bug? Have a suggestion? Feel free to:
- **Test** on different gamepads and browsers
- **Report issues** in the GitHub issues tracker
- **Submit pull requests** for improvements
- **Share** this project with others who are planning to use gamepads.

---

## 📚 Acknowledgement 

- **[W3C Gamepad API Specification](https://w3c.github.io/gamepad/)** – Official API documentation
- **[MDN Gamepad API Guide](https://developer.mozilla.org/en-US/docs/Web/API/Gamepad_API)** – Browser support and usage examples
- **[PlayStation Button Mapping](https://en.wikipedia.org/wiki/PlayStation_controller)** – PS controller layout reference
- **[Xbox Button Mapping](https://en.wikipedia.org/wiki/Xbox_controller)** – Xbox controller layout reference

<div align="center">

**Made with ❤️ for the researchers planning on adopting new response methods in behavioural science**

</div>
