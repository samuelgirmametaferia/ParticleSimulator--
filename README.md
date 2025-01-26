# Particle Simulator README

## Overview

Welcome to **Particle Simulator**, an interactive tool designed to help users explore and experiment with the dynamics of particles within various physics-based environments. This tool allows you to visualize particle interactions, including gravity, collisions, and other forces, in real time. It is especially beneficial for educators in physics classrooms who want to incorporate more interactive teaching methods.

The simulator provides users with full control over the properties of the particles and the environment, enabling them to customize their simulations to explore a wide range of physical phenomena.

## Key Features

- **Interactive Controls**: Customize particle shapes, count, size, and behavior to suit your simulation needs.
- **Real-Time Physics**: Observe particles interacting under forces like gravity and collisions for an immersive experience.
- **Dynamic Visualization**: Change particle colors and interaction modes to visualize different physical phenomena.
- **Customizable Containers**: Choose between different container shapes (rectangles, circles) to confine particle movements.
- **Velocity-Based Coloring**: Visualize particle speed using color gradients, providing a deeper understanding of the simulation.
- **Responsive Design**: Enjoy a seamless experience across various devices and screen sizes.
- **Performance Alerts**: Get notified when particle counts exceed optimal limits to maintain smooth simulation performance.

## How to Use

### Basic Setup
1. **Controls Panel**: 
   - Customize the particles using the controls panel. You can set the particle shape, size, count, and behavior.
   - You can toggle gravity, change the interaction mode (e.g., pull or push), and select the container shape (rectangle or circle).

2. **Canvas Interactions**:
   - Click or drag on the canvas to apply forces to the particles and see their movement and interaction.
   - Press the "Spawn Particles" button to initialize or reset the simulation with your selected configurations.
   - Change between different interaction modes and visual effects to observe various physical effects.

### Features in Detail
- **Shape Selector**: Choose between different particle shapes (circle, square, or hexagon).
- **Particle Count**: Set the number of particles you want to simulate. The default value is 256, but you can increase or decrease the number of particles.
- **Gravity**: Toggle gravity on or off to simulate the effect of gravitational force on the particles.
- **Interaction Mode**: Select the interaction mode, where you can apply either a "pull" or "push" force on the particles.
- **Coloring Options**: 
  - **Single Color**: Use the color picker to select a single color for all particles.
  - **Velocity Color Mode**: Particles are colored based on their speed, offering a visual representation of particle velocity.
  - **Random Color**: Each particle gets a random color.
  - **Collision Mode**: Color changes can be triggered upon particle collisions (for dynamic feedback).
  
### Container Options
- **Rectangular Container**: Particles are confined within a rectangular boundary.
- **Circular Container**: Particles are confined within a circular boundary centered on the canvas.

### Collisions
- **Elastic Collisions**: When particles collide, they bounce off each other as though the collisions are perfectly elastic.
- **Fluid Mode**: In this mode, collisions are more fluid-like, with particles separating based on distance and moving with softened interactions.

### Performance Alerts
- The simulator includes warnings when the number of particles exceeds a level that could lead to performance issues. For large numbers of particles, be mindful of system performance.

## Requirements

- **Browser**: The simulator is web-based and works across all modern browsers (Chrome, Firefox, Safari, Edge).
- **Device**: Optimized for use on desktops, tablets, and mobile devices.

## Installation

To run the Particle Simulator locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo/particle-simulator.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd particle-simulator
   ```

3. **Open `index.html`** in your web browser to start the simulator.

## Code Structure

Here’s a breakdown of the key components in the code:

### `index.html`
- This is the main HTML file where the canvas and the control elements (sliders, buttons, etc.) are defined.

### `script.js`
- Contains the main JavaScript code responsible for managing the simulation, including:
  - **Particle Class**: Defines particle behavior, including movement, drawing, and collision detection.
  - **Simulation Functions**: Handles particle spawning, collision detection, force application, and animation.
  - **UI Elements**: Updates particle properties based on user input, such as shape, size, count, gravity, and more.

### `styles.css`
- CSS file for styling the UI elements, including the canvas and control panels.

## User Interface

The user interface consists of:

- **Particle Settings Panel**: Allows you to customize particle shapes, count, size, and behavior.
- **Canvas Area**: Where the particles are visualized in real-time.
- **Control Panel**: Adjust the simulation settings, including the interaction mode, gravity, and container shape.

### Key Controls
- **Shape**: Select the particle shape (circle, square, or hexagon).
- **Count**: Set the number of particles in the simulation.
- **Max Size**: Adjust the maximum particle size.
- **Gravity**: Toggle gravity on or off.
- **Mode**: Choose the interaction mode (pull or push).
- **Container Shape**: Choose between a rectangular or circular container for the particles.
- **Coloring**: Choose a coloring mode (single color, random color, velocity-based, or collision-based).
- **Spawn Particles**: Create new particles based on the selected settings.

## Performance Considerations

While the Particle Simulator can handle a large number of particles, it’s important to keep in mind that very high particle counts can impact performance, especially on lower-end devices or browsers. The tool will warn you when the particle count is getting too high, but it's always a good idea to experiment within reasonable limits for optimal performance.

## Troubleshooting

- **Simulation Lag**: If the simulation slows down, try reducing the particle count or disabling certain effects like velocity coloring.
- **No Particle Movement**: Ensure that gravity is enabled or apply forces by clicking or dragging on the canvas.
- **Collision Mode Not Working**: Ensure you're using the correct collision mode and that particles are overlapping during collisions.

## Future Enhancements

- **More Physics Models**: Incorporate additional physics models like elasticity, drag, or more complex interactions.
- **Improved UI**: Provide better user interface elements, including presets for common setups or configurations.
- **Particle Trails**: Allow users to visualize particle trajectories for a more dynamic experience.

## License

This project is open-source and released under the [MIT License](LICENSE).

---

**Enjoy experimenting with particle dynamics and uncovering fascinating physical phenomena!**
