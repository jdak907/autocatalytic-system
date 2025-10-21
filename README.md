# Autocatalytic System

This project is a visual and narrated exploration of autocatalytic AI growth, where capability produces more capability, constraints become endogenous variables, and exponential is merely the baseline and not the ceiling. The simulation renders a coupled system of AI capability, capacity limits, energy, compute, data, and multiplicative productivity to show how feedback turns curves into trajectories. The presentation style borrows a page from The Hitchhiker's Guide to the Galaxy: a calm British narrator explaining something potentially civilization-bending as though it were a slightly inconvenient footnote in an interstellar travel manual. The goal is equal parts clarity, inevitability, and perspective, because if we are going to watch the curve go vertical we might as well do it with British composure and without panicking.

## 🎯 Overview

An interactive 3D visualization that models autocatalytic AI systems through coupled differential equations, featuring:

- **Real-time 3D curve rendering** with WebGL
- **Narrated explanation** with British voice synthesis
- **Mathematical equations** rendered with MathJax
- **CRT-style visual effects** for retro-futuristic aesthetics
- **Responsive design** that works across devices

## 🚀 Quick Start

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd autocatalytic-system-1
   ```

2. **Start a local server**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in browser**
   ```
   http://localhost:8000
   ```

4. **Click "ACTIVATE"** to begin the experience

## 🛠️ Technical Stack

### Core Technologies
- **HTML5** - Semantic structure and accessibility
- **CSS3** - Custom properties, animations, and responsive design
- **JavaScript ES6+** - Modern async/await, modules, and performance optimizations
- **WebGL** - Hardware-accelerated 3D graphics via Three.js

### Dependencies
- **[Three.js v0.161.0](https://threejs.org/)** - 3D graphics library
- **[MathJax v3](https://www.mathjax.org/)** - Mathematical equation rendering
- **Web Speech API** - Text-to-speech synthesis
- **Web Audio API** - Audio context management

### Browser Requirements
- **WebGL 1.0+** support
- **ES6 modules** support
- **Web Speech API** support (for narration)
- **Modern JavaScript** features (async/await, arrow functions)

## 🧮 Mathematical Model

The simulation implements a coupled system of differential equations modeling autocatalytic AI growth:

### Core Variables
- **I(t)** - AI Capability (grows with feedback)
- **K(t)** - Carrying Capacity (constraint ceiling)
- **E(t)** - Energy Budget (resource limitation)
- **A(t)** - Algorithms (efficiency multiplier)
- **C(t)** - Compute Power (processing capacity)
- **D(t)** - Data Quality (training material)
- **P(t)** - Productivity (multiplicative output)

### Key Equations
```
P(t) = γ A^α C^χ D^η
I'(t) = rI(1 - I/K)(1 + p_eff·P)
```

### System Dynamics
- **Positive feedback loops** between capability and capacity
- **Resource constraints** that evolve endogenously
- **Multiplicative productivity** from combined factors
- **Exponential growth** as baseline behavior

## 🎨 Visual Design

### CRT Aesthetic
- **Green phosphor glow** effects using CSS text-shadow
- **Scanline patterns** with repeating linear gradients
- **Flicker animation** simulating CRT refresh
- **Retro-futuristic** color palette

### 3D Visualization
- **Animated curves** showing system evolution
- **Glowing halos** around data lines
- **Starfield background** with parallax drift
- **Grid and axes** with subtle glow effects

### Responsive Layout
- **Fixed viewport** with full-screen canvas
- **Flexible HUD** elements that adapt to screen size
- **Touch-friendly** controls for mobile devices

## 🔊 Audio System

### Voice Synthesis
- **British accent** preference with fallback options
- **Calm, measured delivery** matching the narrative tone
- **User gesture unlock** for browser autoplay policies
- **Persistent settings** stored in localStorage

### Audio Features
- **Voice toggle** control
- **Automatic timing** synchronized with visual elements
- **Error handling** for unsupported browsers

## ⚡ Performance Optimizations

### Code Optimizations
- **CSS custom properties** for consistent theming
- **Named constants** replacing magic numbers
- **Proper geometry disposal** preventing memory leaks
- **Cached DOM elements** reducing query overhead
- **Efficient rendering loops** with requestAnimationFrame

### Memory Management
- **Three.js geometry disposal** on updates
- **Texture cleanup** for sprites and materials
- **Event listener cleanup** on component unmount
- **Garbage collection** friendly object patterns

### Rendering Performance
- **WebGL power preference** set to high-performance
- **Pixel ratio limiting** to prevent over-rendering
- **Efficient curve generation** with optimized algorithms
- **Background tab pausing** to save resources

## 🏗️ Architecture

### Module Structure
```
index.html
├── CSS Styles (custom properties, animations)
├── HTML Structure (semantic elements, accessibility)
├── JavaScript Modules
│   ├── MathJax Integration
│   ├── Voice Synthesis System
│   ├── Three.js 3D Scene
│   ├── Simulation Engine
│   ├── Curve Rendering
│   └── UI Controls
└── External Dependencies (CDN)
```

### Key Components
- **Simulation Engine** - Mathematical model computation
- **3D Renderer** - WebGL scene management
- **Audio Manager** - Voice synthesis and timing
- **UI Controller** - User interaction handling
- **Animation Loop** - Frame-by-frame updates

## 🔧 Development

### Code Quality
- **ESLint** compatible JavaScript
- **Semantic HTML** with proper ARIA labels
- **Accessible design** with keyboard navigation
- **Cross-browser** compatibility testing

### Performance Monitoring
- **Frame rate** monitoring in development
- **Memory usage** tracking for WebGL objects
- **Console warnings** for debugging
- **Error boundaries** for graceful degradation

## 📱 Browser Support

### Fully Supported
- **Chrome 80+** - Full feature support
- **Firefox 75+** - Full feature support
- **Safari 13+** - Full feature support
- **Edge 80+** - Full feature support

### Limited Support
- **Mobile browsers** - Touch controls, reduced effects
- **Older browsers** - Graceful degradation

## 🐛 Troubleshooting

### Common Issues
- **WebGL not supported** - Shows fallback message
- **Audio not working** - Check browser permissions
- **MathJax not loading** - Check network connection
- **Performance issues** - Try reducing pixel ratio

### Debug Mode
Open browser console to see:
- **Performance metrics**
- **Error messages**
- **WebGL context info**
- **Audio context status**

## 📄 License

This project is open source. See the repository for license details.

## 🤝 Contributing

Contributions welcome! Please:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📞 Support

For issues or questions:
- Check the troubleshooting section
- Review browser console for errors
- Ensure all dependencies are loading
- Test in a supported browser