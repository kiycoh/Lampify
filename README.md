# Lampify

## Overview

Lampify is a computer science UNI project: an interactive simulation application inspired by cellular automata, particularly Conway's Game of Life. It features a grid of lamps that evolve over time based on simple rules. This project is built using Python's BreezyPythonGUI and tkinter libraries to provide a graphical user interface for visualization and interaction.

## Features

- **Lamp Class**: Represents individual bulbs with a toggleable state.
- **GridLogic Class**: Manages the grid of bulbs, including rules for evolution, state updates, randomization, and file operations (save/load).
- **GridCanvas Class**: Handles the graphical representation of the bulb grid, including interactions via mouse events.
- **Lampify Class**: Sets up the GUI, incorporating buttons and labels for user interaction, including controls for running the simulation, saving/loading grids, and resetting the grid.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/lampify.git
    cd lampify
    ```

2. Install the required libraries:
https://lambertk.academic.wlu.edu/breezypythongui/installing-breezingpythongui

3. Run the application:
    ```bash
    python lampify.py
    ```

## Usage
![LampifyV2 4](https://github.com/kiycoh/Lampify/assets/152720918/047e96dc-2990-42c7-af53-5f5d3ac36ca1)

- **Randomize**: Populate the grid with a random configuration of lit and unlit bulbs.
- **Auto Run**: Start the automatic evolution of the grid.
- **Run Step**: Advance the grid evolution by one step.
- **Stop**: Halt the automatic evolution.
- **Reset**: Clear the grid and reset the generation counter.
- **Save**: Save the current grid configuration to a text file.
- **Open**: Load a grid configuration from a text file.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute.

---

This repository is a simple and interactive way to explore the principles of cellular automata and grid-based simulations. Enjoy experimenting with Lampify!
