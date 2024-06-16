# Battleship Game in Rust

This is a simple implementation of the classic Battleship game in Rust, showcasing the use of Rust's standard library for I/O handling and random number generation. The game features a player and an opponent, each with their own game board, and allows for basic gameplay including placing ships, firing at the opponent's board, and checking for game over conditions.

## Table of Contents

- [Battleship Game in Rust](#battleship-game-in-rust)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Installation](#installation)
  - [Usage](#usage)
  - [Game Rules](#game-rules)
  - [File Structure](#file-structure)
  - [Methods](#methods)
    - [`Board`](#board)
    - [`main`](#main)
    - [`get_player_input`](#get_player_input)
    - [`generate_opponent_move`](#generate_opponent_move)
  - [Contributing](#contributing)
  - [License](#license)

## Features

- Random ship placement ensuring no overlap or out-of-bounds positioning.
- Basic user input for firing at coordinates.
- Display of game boards with different symbols for hits, misses, and ships.
- Simple game loop with turn-based gameplay.
- Detection of game over conditions.

## Installation

1. Ensure you have Rust installed. If not, download and install it from [rust-lang.org](https://www.rust-lang.org/tools/install).
2. Clone this repository:
## Game Rules

- Each player has a 10x10 board.
- Ships of different sizes (5, 4, 3, 3, 2) are placed randomly on the board.
- Players take turns firing at each other's board by entering coordinates.
- A hit is marked with a red dot (●) and a miss with a blue dot (·).
- The game continues until all ships of one player are sunk.

## File Structure

- `main.rs`: Contains the main game logic and functions.
- `Cargo.toml`: Project configuration file.

## Methods

### `Board`

- `new() -> Self`: Initializes a new game board with all cells empty.
- `place_ship(&mut self, size: usize)`: Randomly places a ship of the given size on the board.
- `can_place_ship(&self, row: usize, col: usize, size: usize, direction: bool) -> bool`: Checks if a ship can be placed at the specified location.
- `fire(&mut self, row: usize, col: usize) -> CellState`: Fires at the specified cell, updating its state.
- `display(&self, hide_ships: bool)`: Displays the game board, optionally hiding the ships.
- `is_game_over(&self) -> bool`: Checks if all ships have been hit.

### `main`

- Initializes player and opponent boards.
- Places ships on both boards.
- Handles the game loop, including player and opponent turns and checking for game over conditions.

### `get_player_input`

- Prompts the player for input coordinates.
- Validates and returns the coordinates.

### `generate_opponent_move`

- Generates random coordinates for the opponent's move.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or additions.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

```sh
git clone https://github.com/yourusername/battleship-rust.git
cd battleship-rust
cargo build
cargo run
```
