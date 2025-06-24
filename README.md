3D Pendulum Simulation
This project presents a simple 3D pendulum simulation using Three.js for rendering and GSAP for animation.

Table of Contents
Features

Installation

Usage

Project Structure

Dependencies

Contributing

License

Features
3D Rendering: Utilizes Three.js to create a 3D environment for the pendulum.

Pendulum Animation: Demonstrates a series of pendulums swinging with a subtle delay between each, powered by GSAP.

Camera Controls: Allows user interaction to orbit and pan the camera using OrbitControls.

Responsive Design: Adapts to different screen sizes.

Shadows: Implements shadows for a more realistic scene.

Installation
To set up and run this project locally, follow these steps:

Clone the repository:

git clone <(https://github.com/alizamir25/3D-Pendulum)>
cd 3d-pendulum-simulation

Note: If you downloaded the files directly, simply navigate to the project directory.

Ensure you have a local web server:
You can use a simple Python HTTP server or any other web server you prefer.
For Python 3:

python -m http.server

For Python 2:

python -m SimpleHTTPServer

Open in your browser:
After starting the server, open your web browser and navigate to http://localhost:8000 (or the address provided by your server).

Usage
Once the page loads, you will see a series of pendulums swinging.

Orbit Camera: Click and drag with your mouse to rotate around the scene.

Pan Camera: Right-click and drag (or use two fingers on a trackpad) to pan the camera.

Project Structure
index.html: The main HTML file that sets up the canvas and loads the necessary JavaScript and CSS files.

style.css: Contains basic styling for the HTML elements, primarily resetting margin and ensuring the canvas is a block element.

three.js: (This file contains the core JavaScript logic for the 3D simulation)

Initializes the Three.js renderer, scene, and camera.

Sets up lights and shadows.

Configures OrbitControls for camera interaction.

Creates multiple pendulum-like objects (a ball and a "hair" representing the string).

Uses GSAP to animate the swinging motion of each pendulum with staggered delays.

Includes a plane at the bottom to receive shadows.

Manages the animation loop and handles window resizing.

Dependencies
This project relies on the following external libraries, which are loaded via CDN in index.html:

Three.js: A JavaScript 3D library that makes it easier to display 3D content on a webpage. (You've referenced three.js locally, but typically for Three.js projects, it's either bundled or loaded from a CDN like https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js).

OrbitControls: A Three.js addon for camera control.

GSAP (GreenSock Animation Platform): A robust JavaScript animation library used here for the pendulum's swinging motion. (The provided three.js code uses gsap.fromTo but it's not explicitly loaded in index.html. You would typically include it like <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.9.1/gsap.min.js"></script>).

Contributing
If you'd like to contribute to this project, please feel free to:

Fork the repository.

Create a new branch (git checkout -b feature/your-feature).

Make your changes.

Commit your changes (git commit -am 'Add new feature').

Push to the branch (git push origin feature/your-feature).

Create a new Pull Request.

License
This project is open source and available under the MIT License.
