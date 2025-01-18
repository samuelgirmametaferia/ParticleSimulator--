
# Particle Simulator

**Particle Simulator** is an interactive web-based simulation tool where users can experiment with dynamic particles in various environments. Users can customize particle properties, container shapes, and interactions to create engaging visual effects and observe particle behaviors in real-time.

## Features

- **Customizable Particles:**
  - Select particle shapes: Circle or Square.
  - Adjust particle count dynamically.
  - Choose particle colors with an intuitive color picker.
  - Enable or disable blending for smooth visual effects.

- **Interactive Controls:**
  - Choose container shapes: Rectangle or Circle.
  - Enable/disable gravity to observe its effects on particles.
  - Switch between interaction modes: "Pull" (attractive) or "Push" (repulsive).
  - Configure collision types: Fluid or Bouncy interactions.

- **Responsive Canvas:**
  - Automatically adjusts to the browser's viewport for a seamless experience.

- **Real-Time Interaction:**
  - Apply forces to particles by clicking on the canvas.

- **Visual Effects:**
  - Enable blending for a stunning "screen" compositing effect.

## Technologies Used

- **HTML**: Structure of the application.
- **CSS**: Styling for a modern and responsive interface.
- **JavaScript**: Core functionality, particle physics, and interactions.
- **Canvas API**: For rendering particles and handling animations.

## Installation and Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/particle-simulator.git
   ```
2. **Navigate to the Directory**:
   ```bash
   cd particle-simulator
   ```
3. **Run Locally**:
   Open the `index.html` file in your browser.

4. **Interact with the Simulator**:
   - Use the controls to configure the simulation.
   - Click "Spawn Particles" to initialize particles with the selected properties.
   - Click anywhere on the canvas to apply forces.

## Controls Overview

| Control          | Description                                        |
|------------------|----------------------------------------------------|
| **Particle Shape** | Choose between Circle or Square particles.        |
| **Number of Particles** | Set the desired number of particles (minimum 1). |
| **Container Shape** | Select the simulation container shape: Rectangle or Circle. |
| **Gravity**        | Toggle gravity to observe downward force effects. |
| **Interaction Mode** | Choose between Pull (attractive) or Push (repulsive). |
| **Particle Color** | Pick a color for the particles using the color picker. |
| **Blending**       | Enable/disable particle color blending effects.   |
| **Collision Type** | Select Fluid or Bouncy collision behaviors.       |

## How It Works

- Particles are created dynamically and rendered onto a `canvas` element.
- Physics such as gravity, collision, and force application are simulated using custom JavaScript code.
- Particle behavior is updated frame-by-frame to provide smooth animations.

## Future Enhancements

- Add support for more particle shapes.
- Introduce velocity-based color transitions.
- Allow user-defined container dimensions.
- Save and load simulation states.

## License

This project is licensed under the [MIT License](LICENSE).

---
