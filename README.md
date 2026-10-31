# ⚛️ Interactive Bloch Sphere Simulator

A standalone 3D quantum state simulator that runs directly in the browser without any installation or external dependencies. This project was created as the 2nd homework assignment for the **Quantum Informatics Applications** course[cite: 5].

## 📌 Features
* **Custom Initial State:** Can be defined using polar (θ) and azimuthal (φ) angles in radians[cite: 5].
* **Quantum Gates:** Supports fundamental single-qubit Pauli, Hadamard, and phase gates (X, Y, Z, H, S, T), as well as parameterized rotation gates (Rx, Ry, Rz) with arbitrary angles[cite: 5].
* **Circuit Builder (Pipeline):** Selected gates can be chained together and applied as a sequence to the current quantum state with a single click[cite: 5].
* **Simultaneous Multi-State Visualization:** The simulator can display multiple individually color-coded state vectors on the Bloch sphere at the same time[cite: 5].
* **Custom 3D Rendering Engine:** Purely HTML5 Canvas-based, utilizing custom 3D projection and camera rotation logic, oriented according to quantum physics conventions (vertical Y-axis).

## 🚀 Running the Simulator (Standalone)
**No web server, framework, or external packages are required** to run the program (e.g., it works perfectly without Node.js or Three.js). 

1. Download or clone the repository.
2. Double-click the `bloch_szimulator.html` file and open it in any modern web browser (Chrome, Firefox, Safari, Edge)[cite: 5].

## 🎮 Controls & Usage
* **3D Camera Movement:** Left-click and drag on the sphere area to rotate the Bloch sphere in 3D space.
* **Zoom In/Out:** Use the mouse wheel to zoom in and out.
* **State Management:** You can add new initial states or delete previous ones on the left panel. The gate sequence (right panel) is always applied to the most recently created state, generating a new state vector in space as the result.

## 🛠 Tech Stack
* **HTML5 & CSS3:** Modern, dark-themed UI (built with CSS variables, Grid, and Flexbox layouts).
* **Vanilla JavaScript (ES6+):** The program logic is purely native JS. Quantum mechanical calculations (complex multiplications, unitary matrix operations) are handled by a custom, lightweight `Complex` class.
* **HTML5 Canvas API:** A custom trigonometric projection system built into the 2D canvas context is responsible for the 3D spatial experience.

---
*Developed within the Computer Engineering program at the Budapest University of Technology and Economics (BME VIK).*
