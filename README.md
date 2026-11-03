# Random Name Generator

A lightweight Python random name generator that creates full names using customizable name lists.

Generate male or female names instantly using simple keyboard shortcuts.

## Features

- Random male full name generation.
- Random female full name generation.
- Customizable first and last name lists.
- Instant generation using keyboard shortcuts.
- Simple console-based interface.

## Requirements

- Python 3
- `keyboard` library

## Installation

Install the required Python dependency:

```bash
python -m pip install keyboard
```

Download or clone this repository and open the Python script.

## Configuration

Before running, configure the file paths at the top of the script:

```python
MALE_FIRST_NAMES_FILE = r"C:\PATH\TO\MALE_NAMES.txt"
FEMALE_FIRST_NAMES_FILE = r"C:\PATH\TO\FEMALE_NAMES.txt"
LAST_NAMES_FILE = r"C:\PATH\TO\LAST_NAMES.txt"
```

Each text file should contain one name per line.

### Example name list

```text
John
Michael
David
James
Robert
```

## Usage

Run the script:

```bash
python random_name_generator.py
```

### Keyboard Controls

| Key | Action |
|---|---|
| M | Generate a male name |
| F | Generate a female name |
| ESC | Exit the generator |

## Additional Notes

- Names are randomly selected from the provided text files.
- First names and last names are selected independently.
- Duplicate name generations are possible.
- Some systems may require administrator privileges for global keyboard detection.

## License

This project is licensed under the [MIT License](LICENSE).
