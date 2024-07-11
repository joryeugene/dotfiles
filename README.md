# PyCharm IdeaVim Configuration

This repository contains my personal IdeaVim configuration for PyCharm, enhancing the IDE with Vim-like capabilities and custom keybindings for improved productivity.

## Table of Contents

1. [Features](#features)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Key Mappings](#key-mappings)
5. [Workflow Tips](#workflow-tips)
6. [Customization](#customization)
7. [Troubleshooting](#troubleshooting)

## Features

- Vim-like editing capabilities in PyCharm
- Custom keybindings for common PyCharm actions
- Integration with PyCharm-specific features
- AceJump integration for quick navigation
- Enhanced refactoring and code navigation shortcuts
- Distraction-free coding mode

## Prerequisites

- PyCharm (Community or Professional edition)
- IdeaVim plugin installed in PyCharm

## Installation

1. Clone this repository:

2. Create a symbolic link to the `.ideavimrc` file:

   - On macOS/Linux:
     ```
     ln -s /path/to/pycharm-ideavim-config/.ideavimrc ~/.ideavimrc
     ```
   - On Windows (run in Command Prompt as Administrator):
     ```
     mklink /H %USERPROFILE%\.ideavimrc \path\to\pycharm-ideavim-config\.ideavimrc
     ```

3. Restart PyCharm or reload the `.ideavimrc` file within PyCharm.

## Key Mappings

### Navigation

- `<leader>e` - AceJump (find character)
- `<leader>w` - AceJump (word mode)
- `<C-o>` - Navigate back
- `<C-i>` - Navigate forward
- `H` - Move to beginning of line
- `L` - Move to end of line

### IDE Actions

- `<leader>ru` - Run
- `<leader>de` - Debug
- `<leader>b` - Toggle breakpoint
- `<leader>gd` - Go to declaration
- `<leader>gi` - Go to implementation
- `<leader>fu` - Find usages
- `<leader>rn` - Rename element
- `<leader>ff` - Go to file
- `<leader>fc` - Go to class
- `<leader>fs` - Go to symbol
- `<leader>o` - File structure popup

### Editing

- `<leader>/` - Comment/uncomment line
- `<leader>l` - Reformat code
- `J` (visual mode) - Move selected lines down
- `K` (visual mode) - Move selected lines up
- `U` - Redo

### Windows and Tabs

- `<leader>q` - Close current tab
- `<leader>qa` - Close all tabs
- `<leader>qo` - Close other tabs
- `<leader>1-9` - Go to tab 1-9
- `<leader>]` - Next tab
- `<leader>[` - Previous tab
- `<leader>sv` - Split vertically
- `<leader>sh` - Split horizontally
- `<C-h/j/k/l>` - Navigate splits

### Other

- `<leader>z` - Toggle distraction-free mode
- `jk` - Escape (insert mode)
- `<S-Space>` - Go to next error
- `<leader>se` - Search everywhere
- `<leader>a` - Find action
- `<leader>t` - Activate terminal
- `<leader>r` - Recent files
- `<leader>fp` - Find in path
- `<leader>p` - Toggle project view
- `<leader>rf` - Quick refactoring menu
- `<leader>i` - Show intention actions
- `<leader>nf` - Create new file
- `<leader>nd` - Create new directory
- `<leader>ro` - Reopen closed tab
- `<leader>sw` - Toggle soft wrap
- `K` - Quick documentation
- `<leader>qi` - Quick implementation
- `<leader>su` - Show usages
- `<leader>oi` - Optimize imports

## Workflow Tips

1. **Quick Navigation**: Use AceJump (`<leader>e` or `<leader>w`) for rapid movement within a file.

2. **Efficient Refactoring**: Utilize `<leader>rn` for renaming and `<leader>rf` for quick access to refactoring options.

3. **Seamless Debugging**: Set breakpoints with `<leader>b` and start debugging with `<leader>de`.

4. **Code Exploration**: Use `<leader>gd` for go to definition, `<leader>fu` for find usages, and `K` for quick documentation.

5. **Distraction-Free Coding**: Toggle distraction-free mode with `<leader>z` when you need to focus.

6. **Multi-File Editing**: Use tab navigation (`<leader>1-9`, `<leader>]`, `<leader>[`) and split windows (`<leader>sv`, `<leader>sh`) for efficient multi-file workflows.

## Customization

To customize this configuration:

1. Open the `.ideavimrc` file in PyCharm.
2. Modify existing mappings or add new ones based on your preferences.
3. Save the file and reload it in PyCharm (`:source ~/.ideavimrc`) or restart PyCharm.

## Troubleshooting

If you encounter any issues:

1. Ensure the IdeaVim plugin is installed and enabled in PyCharm.
2. Check if your PyCharm version is compatible with the IdeaVim plugin.
3. Verify that the `.ideavimrc` file is correctly linked and located in your home directory.
4. Try reloading the `.ideavimrc` file using `:source ~/.ideavimrc` in PyCharm.
5. If a specific keybinding isn't working, check for conflicts in PyCharm's keymap settings.

For more help, refer to the [IdeaVim plugin documentation](https://github.com/JetBrains/ideavim) or open an issue in this repository.


