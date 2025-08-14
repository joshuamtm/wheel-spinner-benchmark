# 🎯 AI Platform Benchmark - Wheel Spinner

An interactive Wheel of Fortune-style spinner designed to benchmark AI coding platforms. This project serves as a standardized test to compare how different AI coding assistants (Replit, Cursor, Lovable, Claude Code) interpret and implement identical requirements.

## 🌐 Live Demo

[**Try it live here!**](https://joshuamtm.github.io/wheel-spinner-benchmark/)

## 🎮 Features

### Core Functionality
- **10-Slice Colorful Wheel**: Pre-populated with American names
- **Realistic Physics**: Smooth acceleration and deceleration mimicking Wheel of Fortune
- **Clear Winner Selection**: Red arrow points directly at the winning segment
- **Visual Feedback**: Winner segment brightens to white for clear identification
- **Celebration Effects**: 
  - Animated winner banner
  - 100+ confetti pieces with varied colors
  - Victory sound effects

### Interactive Elements
- **Click or Keyboard**: Spin with button click or spacebar/enter
- **Sound Design**: 
  - Variable-pitch clicking as wheel slows down
  - Celebratory chimes on win
- **Winner History**: Displays last 3 winners with gradient animations
- **Edit Mode**: Change names on-the-fly without page reload

### Design Philosophy
- **Zombo.com-Inspired**: Hypnotic gradients and early-web charm
- **Retro Aesthetic**: Comic Sans font, rainbow colors, pulsing animations
- **Desktop-First**: Optimized for desktop browsers with responsive scaling

## 🚀 Getting Started

### Option 1: Direct Browser
Simply open `index.html` in any modern web browser.

### Option 2: Local Server
```bash
git clone https://github.com/joshuamtm/wheel-spinner-benchmark.git
cd wheel-spinner-benchmark
python3 -m http.server 8000
# Visit http://localhost:8000
```

### Option 3: Deploy Your Own
Fork this repository and enable GitHub Pages in your repository settings.

## 🎯 Benchmark Purpose

This application was created to evaluate AI coding platforms across several dimensions:

### What We're Testing
1. **Interpretation of Requirements**: How each AI interprets ambiguous specs
2. **Technical Implementation**: Different approaches to the same problem
3. **Code Quality**: Structure, readability, and maintainability
4. **Feature Completeness**: All features implemented in one session
5. **Polish & UX**: Attention to detail and user experience

### Success Metrics
- ✅ Smooth animation performance (no jank)
- ✅ Accurate winner selection matching arrow position
- ✅ All MVP features functional
- ✅ Code clarity and organization
- ✅ Creative interpretation of "Zombo.com-inspired" aesthetic

## 🛠️ Technical Details

### Architecture
- **Platform**: Pure web technologies (HTML5, CSS3, JavaScript ES6+)
- **Graphics**: HTML5 Canvas API for wheel rendering
- **Audio**: Web Audio API for dynamic sound generation
- **Animation**: RequestAnimationFrame for smooth 60fps animation
- **State**: Client-side only (no backend/database required)

### Key Algorithms
- **Winner Calculation**: Precise angle mathematics to match arrow position
- **Easing Function**: Cubic ease-out for realistic deceleration
- **Sound Timing**: Dynamic pitch adjustment based on spin speed

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 📝 Customization

### Changing Names
1. Use the built-in edit mode in the UI
2. Or modify the `defaultNames` array in the code:
```javascript
const defaultNames = [
    'Your', 'Custom', 'Names', 'Here'
];
```

### Adjusting Colors
Modify the `colors` array to change segment colors:
```javascript
const colors = [
    '#ff006e', '#8338ec', '#3a86ff', // ... your colors
];
```

### Spin Duration
Adjust timing in the `spin()` function:
```javascript
const spinDuration = 4000 + Math.random() * 2000; // 4-6 seconds
```

## 🤝 Contributing

This is a benchmark project, but improvements are welcome! Please maintain the core feature set to ensure fair comparisons across platforms.

## 📄 License

MIT License - Use freely for your own benchmarking or entertainment!

## 🎉 Acknowledgments

- Inspired by Wheel of Fortune and Zombo.com
- Created as part of AI platform comparison research
- Built with Claude Code in a single session

---

**Remember**: At Zombo.com, anything is possible. The same goes for this wheel! 🌈✨