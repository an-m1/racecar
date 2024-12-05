
# Animation: 3D Oval Race Track with Dynamic Camera

## Project Overview
We developed a 3D animation of a two-car race on an oval track, featuring dynamic camera angles and transitions. The animation includes smooth motion, realistic object interaction, and scene-specific enhancements to create an immersive experience. We leveraged WebGL and Three.js for rendering and animation.

## Key Features
1. **Dynamic Camera Transitions**: The camera dynamically changes modes to offer different perspectives, such as bird’s-eye view and side views. Smooth interpolation ensures seamless transitions.
2. **Realistic Car Movement**: Cars follow an oval trajectory with variable speed to simulate natural motion. The motion incorporates acceleration and deceleration using trigonometric functions.
3. **Interactive Scene Elements**: Grass, track, and car models were built hierarchically to optimize rendering and enable interactivity.
4. **Responsive Design**: The animation adapts to different screen sizes, maintaining consistent aspect ratios and rendering quality.

## Libraries and Techniques
### Libraries
- **Three.js**: A lightweight JavaScript library used for 3D rendering and animations. It provides tools for camera manipulation, geometry creation, and lighting.
- **WebGL**: The foundation for rendering 3D graphics within the browser without additional plugins.

### Techniques
- **Hierarchical Modeling**: Used for creating the cars and other elements, allowing modular and reusable components.
- **Camera Interpolation**: Smooth camera transitions achieved using `lerpVectors` and easing functions.
- **Trigonometric Functions**: Implemented for smooth acceleration and deceleration of cars.
- **Event-Driven Resizing**: Ensures the scene adapts dynamically to window size changes.

## Implementation Details
### Scene Composition
- **Grass and Track**: The scene includes an outer square and an inner circular grass area, with the oval track rendered using `RingGeometry`.
- **Car Models**: Cars are designed with basic geometric shapes and assigned unique colors for visual distinction.

### Animation Logic
- **RequestAnimationFrame**: Utilized to synchronize the rendering loop with the browser’s refresh rate, optimizing performance.
- **Easing Functions**: `easeInOutQuad` smoothens camera transitions, avoiding abrupt changes.
- **Trigonometric Updates**: Car positions are updated based on sine and cosine functions to maintain a natural oval trajectory.

### Debugging Efforts
- Fixed alignment issues in car positioning and ensured smooth camera transitions.
- Resolved glitches such as z-fighting on the grass and track.
- Optimized performance to achieve stable frame rates across various hardware setups.

## Skills Demonstrated
- **3D Modeling and Animation**: Designing realistic car models and implementing dynamic animations.
- **Graphics Programming**: Using WebGL and Three.js for rendering and real-time updates.
- **Problem-Solving**: Debugging visual glitches and optimizing performance.
- **Responsive Design**: Ensuring adaptability to screen resizing.

## File Structure
- **HTML and JavaScript**: The main files (`main.html` and `main.js`) contain all the logic and rendering code.
- **Assets**: Organized textures and materials for grass, track, and other elements.

## Acknowledgments
This project was created as an educational exercise to explore WebGL animations and Three.js functionalities. All textures are either public domain or self-created.

---
