# Random Name Generator - Setup & Installation

**Version:** 1.0.0

---

## About

Random Name Generator is a lightweight Python utility that generates random full names using customizable text files.

It uses keyboard shortcuts to generate male or female names instantly, displaying the results directly in the command prompt.

## Features

- Random male full name generation.
- Random female full name generation.
- Customizable first and last name lists.
- Instant name generation using keyboard shortcuts.
- Console-based output.
- Automatically loads names from external text files.

## Requirements

The following software is required:

- Python 3
- Python `keyboard` library
- Windows (recommended)

## Installation

### Step 1 - Install Python

Download and install Python 3 from:

https://www.python.org/downloads/

During installation on Windows, make sure to enable:

- Add Python to PATH

To verify Python is installed, open Command Prompt and enter:

```bash
python --version
```

### Step 2 - Install Dependencies

Open Command Prompt and run:

```bash
python -m pip install keyboard
```

This installs the keyboard library required for detecting key presses.

### Step 3 - Download the Project

Download or clone the Random Name Generator repository from GitHub.

If downloading through GitHub:

1. Open the project repository.
2. Select the green Code button.
3. Select Download ZIP.
4. Extract the downloaded ZIP file.
5. Locate the Python script.

## Name List Configuration

The generator requires three separate text files:

| File | Purpose |
|---|---|
| Male First Names | Contains male first names. |
| Female First Names | Contains female first names. |
| Last Names | Contains last names used for both categories. |

### Editing File Paths

Open the Python script in a text editor.

Locate the FILE PATHS section near the beginning:

```python
MALE_FIRST_NAMES_FILE = r"C:\EXAMPLE\PATH\TO\FILE.txt"
FEMALE_FIRST_NAMES_FILE = r"C:\EXAMPLE\PATH\TO\FILE.txt"
LAST_NAMES_FILE = r"C:\EXAMPLE\PATH\TO\FILE.txt"
```

Replace each example path with the actual location of your text files.

For example:

```python
MALE_FIRST_NAMES_FILE = r"C:\RandomNameGenerator\Names\male_first_names.txt"
FEMALE_FIRST_NAMES_FILE = r"C:\RandomNameGenerator\Names\female_first_names.txt"
LAST_NAMES_FILE = r"C:\RandomNameGenerator\Names\last_names.txt"
```

### Formatting Name Lists

Each text file should contain one name per line.

Example:

```text
John
Michael
David
James
Robert
```

Blank lines are automatically ignored.

**Important:** All three text files must exist at their configured locations before starting the generator.

## Running the Generator

Open Command Prompt in the project folder.

Run:

```bash
python random_name_generator.py
```

Replace the filename if your Python script uses a different name.

Once launched, the generator will display its available keyboard controls.

## Keyboard Controls

| Key | Action |
|---|---|
| M | Generate a random male name. |
| F | Generate a random female name. |
| ESC | Exit the generator. |

Generated names are printed directly into the Command Prompt window.

## How Name Generation Works

The generator independently selects:

1. A random first name from the selected gender's name list.
2. A random last name from the shared last-name list.
3. Combines both selections into a full name.

For example:

```text
=== RANDOM NAME GENERATOR ===
Press M = Male Name
Press F = Female Name
Press ESC = Exit

John Smith
Emily Johnson
Michael Brown
```

Names can repeat because selections are completely random.

## Troubleshooting

### Problem: Python is not recognized.

**Solution:**

Make sure Python is installed and added to your system PATH.

### Problem: No module named 'keyboard'.

**Solution:**

Run:

```bash
python -m pip install keyboard
```

### Problem: FileNotFoundError.

**Solution:**

Check the three configured file paths and make sure all name-list files exist.

### Problem: Permission or keyboard access errors.

**Solution:**

Try running Command Prompt as Administrator.

The keyboard library may require elevated permissions depending on the system and how keyboard input is being detected.

### Problem: No names are generated.

**Solution:**

Make sure your text files contain valid names, with one name per line, and that the configured paths point to the correct files.

## Project Structure

A recommended folder arrangement:

```text
Random-Name-Generator/
│
├── random_name_generator.py
├── README.md
├── SETUP.md
├── LICENSE
│
└── Names/
    ├── male_first_names.txt
    ├── female_first_names.txt
    └── last_names.txt
```

## Additional Notes

- Names are selected randomly from the provided text files.
- First and last names are selected independently.
- Duplicate name generations are possible.
- The generator does not require an internet connection.
- Name lists can be customized by editing the text files.
- Keyboard detection may require administrator privileges on some systems.

## License

This project is distributed under the MIT License.

See the included LICENSE file for details.

---

**Enjoy generating random names!**
