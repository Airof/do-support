# do-support

## Overview

This is a very simple extension that provides code snippets and syntax highlighting for ModelSim DO files in Visual Studio Code.

## Features

- Syntax highlighting for DO files
- Snippets for commonly used ModelSim commands
- Supports keywords, filenames, numbers, and comments

## Installation

### Manual Installation

1. Download the `.vsix` file from the repository root.
   - [Download do-support-0.0.1.vsix](https://github.com/Airof/do-support/blob/master/do-support-0.0.1.vsix)
2. Open **VS Code**.
3. Open the **Extensions** tab (`Ctrl+Shift+X`).
4. Click on the **three dots (⋮)** in the top-right corner.
5. Select **Install from VSIX...**.
6. Choose the downloaded `.vsix` file.

### Ensure `.do` Files Use the Correct Language Mode
By default, VS Code treats `.do` files as **Tcl**, but your extension should recognize them as **DO files**. To check and fix this:

1. **Open a `.do` file** in VS Code.
2. Look at the **bottom-right corner** where the language mode is displayed.
   - If it says `Tcl`, VS Code still thinks it's a Tcl file.
   - If it says `DO`, then your extension is working correctly.
3. **If it's still Tcl**, manually switch it:
   - Click the language name (`Tcl`).
   - Search for `do` and select it.
   - VS Code should remember this setting for future `.do` files.
4. To make this change permanent, update your `settings.json`:

   ```json
   "files.associations": {
       "*.do": "do"
   }
   ```

## Optional Use

If you are working on **VHDL projects in ModelSim** or want to try this extension, you have the option. You might also find it useful for projects like **[Mano-Machine](https://github.com/Airof/Mano-Machine)**.

## Contributing

Feel free to submit issues and pull requests to improve this extension!

## License

MIT

