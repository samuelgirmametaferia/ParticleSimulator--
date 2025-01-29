Particle Simulator README

## Overview

Welcome to **Particle Simulator**, an interactive tool devised to let users experiment and explore the dynamics of particles inside different physics-based environments. The following simulator gives an insight into the visualization of these particles interacting against their fellows, gravity, or even other sources acting as a potential force. That helps lots and might be very valuable for physics teachers who want to include interactive approaches in their teachings.

This will allow complete control over the properties of the particles and the environment in the personalization of their simulation for studying a wide variety of physical phenomena.

## Key Features

* **Interactive Controls**: Change the shape, number, and size of the particles and their behavior regarding everything that may be required from the simulation.
* **Real-time Physics**: Interaction of the particles by the use of forces, including gravity and collision, with the purpose of obtaining realism.
Dynamic Visualization: Color of particles, mode of interaction can be changed for visualizing a wide range of physical phenomena. Customizable Containers: Rectangular, Circular shapes for containing particles. Velocity Colouring: Enhanced way of visualization of particle speed through colour gradients for better understanding of simulation. Responsiveness: Seamless user experiences across a multitude of devices and screen sizes.
- **Performance Indicator**: Notification when the number of particles is higher than the number that can be smoothly processed.

How to Use

### Basic Setup
1. **Controls Panel** : 
   - In the controls panel you are able to change particle settings: particle shape, size, count, behavior.
You are able to turn gravity on/off, change interaction mode, default is pull or push and select container shape: rectangle or circle.

2. **Canvas Interactions:**
Click anywhere in the canvas to exert forces on the particles, and observe the motion of the particles. Click the "Spawn Particles" button to start or restart the simulation with desired settings. Use the mode switches to turn on and off various modes of interaction as well as various visual effects in order to demonstrate various physical phenomena.

### Features in Detail
Shape Picker: Circle, square, or hexagon; pick one. Particle Count: The number of particles to project. By default 256. Raise it if you feel too small the amount, turn down vice-versa. Gravity: on/off Gravity is an option on/off to be set for simulation to work like a gravitational pull. Interaction Mode: Different kinds of interactions could be provided or applied as in "pull or "push forces to particles. Color Choices
- **Single Color**: Choose one color using the color picker for all particles.
- **Velocity Color Mode**: Each particle gets a color according to their speed so that one can visually see the velocity of the particles.
 - **Random Color**: Each particle gets a random color.
- **Collision Mode**: Color changes can be activated by the collision of particles dynamic feedback.

Container Options
- **Rectangular Container**: Particles will be bound inside the area of a rectangle.
- **Circular Container**: Particles bound within the circle around the center of the canvas.

### Collisions
- **Elastic Collisions**: On collision, the particles interacting will bounce off each other as in an elastic collision.
- **Fluid Mode**: Particles will move more fluidly. All interactions and separations will be distance-based softened.

### Performance Warnings
- The simulator does give warnings if the number of particles being used is approaching, or has exceeded a number at which system performance will probably be significantly degraded. If running a very large number of particles, pay attention to system performance.

## Requirements

- **Browser**: Purely web-based. Should run seemlessly on all modern browsers including Chrome, Firefox, Safari, Edge.
- **Device**: Optimised for use on desktops, tablets and mobiles.

Installation

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

The following are major things that one would find in the code:

### `index.html`
Currently the entire simulator is written into one file, but I am working on splitting the files and making an API.

Main HTML file setting up canvas as well as all sliders or other input controls used in this demonstration

### `script.js`

**The file hasn't been added yet, but in the future I am planning to split the code into different files.**
Further on, most important parts of your JavaScript code, hence responsible for taking care of your Simulation functionalities, those will encompass:

 **Particle Class** describing what one particle can perform-move, draw and Collision
 **Simulation Functions** Spawn, Check collision, and application of any Force and animation.
**UI Elements**: Particle settings modification on input, shape type, number count, gravity behaviour etc.
Css
`styles.css`
**The file hasn't been added yet, but in the future I am planning to split the code into different files.**
CSS file which gives style to ui elements, ranging from the canvas to all of the control panel.
## Ui
User Interface
**Particle Setting Panel**: Users has the ability to change the shape type of particle, the number, size, size of the particles.
- **Canvas Area**: Where the particles should be seen living.
- **Control Panel**: Gives facility for the user to change some of the parameters of simulation such as interaction mode, gravity and container shape.
  
### Hot Keys
- **Shape**: Select form the shape the particles will have: Circle, square, hexagon
- **Count**: Selecciona how much are in the number of the particle that is going on the simulation.
- **Max Size**: Although the sizes will still be random, the maximum will be increased to your setting value. P.S the default is 10px.
- **Gravity**: ON/OFF gravity.
- **Mode**: The mode of interaction - pull or push.
- **Container Shape**: The container can be either rectangular or circular in shape.
- **Coloring**: Single color, random color, velocity based or collision based.
- **Spawn Particles**: Sending out new particles based on the above settings.

## Performance Considerations

The simulation is set to a default of 256 particles(a power of two), and I can reasonably say that a particle count on a 9th IPAD ~ 1090.
The simulator of a Particle is supporting up to hundreds or thousands of them. Note, however, that much large ones do lower performance curve, specially on low range devices or browser, The tool is going to warn you if it gets too many of these particles, however, it will still be better that you experiment and apply within reasonable limit for optimal execution of performance. 

## Troubleshooting

- **Simulation Lag**: If simulation is running slow, decrease the number of particles, or disable effects like Color by Velocity.
- **Particles Gravity**: To activate gravity either use the prebuilt checkbox or force it own in the code!
- **Collision Mode Not Behaving Correctly**: Particle intersections are not ubgs! Particles need to be overlapping in order to detect the collision. This is so performance can be kept reasonable!

## Future Improvements

- **More Physics Models**: Include more physics models, such as for elasticity and drag among others that are complicated.
- **Better UI**: Intuitive UI - comfort for users. E.g. Presets for typical sets ups/ configurations.
- **Particle Trails**: Allow the user to see the trajectories of particles so the experience is more dynamic.

## License

This project is open source and released under the [MIT License](LICENSE).

---
**Go and have fun playing with the particles! Peace out!**
