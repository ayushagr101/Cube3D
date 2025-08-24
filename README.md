# 3D Cube Viewer

An interactive 3D cube visualization built with pure HTML and CSS, featuring smooth animations, dynamic lighting effects, and intuitive controls for exploring different perspectives.

## ✨ Features

- **Interactive 3D Cube**: Rotate and view the cube from 6 different angles
- **Smooth Animations**: Fluid transitions with cubic-bezier easing
- **Auto-Rotation**: Continuous 30-second rotation cycle when not manually controlled
- **Dynamic Background**: Animated gradient lighting with pulse and movement effects
- **Responsive Design**: Optimized for both desktop and mobile devices
- **Dual Control System**: Both button controls and dot indicators
- **Glass Morphism UI**: Modern frosted glass aesthetic with backdrop blur effects

## 🎯 Use Cases

Perfect for:
- **Product Showcases**: Display products from multiple angles
- **3D Model Previews**: Interactive model examination
- **Portfolio Projects**: Demonstrate 3D CSS skills
- **Educational Content**: Geometry and perspective learning
- **UI/UX Prototypes**: Modern interaction patterns

## 🚀 Getting Started

### Quick Setup

1. **Clone or Download** the project files
2. **Open `index.html`** in any modern web browser
3. **Start Exploring** - click the view buttons or dot indicators

### File Structure

```
3d-cube-viewer/
├── index.html          # Main HTML structure
├── style.css           # Complete styling and animations
└── README.md           # This documentation
```

## 🎮 How to Use

### Controls

- **View Buttons**: Click any of the 6 labeled buttons to rotate to that face
- **Dot Indicators**: Use the circular indicators below the cube for quick navigation
- **Reset Button**: Return to auto-rotation mode
- **Auto Mode**: Leave all controls unselected to watch continuous rotation

### Available Views

| View | Description |
|------|-------------|
| **Front** | Main product perspective |
| **Back** | Technical specifications panel |
| **Left** | Control interface side |
| **Right** | Connection ports side |
| **Top** | Overhead cooling system view |
| **Bottom** | Base mounting points |

## 🛠 Customization

### Changing Colors

Edit the CSS variables in `style.css`:

```css
:root {
    --primary-color: #ffffff;    /* Primary white color */
    --accent-color: #7a63ff;     /* Purple accent */
    --bg-color: #0a0a14;         /* Dark background */
}
```

### Modifying Cube Content

Update the content in each `.cube-face` div in `index.html`:

```html
<div class="cube-face front">
    Your Content Here
    <span>Subtitle text</span>
</div>
```

### Adjusting Animation Speed

Change the animation duration in `style.css`:

```css
.scene {
    animation: autoRotate 30s linear infinite; /* Change 30s to your preference */
}
```

### Cube Size

Modify the cube dimensions:

```css
.scene {
    width: 360px;    /* Change cube size */
    height: 360px;
}
```

### Required CSS Features

- CSS 3D Transforms
- CSS Grid/Flexbox
- CSS Custom Properties (Variables)
- Backdrop Filter (for blur effects)

## 🎨 Technical Highlights

### Advanced CSS Features Used

- **3D Transforms**: `perspective`, `transform-style: preserve-3d`
- **CSS Variables**: Dynamic theming system
- **Backdrop Filters**: Glass morphism effects
- **Complex Animations**: Keyframe animations with easing
- **CSS Grid & Flexbox**: Modern layout systems
- **Responsive Design**: Mobile-first approach

### Performance Optimizations

- **Hardware Acceleration**: Using `transform3d` for GPU rendering
- **Efficient Animations**: Animating only transform properties
- **Minimal JavaScript**: Pure CSS interactions where possible
- **Optimized Selectors**: Efficient CSS targeting

## 🔧 Advanced Modifications

### Adding New Faces

To add more cube faces (for shapes beyond a cube):

1. **Add HTML structure** for new faces
2. **Calculate transform values** for positioning
3. **Update control system** with new radio inputs
4. **Add corresponding CSS** for the new transforms

### Custom Animations

Create new animation sequences:

```css
@keyframes customRotation {
    0% { transform: rotateY(0deg) rotateX(0deg); }
    100% { transform: rotateY(180deg) rotateX(45deg); }
}
```

### Interactive Enhancements

Consider adding:
- Mouse drag controls
- Touch gestures for mobile
- Keyboard navigation
- Sound effects
- Loading states

## 📊 Performance Notes

- **Smooth 60fps** animations on modern devices
- **Lightweight**: No external dependencies
- **Fast Loading**: Minimal file sizes
- **Memory Efficient**: CSS-only animations

## 🤝 Contributing

Feel free to:
- Report bugs or issues
- Suggest new features
- Submit improvements
- Share your customizations

## 🙏 Acknowledgments

Built with modern CSS3 features and inspired by contemporary web design trends. Special focus on accessibility and performance optimization.

---

**Enjoy exploring your 3D cube!** 🎲
