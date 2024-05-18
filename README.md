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
[[https://lambertk.academic.wlu.edu/breezypythongui/installing-breezingpythongui/|BreezyPythonGUI Website]]

3. Run the application:
    ```bash
    python lampify.py
    ```

## Usage

- **Randomize**: Populate the grid with a random configuration of lit and unlit bulbs.
- **Auto Run**: Start the automatic evolution of the grid.
- **Run Step**: Advance the grid evolution by one step.
- **Stop**: Halt the automatic evolution.
- **Reset**: Clear the grid and reset the generation counter.
- **Save**: Save the current grid configuration to a text file.
- **Open**: Load a grid configuration from a text file.

## Classes and Methods

### Lamp

- `__init__(self, state=False)`: Initialize the lamp with an off state.
- `toggle_state(self)`: Toggle the state of the lamp.
- `get_state(self)`: Return the current state of the lamp.

### GridLogic

- `__init__(self, row=50, col=50)`: Initialize a grid of lamps.
- `get_neighbours(self, i, j)`: Count the number of lit neighboring bulbs.
- `update_cell_state(self, row, col)`: Determine the next state of a bulb based on its neighbors.
- `next_gen(self)`: Advance the grid to the next generation.
- `randomize(self)`: Randomly set the state of each bulb in the grid.
- `save_to_text(self)`: Save the grid configuration to a text file.
- `load_from_text(self)`: Load a grid configuration from a text file.
- `get_grid(self)`: Print the grid to the terminal (for debugging).

### GridCanvas

- `__init__(self, parent, cell_size=10, rows=50, cols=50)`: Initialize the canvas and draw the grid.
- `draw_grid(self)`: Draw the grid on the canvas.
- `update_grid(self)`: Update the canvas display based on the grid state.
- `evolvi(self)`: Evolve the grid over time.
- `SaveFile(self)`: Save the grid configuration to a file.
- `OpenFile(self)`: Load a grid configuration from a file.
- `autorun(self)`: Start automatic evolution.
- `runstep(self)`: Evolve the grid by one step.
- `stop(self)`: Stop the automatic evolution.
- `reset(self)`: Reset the grid and counters.
- `randomizer(self)`: Randomize the grid.
- `mousePressed(self, event)`: Handle mouse press events.
- `mouseReleased(self, event)`: Handle mouse release events.
- `mouseDragged(self, event)`: Handle mouse drag events.

### Lampify

- `__init__(self, cell_size=10, rowc=50, colc=50)`: Initialize the main GUI window.
- `create_widgets(self)`: Create and place widgets on the GUI.
- `update_generation_label(self)`: Update the generation counter label.
- `update_path_label(self)`: Update the file path label when a file is opened.
- `update_savefile_label(self)`: Update the file path label when a file is saved.
- `shortener(self, string)`: Shorten a file path for display.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please read the [CONTRIBUTING](CONTRIBUTING.md) file for guidelines on how to contribute.

---

This repository is a simple and interactive way to explore the principles of cellular automata and grid-based simulations. Enjoy experimenting with Lampify!
