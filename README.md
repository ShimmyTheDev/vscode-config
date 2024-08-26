# VSCode Settings
### ... and keybindings made for productivity
A VSCode config using Vim motions, based on MelkeyDev's [vscode_bindings](https://github.com/Melkeydev/vscode_bindings) with a few personal adjustments.

## Installation
### Linux
##### Backup current settings and keybindings (optional)
```bash
cp ~/.config/Code/User/settings.json ~/.config/Code/User/settings.json.bak
cp ~/.config/Code/User/keybindings.json ~/.config/Code/User/keybindings.json.bak
```

##### Clone the repository and remove unnecessary files
```bash
rm ~/.config/Code/User/settings.json ~/.config/Code/User/keybindings.json
git clone https://github.com/ShimmyTheDev/vscode-config.git ~/.config/Code/User
rm ~/.config/Code/User/README.md ~/.config/Code/User/LICENSE
```
---
### MacOS: 
##### Backup current settings and keybindings (optional)
```bash
cp ~/Library/Application\ Support/Code/User/settings.json ~/Library/Application\ Support/Code/User/settings.json.bak
cp ~/Library/Application\ Support/Code/User/keybindings.json ~/Library/Application\ Support/Code/User/keybindings.json.bak
```
##### Clone the repository and remove unnecessary files
```bash
rm ~/Library/Application\ Support/Code/User/settings.json ~/Library/Application\ Support/Code/User/keybindings.json
git clone https://github.com/ShimmyTheDev/vscode-config.git ~/Library/Application\ Support/Code/User
rm ~/Library/Application\ Support/Code/User/README.md ~/Library/Application\ Support/Code/User/LICENSE
```
---
### Windows (Command prompt): 
##### Backup current settings and keybindings (optional)
```ps
copy "%APPDATA%\Code\User\settings.json" "%APPDATA%\Code\User\settings.json.bak"
copy "%APPDATA%\Code\User\keybindings.json" "%APPDATA%\Code\User\keybindings.json.bak"
```
##### Clone the repository and remove unnecessary files
```ps
git clone https://github.com/ShimmyTheDev/vscode-config.git %APPDATA%\Code\User\
del "%APPDATA%\Code\User\README.md" "%APPDATA%\Code\User\LICENSE"
```
---
# User Settings

- **Format on Save** (`editor.formatOnSave`): Automatically formats the code when you save a file.

- **Suggest Insert Mode** (`editor.suggest.insertMode`): Replaces the text with the selected suggestion from IntelliSense instead of just inserting it.

- **Terminal Font Family** (`terminal.integrated.fontFamily`): Specifies the font family for the integrated terminal as "FiraCode Nerd Font".

- **Linked Editing** (`editor.linkedEditing`): Enables linked editing of HTML and XML tags, where typing a tag name automatically updates the matching closing tag.

- **Update Imports on File Move** (`javascript.updateImportsOnFileMove.enabled`): Automatically updates import paths when a JavaScript or TypeScript file is moved or renamed.

- **Zoom Level** (`window.zoomLevel`): Adjusts the overall zoom level of the editor's interface to 1.5.

- **Launch Configuration** (`launch`): Placeholder for launch configurations, currently empty.

- **JSON Settings** (`[json]`): Placeholder for JSON-specific settings, currently empty.

- **Minimap** (`editor.minimap.enabled`): Disables the minimap, the small overview of the code on the right side of the editor.

- **Breadcrumbs** (`breadcrumbs.enabled`): Disables breadcrumbs, the navigation aid at the top of the editor that shows the file path.

- **Icon Theme** (`workbench.iconTheme`): Sets the icon theme to "material-icon-theme".

- **Show Release Notes** (`update.showReleaseNotes`): Disables the automatic display of release notes after updating.

- **Zen Mode Line Numbers** (`zenMode.hideLineNumbers`): Keeps line numbers visible even in Zen Mode.

- **Vim: Use System Clipboard** (`vim.useSystemClipboard`): Enables using the system clipboard with Vim commands.

- **Vim: Leader Key** (`vim.leader`): Sets the Vim leader key to the spacebar.

- **Vim: Highlight Search** (`vim.hlsearch`): Highlights search results when using Vim search.

### Vim Normal Mode Keybindings

- **Switch Buffers** (`<S-h>`, `<S-l>`): `Shift + H` switches to the previous buffer; `Shift + L` switches to the next buffer.

- **Splits** (`leader + v`, `leader + s`): `Leader + v` opens a vertical split; `Leader + s` opens a horizontal split.

- **Pane Navigation** (`leader + h/j/k/l`): `Leader + h/j/k/l` navigates to the left, down, up, and right panes, respectively.

- **File Management** (`leader + w/q/x`): `Leader + w` saves the current file; `Leader + q` quits; `Leader + x` saves and quits.

- **Markers Navigation** (`[d`, `]d`): `[d` jumps to the previous marker; `]d` jumps to the next marker.

- **Quick Fix and Format** (`leader + c/a`, `leader + f/p`): `Leader + c + a` opens quick fixes; `Leader + f` opens Quick Open; `Leader + p` formats the document.

- **Preview Definition** (`g + h`): `g + h` shows a hover with the definition of the symbol under the cursor.

### Vim Visual Mode Keybindings

- **Indentation** (`<`, `>`): `<` outdents and `>` indents selected lines while staying in visual mode.

- **Move Lines** (`J`, `K`): `J` moves selected lines down; `K` moves them up.

- **Toggle Comment** (`leader + c`): `Leader + c` toggles comments for the selected lines.

### Go

- **Auto Update Go Tools** (`go.toolsManagement.autoUpdate`): Automatically updates Go tools as needed.

### Workbench Settings

- **Activity Bar Location** (`workbench.activityBar.location`): Hides the activity bar on the left side of the window.

- **Color Theme** (`workbench.colorTheme`): Sets the color theme to "One Dark Pro Darker".

- **Editor Font Family** (`editor.fontFamily`): Sets the editor's font family to "FiraCode Nerd Font".


# Keybindings

## Navigation

| Keybinding            | Description |
|-----------------------|-------------|
| `Ctrl + P`            | Opens the Quick Open dialog to quickly navigate between files. |
| `Ctrl + Shift + A`    | Switches focus to the next terminal instance when a terminal is active. |
| `Ctrl + Shift + B`    | Switches focus to the previous terminal instance when a terminal is active. |
| `Ctrl + Shift + J`    | Toggles the visibility of the bottom panel (e.g., terminal, problems, output). |
| `Ctrl + Shift + N`    | Creates a new terminal instance when a terminal is active. |
| `Ctrl + Shift + W`    | Closes the active terminal instance when a terminal is focused. |

## File Tree

| Keybinding            | Description |
|-----------------------|-------------|
| `Ctrl + E`            | Opens the file explorer when the sidebar is hidden. |
| `Ctrl + E`            | Focuses the file explorer when the sidebar is visible but the explorer is not focused. |
| `Ctrl + E`            | Focuses the file explorer when it’s open but not focused. |
| `Ctrl + E`            | Closes the sidebar when the file explorer is focused. |
| `N`                   | Creates a new file in the file explorer when it is focused, and no input field is active. |
| `R`                   | Renames the selected file in the file explorer when it is focused, and no input field is active. |
| `Shift + N`           | Creates a new folder in the file explorer when it is focused. |
| `D`                   | Deletes the selected file in the file explorer when it is focused, and no input field is active. |

## Extra

| Keybinding            | Description |
|-----------------------|-------------|
| `Ctrl + Shift + 5`    | Matches the corresponding opening or closing tag in the editor (Emmet command). |
| `Ctrl + Z`            | Toggles Zen Mode, which hides the activity bar, status bar, and sidebars for a distraction-free coding environment. |

---
**NOTE**

MacOS users may want to review their default bindings and update them accordingly due to different role of CMD and Ctrl buttons in OSX systems

---