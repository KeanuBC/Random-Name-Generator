# Random Name Generator v1.0.0

## Overview
A simple Python utility that generates random full names using customizable text files containing first and last names.

The generator uses keyboard shortcuts to quickly generate either male or female names without needing to interact with a menu.

## Features
- **Male Name Generation:** Generates random male full names.
- **Female Name Generation:** Generates random female full names.
- **Custom Name Lists:** Uses separate text files for male first names, female first names, and last names.
- **Keyboard Shortcuts:** Generate names instantly using M and F.
- **Simple Operation:** Runs in the background and prints generated names directly to the console.

## Controls
- **M:** Generate a random male name.
- **F:** Generate a random female name.
- **ESC:** Exit the generator.

## Requirements
- Python 3
- keyboard Python library

## Configuration
Before running the script, edit the three file paths at the top of the Python script:

- `MALE_FIRST_NAMES_FILE`
- `FEMALE_FIRST_NAMES_FILE`
- `LAST_NAMES_FILE`

Each text file should contain one name per line.

## Notes
- Generated names are selected randomly from the provided text files.
- First names and last names are selected independently.
- Names can repeat between generations.
- The keyboard library may require administrator privileges on some systems.

## License
Distributed under the MIT License.
