# Ellipse & Staircase Generator

**A modern, enhanced version of the Minecraft Circle Generator with Material Design UI and 3D visualization**

![Preview](https://github.com/netrokus/ellipse-and-staircase-generator/blob/main/screenshots/preview.png)

## 🌟 Features

- **Interactive Ellipse Generation**: Create precise ellipses and circles for survival game builds
- **3D Staircase Visualization**: View your spiral staircases in full 3D with interactive camera controls
- **Fill Steps Mode**: Generate solid wedge-shaped steps instead of single-line spokes for gap-free staircases
- **Progressive Building**: Watch your staircase build incrementally, step by step, in 3D
- **Modern UI**: Clean Material Design interface with intuitive controls
- **Dark/Light Themes**: Eye-friendly themes with seamless switching
- **Mirror Controls**: Link width/height for perfect circles or separate for ellipses
- **Responsive Design**: Works seamlessly on desktop and mobile devices
- **Smart Interface**: Controls automatically show/hide based on context
- **Zoom & Pan**: Navigate in both 2D and 3D with mouse and keyboard controls
- **Selection Tool**: Click and drag to highlight specific areas in 2D mode

## 🚀 Live Demo

**[Try it now →](https://netrokus.github.io/ellipse-and-staircase-generator/)**

## 🎮 How to Use

### 2D Mode (Default)
1. **Set Dimensions**: Adjust outer and inner ellipse width/height
2. **Configure Spokes**: Set spoke count and navigate through individual spokes
3. **Toggle Fill Steps**: Enable to create solid wedge-shaped steps instead of single lines
4. **Choose Display**: Select fit mode (window, width, or height)
5. **Interact**: 
   - Left-click + drag to select areas
   - Right-click + drag to pan
   - Mouse wheel to zoom in/out

### 3D Mode
1. **Click "2D Mode" button** in the header to switch to 3D visualization
2. **Set Staircase Parameters**:
   - Choose direction (upward or downward spiral)
   - Adjust step height
   - Set starting spoke position
3. **View Modes**:
   - **Show All Steps**: View the complete spiral staircase
   - **Show Single Step**: Build the staircase incrementally using Previous/Next buttons
4. **Navigate**:
   - Drag to rotate the camera around the staircase
   - Shift + drag to pan the camera
   - Mouse wheel to zoom in/out
   - **WASD** or **Arrow keys** to move the camera
   - **Q/E** to move up/down

## 🛠️ Controls

### Ellipse Controls
- **Width/Height**: Set ellipse dimensions (3+ for outer, 1+ for inner)
- **Mirror Button**: 🔗 Link width/height for perfect circles
- **+/- Buttons**: Quick increment/decrement values

### Spoke Controls
- **Count**: Number of spokes (4-64)
- **Fill Steps**: Toggle between single-line spokes and solid wedge-shaped steps
- **Previous/Next**: Navigate through individual spokes (2D) or build incrementally (3D single step mode)

### 3D Staircase Controls (3D Mode Only)
- **View Mode**: Toggle between showing all steps or building incrementally
- **Direction**: Choose upward or downward spiral
- **Step Height**: Control the vertical distance between each step (0.5-5 blocks)
- **Start Spoke**: Set which spoke the spiral begins from (visible in "Show All Steps" mode)

### Display Options (2D Mode Only)
- **Fit to Window**: Auto-scale to fit container
- **Fit Width**: Scale to container width
- **Fit Height**: Scale to container height

## 💻 Technical Details

- **Pure HTML/CSS/JavaScript**: Single-file application, runs entirely in browser
- **Canvas-based 2D Rendering**: Smooth, scalable 2D graphics
- **Three.js 3D Rendering**: Hardware-accelerated 3D visualization with instanced rendering for performance
- **CSS Custom Properties**: Theme system with seamless dark/light mode switching
- **Responsive Grid System**: Adapts to all screen sizes with scrollable controls
- **Smart UI**: Context-aware interface that shows/hides controls based on current mode
- **Optimized Performance**: Instanced mesh rendering for thousands of blocks without lag

## 🎨 Themes

The application includes two carefully crafted themes:

- **Light Theme**: Clean, professional appearance for daytime use
- **Dark Theme**: Easy on the eyes for extended building sessions (default)

Theme toggles instantly and affects both 2D and 3D rendering.

## 🗃️ Installation & Setup

### Option 1: Direct Download
1. Download `index.html` from this repository
2. Open in any modern web browser
3. No installation required!

### Option 2: Local Development
```bash
git clone https://github.com/netrokus/ellipse-and-staircase-generator.git
cd ellipse-and-staircase-generator
# Open index.html in your browser
```

### Option 3: Host Your Own
Deploy to any static hosting service:
- **GitHub Pages**: Enable in repository settings
- **Netlify**: Drag and drop the HTML file
- **Vercel**: Connect your GitHub repository

## 🔧 Browser Compatibility

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+

**Note**: 3D mode requires WebGL support (available in all modern browsers).

## 📜 Credits & Attribution

### Original Work
- **Creator**: Timothy Miller, Binghamton University
- **Original Tool**: [Minecraft Circle Generator](https://www.cs.binghamton.edu/~millerti/circlegen.html)
- **Institution**: Computer Science Department, Binghamton University

### Enhancements
This version builds upon the original with:
- **3D visualization mode** with full camera controls and progressive building
- **Fill Steps feature** for creating solid, gap-free staircases
- Internal ellipse and customizable spoke system for spiral staircases
- Complete UI/UX redesign using Material Design 3 principles
- Dark/light theme system with instant switching
- Responsive layout for mobile and desktop devices
- Context-aware interface with smart control visibility
- Modern CSS Grid and Flexbox layout
- Hardware-accelerated 3D rendering with Three.js
- Optimized performance with instanced rendering
- Enhanced accessibility features

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues and enhancement requests.

### Development Setup
1. Fork the repository
2. Make your changes
3. Test across different browsers (especially 3D mode)
4. Submit a pull request

### Ideas for Future Enhancements
- [ ] Export as image/SVG
- [ ] Save/load patterns
- [x] 3D visualization mode
- [ ] Pattern library/presets
- [ ] Block material selection
- [ ] Measurement tools
- [ ] VR mode support
- [ ] Animation playback of staircase construction

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

The original algorithm and concept are credited to Timothy Miller, Binghamton University.
