# PyCharm IdeaVim Configuration

This repository contains my personal IdeaVim configuration for PyCharm, enhancing the IDE with Vim-like capabilities and custom keybindings for improved productivity.

## Features

- Vim-like editing capabilities in PyCharm
- Custom keybindings for common PyCharm actions
- Integration with PyCharm-specific features
- NERDTree for file navigation
- Enhanced refactoring and code navigation shortcuts

## Prerequisites

- PyCharm (Community or Professional edition)
- IdeaVim plugin installed in PyCharm

## Installation

1. Clone this repository:

2. Create a symbolic link to the `.ideavimrc` file:
- On macOS/Linux:
  ```
  ln -s /path/to/dotfiles/.ideavimrc ~/.ideavimrc
  ```
- On Windows (run in Command Prompt as Administrator):
  ```
  mklink /H %USERPROFILE%\.ideavimrc \path\to\dotfiles\.ideavimrc
  ```

3. Restart PyCharm or reload the `.ideavimrc` file within PyCharm.

## Key Mappings

### Navigation

- `<C-o>` - Navigate back
- `<C-i>` - Navigate forward
- `H` - Move to beginning of line
- `L` - Move to end of line
- `<leader>e` - Recent files
- `<leader>gc` - Go to class
- `<leader>gd` - Go to declaration
- `<leader>ge` - Go to next error
- `<leader>gf` - Go to file
- `<leader>gi` - Go to implementation
- `<leader>gp` - Go to previous error
- `<leader>gs` - Go to symbol
- `<leader>gt` - Go to test
- `<leader>gu` - Show usages

### IDE Actions

- `<leader>ru` - Run
- `<leader>de` - Debug
- `<leader>st` - Stop
- `<leader>tb` - Toggle breakpoint
- `<leader>df` - Toggle distraction-free mode
- `<leader>fa` - Go to action
- `<leader>fc` - Reformat code
- `<leader>ff` - Find in path
- `<leader>hw` - Hide all windows (non-code panels)
- `<leader>me` - Maximize editor in split
- `<leader>oi` - Optimize imports
- `<leader>pi` - Parameter info
- `<leader>pm` - Toggle presentation mode
- `<leader>rr` - Replace in path
- `<leader>sd` - Show error description
- `<leader>se` - Search everywhere
- `<leader>si` - Show intention actions

### Editing

- `<leader>/` - Comment/uncomment line
- `J` (visual mode) - Move selected lines down
- `K` (visual mode) - Move selected lines up
- `U` - Redo

### Windows and Tabs

- `<leader>qa` - Close all editors
- `<leader>qo` - Close all editors but active
- `<leader>qp` - Close project
- `<leader>qt` - Close active tab
- `<leader>qx` - Close content
- `<leader>1-9` - Go to tab 1-9
- `<leader>]` - Next tab
- `<leader>[` - Previous tab
- `<leader>sc` - Unsplit
- `<leader>sh` - Split horizontally
- `<leader>sm` - Move editor to opposite tab group
- `<leader>sv` - Split vertically
- `<leader>sw` - Toggle soft wraps
- `<C-h/j/k/l>` - Navigate splits

### Tool Windows

- `<leader>td` - Activate debug tool window
- `<leader>tp` / `<leader>pt` - Activate project tool window
- `<leader>tr` - Activate run tool window
- `<leader>ts` - Activate structure tool window
- `<leader>tt` - Activate terminal tool window

### Other

- `<leader>w` - Save all
- `<leader>ve` - Edit .ideavimrc
- `<leader>vr` - Reload .ideavimrc
- `<leader>vv` - Version control quick list
- `jk` - Escape (insert mode)
- `K` - Quick documentation
- `<leader>nf` - New file
- `<leader>nd` - New directory

### Refactoring

- `<leader>re` - Refactoring quick list
- `<leader>rf` - Introduce field
- `<leader>ri` - Inline
- `<leader>rm` - Extract method
- `<leader>rn` - Rename element
- `<leader>rp` - Introduce parameter
- `<leader>rv` - Introduce variable

### Plugins

- NERDTree: Use for file navigation (see NERDTree section for mappings)
- Exchange: Use `cx{motion}` to mark and exchange text
- Surround: Use `ys`, `cs`, and `ds` for surrounding operations
- Commentary: Use `gc` for commenting operations
- Which-Key: Provides a popup menu of available keybindings

## NERDTree Mappings

- `o` - Open files, directories and bookmarks
- `go` - Open selected file, but leave cursor in the NERDTree
- `t` - Open selected node/bookmark in a new tab
- `T` - Same as 't' but keep the focus on the current tab
- `i` - Open selected file in a split window
- `gi` - Same as i, but leave the cursor on the NERDTree
- `s` - Open selected file in a new vsplit
- `gs` - Same as s, but leave the cursor on the NERDTree
- `O` - Recursively open the selected directory
- `x` - Close the current nodes parent
- `X` - Recursively close all children of the current node
- `P` - Jump to the root node
- `p` - Jump to current nodes parent
- `K` - Jump up inside directories at the current tree depth
- `J` - Jump down inside directories at the current tree depth
- `<C-J>` - Jump down to next sibling of the current directory
- `<C-K>` - Jump up to previous sibling of the current directory
- `r` - Recursively refresh the current directory
- `R` - Recursively refresh the current root
- `m` - Display the NERDTree menu
- `q` - Close the NERDTree window
- `A` - Zoom (maximize/minimize) the NERDTree window

## Customization

To customize this configuration:

1. Open the `.ideavimrc` file in PyCharm (leader ve).
2. Modify existing mappings or add new ones based on your preferences.
3. Save the file and reload it in PyCharm (`:source ~/.ideavimrc`) or restart PyCharm (leader vr).

## Troubleshooting

If you encounter any issues:

1. Ensure the IdeaVim plugin is installed and enabled in PyCharm.
2. Check if your PyCharm version is compatible with the IdeaVim plugin.
3. Verify that the `.ideavimrc` file is correctly linked and located in your home directory.
4. Try reloading the `.ideavimrc` file using `:source ~/.ideavimrc` in PyCharm.
5. If a specific keybinding isn't working, check for conflicts in PyCharm's keymap settings or overloaded <leader> key bindings.

For more help, refer to the [IdeaVim plugin documentation](https://github.com/JetBrains/ideavim) or open an issue in this repository.
