---

# Particle Simulator

This is an interactive particle simulator built using HTML, CSS, and JavaScript. The application allows users to simulate particles inside a customizable container. Users can manipulate various aspects of the simulation, such as the number of particles, their shape, and the effects of gravity, collision, and interaction modes.

## Technologies Used

- **HTML**: Provides the structure of the web page, including the canvas for drawing particles and the controls for interacting with the simulation.
- **CSS**: Used for styling the page and positioning the elements (e.g., controls and canvas) for a clean and user-friendly interface.
- **JavaScript**: Powers the logic behind the particle simulation, enabling the creation, movement, and interaction of particles on the canvas.

## Features

- **Particle Shape**: Choose between a circular or square particle shape.
- **Particle Count**: Select the number of particles to spawn, with the option to customize the amount (up to a user-specified limit).
- **Container Type**: Choose between a rectangular or circular container for the simulation.
- **Gravity**: Toggle gravity on and off, which affects the downward force applied to particles.
- **Interaction Mode**: Choose between "pull" or "push" interaction modes that affect how the particles react when force is applied.
- **Collision Type**: Simulate two types of particle collisions: "fluid" (soft collisions) and "bouncy" (elastic collisions).
- **Particle Color**: Use a color picker to customize the color of the particles. Additionally, particles can change color based on their speed.
- **Blending Mode**: Option to enable or disable blending, affecting how particles overlap and interact visually.

## Why It Works

The simulator uses the **HTML5 canvas** to draw and animate the particles. The particles are represented as objects with properties like position, velocity, size, color, and shape. Here's how it all comes together:

1. **Particle Creation**: Particles are created with random positions and velocities within the canvas. Users can specify the number of particles and the shape they should take (circle or square).
  
2. **Movement and Gravity**: Each particle has velocity components (`vx`, `vy`) that are updated each frame based on gravity and other forces. Gravity can be toggled on or off, and when enabled, it applies a constant downward acceleration to the particles.

3. **Collision Detection**: The particles are checked for collisions with each other, and depending on the selected collision type, they either "bounce" off each other (elastic collision) or "push" through each other (fluid collision). This adds a layer of interaction that simulates real-world physical behavior.

4. **Container Boundaries**: The particles are constrained within a user-defined container. If the container is rectangular, particles bounce off the edges. In the case of a circular container, particles are reflected off the perimeter.

5. **User Interactions**: Users can interact with the particles by clicking or dragging on the canvas, which applies a force to the particles at the clicked location. The force can either "pull" or "push" particles, depending on the selected mode.

6. **Color and Blending**: Particles can change color based on their speed, with a smooth color transition (hue shift). The blending mode allows for visually appealing overlapping effects.

## Setup and Usage

1. **HTML Structure**: The HTML contains a canvas element where the simulation takes place. Control elements such as dropdowns and checkboxes allow users to customize the simulation parameters.

2. **JavaScript Logic**: The JavaScript handles all the particle physics, including motion, gravity, collision detection, and user interaction. The logic is encapsulated in a `Particle` class, and various functions control the spawning, updating, and rendering of particles.

3. **Interactivity**: As users change simulation parameters (e.g., particle shape, count, or container type), the particle simulation updates in real-time. Users can also apply forces by interacting with the canvas.

## Example of Usage

1. Open the page in a web browser.
2. Select the desired options from the control panel (e.g., particle shape, count, gravity, etc.).
3. Click the "Spawn Particles" button to start the simulation.
4. Interact with the canvas by clicking or dragging to apply forces to the particles.
5. Observe the particles' behavior based on the selected parameters.

--
## License

This project is licensed under the [MIT License](LICENSE).

---
