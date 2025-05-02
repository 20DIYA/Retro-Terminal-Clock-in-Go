# Terminal Digital Clock in Go

This is a simple terminal-based digital clock written in Go. It displays the current time in a large 7-segment style using ANSI escape codes to clear and update the terminal every second.

## Features

- Displays the current system time in **HH:MM:SS** format.
- Uses Unicode block characters to mimic a digital clock.
- Blinking colon every two seconds.
- Refreshes the terminal screen using ANSI escape sequences (no external packages required).

## Requirements

- Go 1.13 or later
- A terminal that supports ANSI escape sequences (Linux, macOS, Windows Terminal, etc.)
