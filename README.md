# Kilo Editor

Kilo is a small, simple, and efficient text editor written in C. Inspired by the original [kilo](https://github.com/antirez/kilo) created by Salvatore Sanfilippo (antirez), this project has been expanded and modified to include additional features like syntax highlighting, modal editing, and more.

## Features

- **Syntax Highlighting**: Supports C/C++, Python, JavaScript, and HTML.
- **Modal Editing**: Similar to Vim, with normal, insert, and command modes.
- **Configurable Settings**: Customize tab stops, quit times, and other options via a configuration file (`.kilorc`).
- **Basic Text Editing Functions**: Insert, delete, and search text within the editor.
- **Line Numbers**: Displayed on the left side for easy navigation.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/BrianBeilby/text-editor.git
   cd kilo-editor
   ```
2. Compile the editor
   ```bash
   make
   ```
3. Run the editor
   ```bash
   ./kilo <filename>
   ```

## Usage
### Normal Mode
- `i`: Enter insert mode
- `:`: Enter command mode
- `/`: Enter search mode
- `h`: Move cursor left
- `j`: Move cursor down
- `k`: Move cursor up
- `l`: Move cursor right
- `x`: Delete character under the cursor
- `Ctrl+Q`: Quit the editor
- `Ctrl+S`: Save the current file

### Insert Mode
- Type text as you would in any editor
- `Esc`: Return to normal mode
- `Enter`: Insert newline
- `Backspace`: Delete character before the cursor

### Command Mode
- `:w`: Save the file
- `:q`: Quit the editor
- `:wq`: Save the file and quit the editor

### Search Mode
- `/pattern`: Search for `pattern` in the text

### Configuration

You can create a `.kilorc` file in the home directory to customize the editor's settings. Here is an example configuration file:

```plaintext
KILO_TAB_STOP=4
KILO_QUIT_TIMES=3
KILO_STATUS_MSG_TIMEOUT=5
KILO_SHOW_LINE_NUMBERS=1
KILO_WRAP_LINES=1
KILO_USE_SPACES_FOR_INDENT=1
KILO_HIGHLIGHT_SEARCH_MATCHES=1
```

## Credits

This project is based on the following resources:
- The original [kilo](https://github.com/antirez/kilo) editor by Salvatore Sanfilippo ([antirez](https://github.com/antirez)).
- This [tutorial](https://viewsourcecode.org/snaptoken/kilo/index.html) by [snaptoken](https://github.com/snaptoken), which provided detailed guidance and examples.
