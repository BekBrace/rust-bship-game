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

```sh
git clone https://github.com/yourusername/battleship-rust.git
cd battleship-rust
cargo build
cargo run
```
