Interactive Bloch Sphere Visualizer 🌐
An intuitive, web-based 3D visualization tool for learning the fundamentals of single-qubit quantum gates. This project provides a hands-on experience, allowing users to apply quantum gates and instantly see their effect on a qubit's state vector.

This project was created as a submission for the CQhack25 Hackathon.

Live Demo »
(Replace the link above with your actual GitHub Pages URL after deploying!)

✨ Features
Full 3D Interaction: Rotate, pan, and zoom the Bloch Sphere with your mouse to view the state vector from any angle.

Real-time Gate Application: Click buttons to apply common quantum gates (X, Y, Z, H, S, T) and watch the state vector animate to its new position instantly.

Live State Vector Display: The precise mathematical state of the qubit (α and β complex coefficients) is always visible and updates with every gate operation.

Intuitive Labels: Key states like |0⟩, |1⟩, |+⟩, |-⟩, etc., are clearly labeled on the sphere for easy reference.

Responsive Design: The visualizer works smoothly on both desktop and mobile browsers.

Zero Installation: Runs entirely in the browser with no setup required.

🚀 How to Use
Open the Live Demo link.

Rotate the Sphere: Click and drag your mouse on the sphere to rotate the camera.

Apply Gates: Use the control panel on the right to click on a gate button (e.g., H).

Observe: Watch the red arrow (the state vector) move to its new position.

Reset: Click the Reset to |0⟩ button at any time to return the qubit to its ground state.

🛠️ Technologies Used
Three.js: A powerful 3D graphics library for creating and rendering the scene in WebGL.

HTML5 & CSS3: For the core structure and modern styling.

Tailwind CSS: For rapidly building the user interface and control panels.

JavaScript (ES6 Modules): For all the application logic, including the quantum state calculations and user interactions.

🔬 How It Works
The application simulates the behavior of a single qubit without connecting to actual quantum hardware.

State Representation: The qubit's state is stored internally as a state vector with two complex numbers, [α, β]. The initial state is |0⟩, which corresponds to α=1 and β=0.

Gate Application: Each quantum gate is represented by a 2x2 matrix. When a user clicks a gate button, the application performs a matrix-vector multiplication of the gate's matrix with the current state vector.

Visualization: The resulting α and β values are converted from the state vector representation to spherical coordinates (θ, φ). These coordinates are then used to determine the direction of the red arrow on the 3D sphere, providing a direct visual representation of the qubit's abstract mathematical state.

🔮 Future Ideas
Quantum Circuit Builder: Allow users to drag-and-drop gates into a sequence and run the entire circuit.

Measurement Simulation: Add a "Measure" button that collapses the state vector to either |0⟩ or |1⟩ based on the probabilities (|α|² and |β|²).

More Gates: Include multi-qubit gates (like CNOT) and visualizations for entangled states.

Custom Gate Input: Allow users to input their own 2x2 unitary matrices to see what they do.

📄 License
This project is open-source and available under the MIT License.
