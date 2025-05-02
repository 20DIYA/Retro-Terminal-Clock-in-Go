# Retro Terminal Clock

This is a simple retro-style terminal clock written in Go. The clock is displayed in ASCII art, showing the current time in a digital format using block-style characters. It updates every second and works in the terminal/console environment.

## Features

- Displays the current time in a retro digital clock format using ASCII art.
- The clock updates every second.
- The colon between hours, minutes, and seconds blinks every second for a retro effect.
- The clock is entirely terminal-based and requires no external dependencies.

## Screenshots

![Retro Terminal Clock](./screenshot.png)

## Installation

To run the Retro Terminal Clock, you'll need to have Go installed on your system.

1. Install [Go](https://golang.org/dl/), if you haven't already.
2. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/retro-terminal-clock.git
    cd retro-terminal-clock
    ```

3. Build the project:

    ```bash
    go build
    ```

4. Run the project:

    ```bash
    ./retro-terminal-clock
    ```

## Code Explanation

### `clearScreen` function:
Clears the terminal screen using ANSI escape codes.

### `moveCursorTopLeft` function:
Moves the cursor to the top-left corner of the terminal screen using ANSI escape codes.

### `main` function:
- It initializes placeholders for each digit (`0` to `9`) and a colon (`:`) in ASCII art.
- The clock is updated every second with the current time.
- The current hour, minute, and second are split into tens and ones digits, which are used to display the time on the terminal.
- The colon blinks every second for a retro effect.
  
### Time Representation:
Each digit and the colon is represented using a 5x3 matrix of characters. For example, the number `8` is represented as:

