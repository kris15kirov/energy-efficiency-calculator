# 🏢 EcoCalc - Building Energy Efficiency Calculator

A modern web application for calculating building heat loss and evaluating energy efficiency. Built with Node.js and vanilla JavaScript, featuring a sleek dark green theme inspired by professional design standards.

![EcoCalc Preview](https://img.shields.io/badge/Status-Active-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue)

## 🌟 Features

- **Heat Loss Calculation** - Calculate heat loss through building walls based on material, thickness, and temperature differential
- **Material Database** - Pre-loaded materials with thermal conductivity values (Concrete, Brick, Bitumen, Wood, Glass Wool)
- **Energy Efficiency Rating** - Visual indicator showing efficiency from Good to Poor
- **Bilingual Support** - Full English and Bulgarian language toggle
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **PWA Ready** - Progressive Web App support with service worker

## 🛠️ Technology Stack

- **Frontend**: HTML5, CSS3 (Vanilla), JavaScript (ES6+)
- **Backend**: Node.js, Express.js
- **Styling**: Custom CSS with glassmorphism effects
- **Icons**: Bootstrap Icons
- **Database**: Firebase Firestore (optional cloud sync)

## 🚀 Quick Start

### Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/kris15kirov/energy-efficiency-calculator.git
   cd energy-efficiency-calculator
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start the server**
   ```bash
   npm start
   ```

4. **Open in browser**
   - **Laptop**: http://localhost:3000
   - **Phone/Tablet** (same WiFi network): http://YOUR_LOCAL_IP:3000

## 📱 Accessing from Phone/Tablet (Demo Review)

To test on your mobile device while the server is running on your laptop:

1. Make sure your phone and laptop are on the **same WiFi network**
2. Find your laptop's local IP address:
   - **Mac**: Run `ipconfig getifaddr en0` in Terminal
   - **Windows**: Run `ipconfig` in Command Prompt, look for IPv4 Address
3. Open your phone's browser and navigate to: `http://[YOUR_IP]:3000`

**Example**: If your IP is `192.168.100.165`, open `http://192.168.100.165:3000` on your phone.

## 📐 How It Works

The calculator uses the following heat transfer formula:

```
Q = U × A × ΔT
```

Where:
- **Q** = Heat Loss (Watts)
- **U** = Thermal Transmittance (1/R, where R = thickness/λ)
- **A** = Surface Area (m²)
- **ΔT** = Temperature Difference (°C)

### Material Thermal Conductivity (λ)

| Material | λ (W/m·K) |
|----------|-----------|
| Concrete | 1.65 |
| Brick | 0.79 |
| Bitumen Insulation | 0.27 |
| Wood | 0.13 |
| Glass Wool | 0.04 |

## 🏛️ Project Information

This project was developed as part of a research initiative at the Bulgarian Academy of Sciences (BAS).

| Role | Name |
|------|------|
| **Student** | Kristiyan Kirov |
| **Mentor** | Dr. Veneta Yosifova |
| **Institute** | [IICT - Bulgarian Academy of Sciences](https://www.bas.bg/) |

**Address**: БАН IV км., ул. "Акад. Георги Бончев" 2, Блок 2, 1113 София

## 📁 Project Structure

```
energy-efficiency-calculator/
├── public/
│   ├── index.html      # Main HTML file
│   ├── styles.css      # Custom styling (dark green theme)
│   ├── script.js       # Application logic & translations
│   ├── manifest.json   # PWA manifest
│   └── service-worker.js
├── server.js           # Express server
├── package.json        # Dependencies
└── README.md
```

## 🌐 Language Support

Toggle between English and Bulgarian using the **EN / BG** button in the navigation bar. All UI elements, labels, and tooltips are fully translated.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

**© 2025 Energy Efficiency Project | Bulgarian Academy of Sciences**
