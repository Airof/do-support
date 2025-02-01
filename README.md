# do-support

## Overview
This is a very simple extension that provides **code snippets** and **syntax highlighting** for **ModelSim DO files** in Visual Studio Code.

## Features
- Syntax highlighting for DO files
- Snippets for commonly used ModelSim commands
- Supports keywords, filenames, numbers, and comments

## Installation
### Manual Installation
1. Download the `.vsix` file from the repository root.
2. Open **VS Code**.
3. Open the **Extensions** tab (`Ctrl+Shift+X`).
4. Click on the **three dots (⋮)** in the top-right corner.
5. Select **Install from VSIX...**.
6. Choose the downloaded `.vsix` file.

## Usage
### Syntax Highlighting
This extension highlights keywords, filenames, numbers, and comments in DO files.

### Snippets
Type a command (e.g., `vsim`) and press **Tab** to expand it.

## Example
```do
vcom ALU/FullAdder.vhd
vsim work.FullAdder
add wave *

force a 0 0ns, 1 10ns -repeat 20
force b 0ns 0, 1 20ns -repeat 40
force cin 0 0, 1 40 -repeat 80

run 80;
```

## Optional Use
If you are working on **VHDL projects in ModelSim** or want to try this extension, you have the option. You might also find it useful for projects like **[Mano-Machine](https://github.com/Airof/Mano-Machine)**.

## Contributing
Feel free to submit issues and pull requests to improve this extension!

## License
MIT

