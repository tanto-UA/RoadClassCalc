# BS EN 13201 Road Lighting Class Calculator

A modern, highly interactive, and visually stunning single-page web application designed to calculate the recommended road lighting class based on the BS EN 13201 standard. 

This tool provides lighting engineers and designers with a responsive interface to determine appropriate lighting classes (M, C, or P) by evaluating weighting values ($V_{WS}$) based on various road characteristics.

## ✨ Features

- **Premium UI & Theme Support**: A beautiful glassmorphic interface with a toggleable Dark/Light mode, designed for clarity and visual appeal.
- **Dynamic 2D Canvas Visualizer**: An interactive, real-time visual simulation of the lighting scene:
  - **Motorised Traffic (M)**: Perspective view of a highway with street lamps casting light pools. Reflects changes in road separation, parked vehicles, and ambient luminance.
  - **Conflict Area (C)**: Intersection scene with zebra crossings, traffic lights, and overlapping floodlights.
  - **Pedestrian Pathway (P)**: Suburban walkway simulation with walkers, trees, and glowing facial recognition indicators.
- **Interactive Requirement Specs**: Dynamically generates the photometric requirements (e.g., $L_{avg}$, $U_o$, $TI$, $E_{avg}$) based on the calculated class. Click on any metric to view an educational modal with vector diagrams and engineering context.
- **Seamless Export (Obsidian Ready)**: Easily copy or download a beautifully formatted Markdown report of your calculation results, perfectly suited for documentation or Obsidian vaults.
- **Zero Dependencies**: Built with pure HTML5, CSS3, and Vanilla JavaScript. Everything is contained within a single file.

## 🚀 Usage

Since the application is self-contained without external dependencies, getting started is extremely simple:

1. Clone or download the repository.
2. Open the `Road Class Calc.html` file in any modern web browser (Chrome, Edge, Firefox, Safari).

If hosted on GitHub Pages, simply navigate to the provided URL to use the calculator instantly.

## 🧮 How it Works

The calculator implements the methodology outlined in BS EN 13201:
1. **Select Area Type**: Choose between Motorised Traffic (M), Conflict Area (C), or Pedestrian/Low Speed (P).
2. **Set Parameters**: Adjust the characteristics of the road (speed, traffic volume, junction density, etc.). Each parameter applies a specific Weighting Value ($V_W$).
3. **Calculate**: The tool sums the weights ($V_{WS}$) and applies the standard formula `Class = 6 - V_{WS}` (with appropriate boundary clamping) to determine the final recommended lighting class.
4. **Review Targets**: The application provides the exact photometric targets your lighting design must achieve to meet the determined class.

## 🛠️ Built With

- **HTML5** & **CSS3** (CSS Variables, Grid, Flexbox, Glassmorphism)
- **Vanilla JavaScript** (ES6+)
- **HTML5 Canvas API** (For real-time 2D rendering)
- Google Fonts (`Inter` and `Outfit`)

## 📄 License

This project is open-source and available for use and modification.
