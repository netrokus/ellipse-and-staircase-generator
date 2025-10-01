# Ellipse Ring Staircase Generator

**A modern tool for designing and building spiral staircases in Minecraft, Enshrouded, and other voxel-based survival games**

## Features

- **Intuitive Staircase Design**: Design spiral staircases by total height and rotation angle
- **Dual View Modes**: Switch between 2D top-down view and 3D visualization
- **Step-by-Step Building**: Navigate through individual steps to build precisely
- **Flexible Configuration**: Create partial spirals (90°, 180°) or multi-rotation towers (720°+)
- **Modern UI**: Clean Material Design interface with dark/light themes
- **Mirror Controls**: Link width/height for perfect circles or separate for ellipses
- **Interactive Camera**: Full 3D controls with mouse and keyboard navigation
- **Responsive Design**: Works seamlessly on desktop and mobile devices

## Live Demo

**[Try it now →](https://netrokus.github.io/ellipse-and-staircase-generator/)**

## How to Use

### Basic Setup

1. **Set Outer Ellipse**: Define the outer boundary of your staircase ring
2. **Set Inner Ellipse**: Define the inner hollow area (makes it a ring)
3. **Configure Staircase**:
   - **Total Height**: How many blocks tall (4-100 blocks)
   - **Rotation**: How far around the circle (45°-720°)
   - **Direction**: Spiral up or down

### 2D Mode (Top-Down View)

Perfect for placing blocks precisely:

- Shows current step from bird's-eye view
- Use **Previous/Next** buttons to cycle through steps
- Grid overlay shows exact block positions
- Ellipse outlines help with alignment

### 3D Mode (Visualization)

See your complete staircase design:

- **View All Steps**: See the entire spiral structure
- **Single Step Mode**: Build incrementally, one step at a time
- **Camera Controls**:
  - Drag to rotate view
  - Shift + drag to pan
  - Mouse wheel to zoom
  - WASD/Arrow keys to move
  - Q/E to move up/down

## Understanding the Controls

### Staircase Parameters

**Total Height**: The number of steps (blocks) from bottom to top
- Example: Height of 20 creates a 20-block tall staircase

**Rotation**: How far the stairs wrap around the ring in degrees
- 90° = quarter circle
- 180° = half circle  
- 360° = full circle
- 720° = two complete rotations

**How they work together**: 
- Height=20, Rotation=360° → 20 steps evenly distributed around a full circle (18° each)
- Height=15, Rotation=180° → 15 steps spanning half the circle (12° each)
- Height=40, Rotation=720° → tall spiral tower with two full rotations (18° each)

### Mirror Controls

Click the sync icon to link width and height:
- **Linked (active)**: Creates perfect circles
- **Unlinked**: Creates ellipses with different dimensions

## Technical Details

- **Single-file application**: No installation needed
- **Canvas 2D rendering**: Precise grid-based top-down view
- **Three.js 3D rendering**: Hardware-accelerated visualization
- **Instanced rendering**: Handles thousands of blocks smoothly
- **No shadows**: Clean visualization without confusing artifacts
- **Theme system**: Seamless dark/light mode switching

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

Note: 3D mode requires WebGL support (available in all modern browsers)

## Installation

### Option 1: Use Online
Visit the [live demo](https://netrokus.github.io/ellipse-and-staircase-generator/)

### Option 2: Download
1. Download `index.html`
2. Open in any modern web browser
3. No installation required

### Option 3: Self-Host
```bash
git clone https://github.com/netrokus/ellipse-and-staircase-generator.git
cd ellipse-and-staircase-generator
# Open index.html in your browser
```

## Use Cases

**Minecraft Towers**: Create spiral staircases for towers and lighthouses
**Enshrouded Builds**: Design elegant circular stairs for multi-level structures  
**Other Voxel Games**: Any game with block-based building

**Tip**: Use 2D mode while building in-game to see exactly which blocks to place for each step

## Credits

### Inspired By
- **Timothy Miller**, Binghamton University
- [Original Minecraft Circle Generator](https://www.cs.binghamton.edu/~millerti/circlegen.html)

### This Tool
A reimagined approach to building spiral staircases in voxel games:
- Height and rotation-based staircase design system
- Dual 2D/3D view modes with seamless switching
- Step-by-step building guide for precise construction
- Material Design 3 UI with dark/light themes
- Optimized 3D rendering with transparent inner ellipse visualization
- Simplified controls focused on practical building use cases
- Mobile-responsive interface

## Contributing

Contributions welcome! Submit issues and pull requests.

### Development
1. Fork the repository
2. Make changes
3. Test in multiple browsers
4. Submit pull request

### Future Ideas
- Export as schematic files
- Save/load staircase designs
- Pattern presets library
- Material/block type selection
- Share designs via URL
- Animation of construction sequence

## License

MIT License - Open source and free to use

Original algorithm by Timothy Miller, Binghamton University
