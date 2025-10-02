# Ellipse Ring Staircase Generator

**A modern tool for designing and building spiral staircases in Minecraft, Enshrouded, and other voxel-based survival games**

## Features

- **Intuitive Staircase Design**: Design spiral staircases by total height and rotation angle
- **Dual View Modes**: Switch between 2D top-down view and 3D visualization
- **Builder Mode**: Full-screen step-by-step guide with keyboard controls for in-game building
- **Flexible Configuration**: Create partial spirals (90°, 180°) or multi-rotation towers (720°+)
- **Starting Angle Control**: Rotate where your staircase begins (0°-315°)
- **Modern UI**: Clean Material Design 3 interface with dark/light themes
- **Mirror Controls**: Link width/height for perfect circles or separate for ellipses
- **Interactive 3D Camera**: Full mouse and keyboard navigation controls
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Live Demo

**[Try it now →](https://netrokus.github.io/ellipse-and-staircase-generator/)**

## Preview

![Preview](https://github.com/netrokus/ellipse-and-staircase-generator/blob/main/screenshots/preview.png)

## How to Use

### Basic Setup

1. **Set Outer Ellipse**: Define the outer boundary of your staircase ring
2. **Set Inner Ellipse**: Define the inner hollow area (makes it a ring)
3. **Configure Staircase**:
   - **Total Height**: How many steps/blocks tall (4-100 blocks)
   - **Rotation**: How far around the circle (45°-720°)
   - **Start Angle**: Where the staircase begins (0°-315°)
   - **Direction**: Spiral up or down

### 2D Mode (Top-Down View)

Perfect for placing blocks precisely:

- Shows current step from bird's-eye view
- Use **Previous/Next** buttons to cycle through steps
- Grid overlay shows exact block positions
- Colored ellipse outlines (red=outer, blue=inner)

### 3D Mode (Visualization)

See your complete staircase design in three dimensions:

- **View All Steps**: See the entire spiral structure
- **Single Step Mode**: Click the view mode icon to toggle - builds incrementally, one step at a time
- **Camera Controls**:
  - Drag to rotate view
  - Shift + drag to pan
  - Mouse wheel to zoom
  - WASD/Arrow keys to move camera
  - Q/E to move up/down

### Builder Mode (NEW!)

Full-screen building assistant for in-game construction:

1. Click **Builder** button in top bar
2. Step counter shows current step number
3. Use arrow keys or on-screen buttons to navigate
4. Info panel shows all parameters at a glance
5. Press **ESC** to exit builder mode

**Perfect for**: Having on a second monitor or tablet while building in-game

## Understanding the Controls

### Staircase Parameters

**Total Height**: The number of steps (blocks) from bottom to top
- Example: Height of 20 creates a 20-block tall staircase

**Rotation**: How far the stairs wrap around the ring in degrees
- 90° = quarter circle
- 180° = half circle  
- 360° = full circle
- 720° = two complete rotations

**Starting Angle**: Where your first step begins (0°-315°)
- 0° = starts at the right (3 o'clock position)
- 90° = starts at the top (12 o'clock position)
- 180° = starts at the left (9 o'clock position)
- 270° = starts at the bottom (6 o'clock position)

**How they work together**: 
- Height=20, Rotation=360° → 20 steps evenly distributed around a full circle (18° per step)
- Height=15, Rotation=180° → 15 steps spanning half the circle (12° per step)
- Height=40, Rotation=720° → tall spiral tower with two full rotations (18° per step)

### Mirror Controls

Click the sync icon (⟲) to link width and height:
- **Linked (active/blue)**: Creates perfect circles - changing one value updates the other
- **Unlinked (inactive/gray)**: Creates ellipses with independent dimensions

### Keyboard Shortcuts

**3D Mode Navigation:**
- `W` / `↑` - Move camera forward
- `S` / `↓` - Move camera backward
- `A` / `←` - Move camera left
- `D` / `→` - Move camera right
- `Q` - Move camera up
- `E` - Move camera down

**Builder Mode:**
- `→` / `↓` - Next step
- `←` / `↑` - Previous step
- `ESC` - Exit builder mode

## Technical Details

- **Single-file application**: No installation or dependencies needed
- **Canvas 2D rendering**: Precise grid-based top-down view
- **Three.js r128**: Hardware-accelerated 3D visualization
- **Instanced rendering**: Efficiently handles thousands of blocks
- **Optimized shadows**: Disabled for cleaner visualization
- **Transparent inner ring**: Blue semi-transparent blocks show the inner boundary
- **Theme system**: Seamless dark/light mode switching with CSS variables

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

**Note**: 3D mode requires WebGL support (available in all modern browsers)

## Installation

### Option 1: Use Online
Visit the [live demo](https://netrokus.github.io/ellipse-and-staircase-generator/)

### Option 2: Download
1. Download the HTML file
2. Open in any modern web browser
3. No installation required - works offline

### Option 3: Self-Host
```bash
git clone https://github.com/netrokus/ellipse-and-staircase-generator.git
cd ellipse-and-staircase-generator
# Open the HTML file in your browser
```

## Use Cases

**Minecraft Towers**: Create spiral staircases for towers and lighthouses  
**Enshrouded Builds**: Design elegant circular stairs for multi-level structures  
**Other Voxel Games**: Any game with block-based building  

**Pro Tip**: Use Builder Mode on a second monitor or tablet - keep it visible while building in-game for step-by-step guidance

## Project Structure

The staircase consists of:
- **Outer ellipse ring** (red outline): The outer boundary
- **Inner ellipse ring** (blue outline): The hollow center (shown as semi-transparent blocks in 3D)
- **Step wedges**: Sections of the ring between inner and outer ellipses, one per step

Each step occupies an angular section of the ring, calculated by dividing the total rotation by the number of steps.

## Credits

### Inspired By
- **Timothy Miller**, Binghamton University
- [Original Minecraft Circle Generator](https://www.cs.binghamton.edu/~millerti/circlegen.html)

### This Tool
A reimagined approach to building spiral staircases in voxel games:
- Height and rotation-based staircase design system
- Dual 2D/3D view modes with seamless switching
- Full-screen builder mode for in-game construction
- Material Design 3 UI with dark/light themes
- Optimized 3D rendering with instanced meshes
- Starting angle control for flexible designs
- Step-by-step navigation system
- Simplified controls focused on practical building use cases
- Mobile-responsive interface

## Contributing

Contributions welcome! Submit issues and pull requests on GitHub.

### Development
1. Fork the repository
2. Make changes to the HTML file
3. Test in multiple browsers (especially 3D mode)
4. Ensure all controls work as expected
5. Submit pull request with description of changes

### Future Ideas
- Export as schematic files (.schem/.nbt)
- Save/load staircase designs (localStorage/JSON)
- Pattern presets library (common sizes)
- Material/block type selection and preview
- Share designs via URL parameters
- Animation showing construction sequence
- Print mode for step-by-step instructions
- Multi-staircase support (double helix)

## Changelog

### v2.0 (Current)
- ✨ Added Builder Mode with full-screen interface
- ✨ Added Starting Angle control (0°-315°)
- 🐛 Fixed all missing function implementations
- 🐛 Fixed theme switching in 2D mode
- 🎨 Improved CSS for builder mode overlays
- ⚡ Streamlined codebase and removed redundant code
- 📝 Enhanced keyboard navigation in builder mode

### v1.0
- Initial release with 2D/3D modes
- Basic ellipse and staircase controls
- Theme switching support

## License

MIT License - Open source and free to use

Original circle generation algorithm by Timothy Miller, Binghamton University  
Staircase implementation and modern interface by netrokus

---

**Built with vanilla JavaScript, HTML5 Canvas, and Three.js**  
**No frameworks, no build process, no dependencies to install**