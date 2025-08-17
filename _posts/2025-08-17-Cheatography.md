---
title: "🎮 Personal Keybindings Cheat Sheet"
date: 2025-08-17
permalink: /posts/2025/cheatography/
tags:
  - keybindings
  - shortcuts
  - configuration
  - cheat-sheet
excerpt: "A comprehensive cheat sheet for keybindings across Gnome, WezTerm, and Neovim"
---

<!-- markdownlint-disable MD033 -->

# 🎮 Personal Keybindings Cheat Sheet

A comprehensive reference for all my customized keyboard shortcuts across different applications.

> 📝 **Legend**:
>
> - <kbd>SUPER</kbd> = Windows/Cmd key
> - <kbd>LEADER</kbd> = Leader key sequence
> - Actions marked with 🔧 are custom configurations

## 🖥️ Gnome Desktop Environment

> **Key Reference**: <kbd>SUPER</kbd> = <kbd>Win</kbd> key

### 🚀 Application Launchers

| Shortcut                                        | Action                | Description             |
| ----------------------------------------------- | --------------------- | ----------------------- |
| <kbd>SUPER</kbd> + <kbd>B</kbd>                 | Launch Browser        | Opens Chrome 🔧         |
| <kbd>SUPER</kbd> + <kbd>F</kbd>                 | Launch File Manager   | Opens Nautilus 🔧       |
| <kbd>SUPER</kbd> + <kbd>T</kbd>                 | Launch Terminal       | Opens WezTerm 🔧        |
| <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>S</kbd> | Launch System Monitor | Opens Mission Center 🔧 |

### 🧭 Navigation & Windows

#### Window Management

| Shortcut                          | Action             | Description                     |
| --------------------------------- | ------------------ | ------------------------------- |
| <kbd>SUPER</kbd> + <kbd>M</kbd>   | Toggle All Windows | Show/hide all normal windows 🔧 |
| <kbd>SUPER</kbd> + <kbd>Q</kbd>   | Close Window       | Close the focused window 🔧     |
| <kbd>SUPER</kbd> + <kbd>H</kbd>   | Hide Window        | Hide the focused window 🔧      |
| <kbd>SUPER</kbd> + <kbd>F11</kbd> | Maximize Toggle    | Toggle window maximization 🔧   |
| <kbd>F11</kbd>                    | Fullscreen Toggle  | Toggle fullscreen mode 🔧       |

#### Workspace Management

| Shortcut                                             | Action             | Description                          |
| ---------------------------------------------------- | ------------------ | ------------------------------------ |
| <kbd>SUPER</kbd> + <kbd>]</kbd>                      | Next Workspace     | Switch to workspace on the right 🔧  |
| <kbd>SUPER</kbd> + <kbd>[</kbd>                      | Previous Workspace | Switch to workspace on the left 🔧   |
| <kbd>SUPER</kbd> + <kbd>1-4</kbd>                    | Go to Workspace    | Switch to specific workspace 🔧      |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>]</kbd>   | Move Window Right  | Move window to next workspace 🔧     |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>[</kbd>   | Move Window Left   | Move window to previous workspace 🔧 |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>1-4</kbd> | Move to Workspace  | Move window to specific workspace 🔧 |

#### Application & Window Switching

| Shortcut                                          | Action               | Description                             |
| ------------------------------------------------- | -------------------- | --------------------------------------- |
| <kbd>SUPER</kbd> + <kbd>TAB</kbd>                 | Switch Applications  | Cycle between applications 🔧           |
| <kbd>SUPER</kbd> + <kbd>`</kbd>                   | Switch App Windows   | Switch windows within an application 🔧 |
| <kbd>ALT</kbd> + <kbd>F6</kbd>                    | Direct Window Switch | Switch windows of an app directly 🔧    |
| <kbd>ALT</kbd> + <kbd>ESC</kbd>                   | Direct Window Switch | Switch windows directly 🔧              |
| <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>TAB</kbd> | System Controls      | Switch between system controls 🔧       |

#### Multi-Monitor Support

| Shortcut                                                    | Action             | Description                      |
| ----------------------------------------------------------- | ------------------ | -------------------------------- |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>DownArrow</kbd>  | Move Down Monitor  | Move window one monitor down 🔧  |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>UpArrow</kbd>    | Move Up Monitor    | Move window one monitor up 🔧    |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>LeftArrow</kbd>  | Move Left Monitor  | Move window one monitor left 🔧  |
| <kbd>SHIFT</kbd> + <kbd>SUPER</kbd> + <kbd>RightArrow</kbd> | Move Right Monitor | Move window one monitor right 🔧 |

### 📸 Screenshots & Recording

| Shortcut                                                           | Action        | Description                     |
| ------------------------------------------------------------------ | ------------- | ------------------------------- |
| <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>SHIFT</kbd> + <kbd>R</kbd> | Record Screen | Interactive screen recording 🔧 |
| <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>A</kbd>                    | Screenshot    | Interactive screenshot tool 🔧  |

### 🔐 System Controls

| Shortcut                                          | Action           | Description              |
| ------------------------------------------------- | ---------------- | ------------------------ |
| <kbd>SUPER</kbd> + <kbd>L</kbd>                   | Lock Screen      | Lock the screen 🔧       |
| <kbd>CTRL</kbd> + <kbd>ALT</kbd> + <kbd>DEL</kbd> | Log Out          | Log out of session 🔧    |
| <kbd>SUPER</kbd> + <kbd>A</kbd>                   | All Applications | Show all applications 🔧 |
| <kbd>SUPER</kbd> + <kbd>SPACE</kbd>               | Switch Input     | Switch input method 🔧   |

### 🪟 Window Tiling

| Shortcut                                         | Action     | Description                  |
| ------------------------------------------------ | ---------- | ---------------------------- |
| <kbd>SUPER</kbd> + <kbd>RightArrow</kbd>         | Tile Right | Move window to right tile 🔧 |
| <kbd>SUPER</kbd> + <kbd>LeftArrow</kbd>          | Tile Left  | Move window to left tile 🔧  |
| <kbd>SUPER</kbd> + <kbd>UpArrow</kbd>            | Tile Up    | Move window to tile above 🔧 |
| <kbd>SUPER</kbd> + <kbd>DownArrow</kbd>          | Tile Down  | Move window to tile below 🔧 |
| <kbd>ALT</kbd> + <kbd>SUPER</kbd> + <kbd>D</kbd> | Span Right | Span window to right tile 🔧 |
| <kbd>ALT</kbd> + <kbd>SUPER</kbd> + <kbd>A</kbd> | Span Left  | Span window to left tile 🔧  |
| <kbd>ALT</kbd> + <kbd>SUPER</kbd> + <kbd>W</kbd> | Span Up    | Span window above 🔧         |
| <kbd>ALT</kbd> + <kbd>SUPER</kbd> + <kbd>S</kbd> | Span Down  | Span window below 🔧         |
| <kbd>SUPER</kbd> + <kbd>C</kbd>                  | Untile     | Remove window from tile 🔧   |

#### Window Menu

| Shortcut                          | Action      | Description                       |
| --------------------------------- | ----------- | --------------------------------- |
| <kbd>ALT</kbd> + <kbd>SPACE</kbd> | Window Menu | Activate focused window's menu 🔧 |

---

## 💻 WezTerm Terminal

> **Key References**:
>
> - <kbd>SUPER</kbd> = <kbd>ALT</kbd>
> - <kbd>SUPER_REV</kbd> = <kbd>ALT</kbd> + <kbd>CTRL</kbd>
> - <kbd>LEADER</kbd> = <kbd>SUPER_REV</kbd> + <kbd>SPACE</kbd>

### 🔧 Function Keys & Utilities

| Shortcut                            | Action             | Description                     |
| ----------------------------------- | ------------------ | ------------------------------- |
| <kbd>F1</kbd>                       | Copy Mode          | Activate copy mode              |
| <kbd>F2</kbd>                       | Command Palette    | Open command palette            |
| <kbd>F3</kbd>                       | Launcher           | Show launcher                   |
| <kbd>F4</kbd>                       | Tab Launcher       | Show launcher (tabs only)       |
| <kbd>F5</kbd>                       | Workspace Launcher | Show launcher (workspaces only) |
| <kbd>F11</kbd>                      | Fullscreen         | Toggle fullscreen               |
| <kbd>F12</kbd>                      | Debug Overlay      | Show debug overlay              |
| <kbd>SUPER</kbd> + <kbd>f</kbd>     | Search Text        | Search in terminal              |
| <kbd>SUPER_REV</kbd> + <kbd>u</kbd> | Open URL           | Open URL under cursor           |

### 📋 Copy & Paste

| Shortcut                                          | Action | Description          |
| ------------------------------------------------- | ------ | -------------------- |
| <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>c</kbd> | Copy   | Copy to clipboard    |
| <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>v</kbd> | Paste  | Paste from clipboard |

### ⌨️ Cursor Movement

| Shortcut                                 | Action     | Description               |
| ---------------------------------------- | ---------- | ------------------------- |
| <kbd>SUPER</kbd> + <kbd>LeftArrow</kbd>  | Line Start | Move cursor to line start |
| <kbd>SUPER</kbd> + <kbd>RightArrow</kbd> | Line End   | Move cursor to line end   |
| <kbd>SUPER</kbd> + <kbd>Backspace</kbd>  | Clear Line | Clear entire line         |

### 📑 Tab Management

#### Tab Creation & Destruction

| Shortcut                            | Action    | Description                |
| ----------------------------------- | --------- | -------------------------- |
| <kbd>SUPER</kbd> + <kbd>t</kbd>     | New Tab   | Spawn tab (default domain) |
| <kbd>SUPER_REV</kbd> + <kbd>f</kbd> | WSL Tab   | Spawn tab (WSL Ubuntu)     |
| <kbd>SUPER</kbd> + <kbd>x</kbd>     | Close Tab | Close current tab          |

#### Tab Navigation

| Shortcut                            | Action         | Description              |
| ----------------------------------- | -------------- | ------------------------ |
| <kbd>SUPER</kbd> + <kbd>[</kbd>     | Next Tab       | Navigate to next tab     |
| <kbd>SUPER</kbd> + <kbd>]</kbd>     | Previous Tab   | Navigate to previous tab |
| <kbd>SUPER_REV</kbd> + <kbd>[</kbd> | Move Tab Left  | Move current tab left    |
| <kbd>SUPER_REV</kbd> + <kbd>]</kbd> | Move Tab Right | Move current tab right   |

#### Tab Appearance

| Shortcut                            | Action         | Description        |
| ----------------------------------- | -------------- | ------------------ |
| <kbd>SUPER</kbd> + <kbd>9</kbd>     | Toggle Tab Bar | Show/hide tab bar  |
| <kbd>SUPER</kbd> + <kbd>0</kbd>     | Rename Tab     | Rename current tab |
| <kbd>SUPER_REV</kbd> + <kbd>0</kbd> | Undo Rename    | Undo tab rename    |

### 🪟 Window Management

| Shortcut                        | Action        | Description          |
| ------------------------------- | ------------- | -------------------- |
| <kbd>SUPER</kbd> + <kbd>n</kbd> | New Window    | Spawn new window     |
| <kbd>SUPER</kbd> + <kbd>=</kbd> | Increase Size | Increase window size |
| <kbd>SUPER</kbd> + <kbd>-</kbd> | Decrease Size | Decrease window size |

### 🔲 Pane Management

#### Pane Creation & Layout

| Shortcut                             | Action           | Description             |
| ------------------------------------ | ---------------- | ----------------------- |
| <kbd>SUPER</kbd> + <kbd>\\</kbd>     | Split Vertical   | Split pane vertically   |
| <kbd>SUPER_REV</kbd> + <kbd>\\</kbd> | Split Horizontal | Split pane horizontally |
| <kbd>SUPER</kbd> + <kbd>Enter</kbd>  | Zoom Pane        | Toggle pane zoom state  |
| <kbd>SUPER</kbd> + <kbd>w</kbd>      | Close Pane       | Close current pane      |

#### Pane Navigation

| Shortcut                            | Action     | Description             |
| ----------------------------------- | ---------- | ----------------------- |
| <kbd>SUPER_REV</kbd> + <kbd>K</kbd> | Move Up    | Navigate to pane above  |
| <kbd>SUPER_REV</kbd> + <kbd>J</kbd> | Move Down  | Navigate to pane below  |
| <kbd>SUPER_REV</kbd> + <kbd>H</kbd> | Move Left  | Navigate to left pane   |
| <kbd>SUPER_REV</kbd> + <kbd>L</kbd> | Move Right | Navigate to right pane  |
| <kbd>SUPER_REV</kbd> + <kbd>P</kbd> | Swap Pane  | Swap with selected pane |

#### Pane Scrolling

| Shortcut                        | Action      | Description          |
| ------------------------------- | ----------- | -------------------- |
| <kbd>SUPER</kbd> + <kbd>u</kbd> | Scroll Up   | Scroll 5 lines up    |
| <kbd>SUPER</kbd> + <kbd>d</kbd> | Scroll Down | Scroll 5 lines down  |
| <kbd>PageUp</kbd>               | Page Up     | Scroll one page up   |
| <kbd>PageDown</kbd>             | Page Down   | Scroll one page down |

### 🎨 Background Images

| Shortcut                            | Action         | Description              |
| ----------------------------------- | -------------- | ------------------------ |
| <kbd>SUPER</kbd> + <kbd>/</kbd>     | Random Image   | Select random background |
| <kbd>SUPER</kbd> + <kbd>,</kbd>     | Next Image     | Cycle to next image      |
| <kbd>SUPER</kbd> + <kbd>.</kbd>     | Previous Image | Cycle to previous image  |
| <kbd>SUPER_REV</kbd> + <kbd>/</kbd> | Fuzzy Select   | Fuzzy select image       |
| <kbd>SUPER</kbd> + <kbd>b</kbd>     | Focus Mode     | Toggle background focus  |

### 🎛️ Key Tables (Leader-based)

#### Font Resize Mode

| Sequence                         | Action              | Description            |
| -------------------------------- | ------------------- | ---------------------- |
| <kbd>LEADER</kbd> + <kbd>f</kbd> | **Enter Font Mode** | Enter font resize mode |
| <kbd>k</kbd>                     | Increase Font       | Increase font size     |
| <kbd>j</kbd>                     | Decrease Font       | Decrease font size     |
| <kbd>r</kbd>                     | Reset Font          | Reset to default size  |
| <kbd>q</kbd> / <kbd>Esc</kbd>    | Exit Mode           | Exit font resize mode  |

#### Pane Resize Mode

| Sequence                         | Action              | Description            |
| -------------------------------- | ------------------- | ---------------------- |
| <kbd>LEADER</kbd> + <kbd>p</kbd> | **Enter Pane Mode** | Enter pane resize mode |
| <kbd>k</kbd>                     | Resize Up           | Adjust pane size up    |
| <kbd>j</kbd>                     | Resize Down         | Adjust pane size down  |
| <kbd>h</kbd>                     | Resize Left         | Adjust pane size left  |
| <kbd>l</kbd>                     | Resize Right        | Adjust pane size right |
| <kbd>q</kbd> / <kbd>Esc</kbd>    | Exit Mode           | Exit pane resize mode  |

---

## ⚡ Neovim Editor

> **Key Reference**: <kbd>LEADER</kbd> = Custom leader key (typically <kbd>,</kbd> or <kbd>SPACE</kbd>)

### 🚀 Essential Navigation

| Shortcut                          | Action           | Description                |
| --------------------------------- | ---------------- | -------------------------- |
| <kbd>j</kbd><kbd>k</kbd>          | Normal Mode      | Exit insert mode 🔧        |
| <kbd>LEADER</kbd> + <kbd>nh</kbd> | Clear Highlights | Clear search highlights 🔧 |
| <kbd>v</kbd> then <kbd>q</kbd>    | Exit Visual      | Exit visual mode 🔧        |

### 🔢 Number Operations

| Shortcut                         | Action    | Description                      |
| -------------------------------- | --------- | -------------------------------- |
| <kbd>LEADER</kbd> + <kbd>+</kbd> | Increment | Increment number under cursor 🔧 |
| <kbd>LEADER</kbd> + <kbd>-</kbd> | Decrement | Decrement number under cursor 🔧 |

### 🪟 Window Management

#### Split Management

| Shortcut                          | Action           | Description                  |
| --------------------------------- | ---------------- | ---------------------------- |
| <kbd>LEADER</kbd> + <kbd>sv</kbd> | Vertical Split   | Split window vertically 🔧   |
| <kbd>LEADER</kbd> + <kbd>sh</kbd> | Horizontal Split | Split window horizontally 🔧 |
| <kbd>LEADER</kbd> + <kbd>se</kbd> | Equal Splits     | Make splits equal size 🔧    |
| <kbd>LEADER</kbd> + <kbd>sx</kbd> | Close Split      | Close current split 🔧       |

#### Tab Management

| Shortcut                          | Action        | Description                       |
| --------------------------------- | ------------- | --------------------------------- |
| <kbd>LEADER</kbd> + <kbd>to</kbd> | New Tab       | Open new tab 🔧                   |
| <kbd>LEADER</kbd> + <kbd>tx</kbd> | Close Tab     | Close current tab 🔧              |
| <kbd>LEADER</kbd> + <kbd>tn</kbd> | Next Tab      | Go to next tab 🔧                 |
| <kbd>LEADER</kbd> + <kbd>tp</kbd> | Previous Tab  | Go to previous tab 🔧             |
| <kbd>LEADER</kbd> + <kbd>tf</kbd> | Buffer to Tab | Open current buffer in new tab 🔧 |

### 🖥️ Terminal Integration

| Shortcut                          | Action          | Description                            |
| --------------------------------- | --------------- | -------------------------------------- |
| <kbd>LEADER</kbd> + <kbd>ts</kbd> | Split Terminal  | Open terminal in split window 🔧       |
| <kbd>LEADER</kbd> + <kbd>tn</kbd> | Terminal Normal | Switch terminal to normal mode 🔧      |
| <kbd>LEADER</kbd> + <kbd>tx</kbd> | Close Terminal  | Close terminal (from terminal mode) 🔧 |

### 💾 Session Management

| Shortcut                          | Action          | Description                              |
| --------------------------------- | --------------- | ---------------------------------------- |
| <kbd>LEADER</kbd> + <kbd>wr</kbd> | Restore Session | Restore session for current directory 🔧 |
| <kbd>LEADER</kbd> + <kbd>ws</kbd> | Save Session    | Save workspace session 🔧                |

### 📄 Buffer Navigation

| Shortcut                            | Action            | Description                      |
| ----------------------------------- | ----------------- | -------------------------------- |
| <kbd>LEADER</kbd> + <kbd>bn</kbd>   | Next Buffer       | Navigate to next buffer 🔧       |
| <kbd>LEADER</kbd> + <kbd>bp</kbd>   | Previous Buffer   | Navigate to previous buffer 🔧   |
| <kbd>LEADER</kbd> + <kbd>bx</kbd>   | Close Buffer      | Close current buffer 🔧          |
| <kbd>LEADER</kbd> + <kbd>b1-9</kbd> | Go to Buffer      | Jump to specific buffer (1-9) 🔧 |
| <kbd>LEADER</kbd> + <kbd><</kbd>    | Move Buffer Left  | Move buffer position left 🔧     |
| <kbd>LEADER</kbd> + <kbd>></kbd>    | Move Buffer Right | Move buffer position right 🔧    |

### 🤖 AI & Copilot

| Shortcut                          | Action            | Description                  |
| --------------------------------- | ----------------- | ---------------------------- |
| <kbd>LEADER</kbd> + <kbd>ce</kbd> | Enable Copilot    | Enable GitHub Copilot 🔧     |
| <kbd>LEADER</kbd> + <kbd>cd</kbd> | Disable Copilot   | Disable GitHub Copilot 🔧    |
| <kbd>CTRL</kbd> + <kbd>O</kbd>    | Accept Suggestion | Accept Copilot suggestion 🔧 |

### 🎨 Formatting & Linting

| Shortcut                          | Action       | Description                    |
| --------------------------------- | ------------ | ------------------------------ |
| <kbd>LEADER</kbd> + <kbd>mp</kbd> | Format Code  | Format current buffer 🔧       |
| <kbd>LEADER</kbd> + <kbd>l</kbd>  | Trigger Lint | Run linting on current file 🔧 |

### 🔍 LSP (Language Server Protocol)

#### Navigation

| Shortcut      | Action          | Description                            |
| ------------- | --------------- | -------------------------------------- |
| <kbd>gR</kbd> | References      | Show LSP references via Telescope 🔧   |
| <kbd>gd</kbd> | Definition      | Go to definition via Telescope 🔧      |
| <kbd>gD</kbd> | Declaration     | Go to declaration 🔧                   |
| <kbd>gi</kbd> | Implementation  | Show implementations via Telescope 🔧  |
| <kbd>gt</kbd> | Type Definition | Show type definitions via Telescope 🔧 |

#### Actions & Information

| Shortcut                          | Action              | Description                    |
| --------------------------------- | ------------------- | ------------------------------ |
| <kbd>LEADER</kbd> + <kbd>ca</kbd> | Code Actions        | Show available code actions 🔧 |
| <kbd>LEADER</kbd> + <kbd>rn</kbd> | Rename              | Smart rename symbol 🔧         |
| <kbd>K</kbd>                      | Hover Documentation | Show hover documentation 🔧    |

#### Diagnostics

| Shortcut                         | Action              | Description                          |
| -------------------------------- | ------------------- | ------------------------------------ |
| <kbd>LEADER</kbd> + <kbd>D</kbd> | File Diagnostics    | Show diagnostics for current file 🔧 |
| <kbd>LEADER</kbd> + <kbd>d</kbd> | Line Diagnostics    | Show diagnostics for current line 🔧 |
| <kbd>[</kbd><kbd>d</kbd>         | Previous Diagnostic | Jump to previous diagnostic 🔧       |
| <kbd>]</kbd><kbd>d</kbd>         | Next Diagnostic     | Jump to next diagnostic 🔧           |

#### LSP Controls

| Shortcut                          | Action             | Description                   |
| --------------------------------- | ------------------ | ----------------------------- |
| <kbd>LEADER</kbd> + <kbd>rs</kbd> | Restart LSP        | Restart LSP server 🔧         |
| <kbd>LEADER</kbd> + <kbd>dh</kbd> | Toggle Hints       | Toggle inlay hints 🔧         |
| <kbd>LEADER</kbd> + <kbd>dd</kbd> | Toggle Diagnostics | Toggle diagnostics display 🔧 |

### 📁 File Explorer (NvimTree)

| Shortcut                          | Action            | Description                        |
| --------------------------------- | ----------------- | ---------------------------------- |
| <kbd>LEADER</kbd> + <kbd>ee</kbd> | Toggle Explorer   | Toggle file explorer 🔧            |
| <kbd>LEADER</kbd> + <kbd>ef</kbd> | Find in Explorer  | Toggle explorer on current file 🔧 |
| <kbd>LEADER</kbd> + <kbd>ec</kbd> | Collapse Explorer | Collapse file explorer 🔧          |
| <kbd>LEADER</kbd> + <kbd>er</kbd> | Refresh Explorer  | Refresh file explorer 🔧           |

### 🔄 Text Substitution

| Shortcut                   | Action            | Description                       |
| -------------------------- | ----------------- | --------------------------------- |
| <kbd>s</kbd>               | Substitute Motion | Substitute with motion 🔧         |
| <kbd>ss</kbd>              | Substitute Line   | Substitute entire line 🔧         |
| <kbd>S</kbd>               | Substitute to EOL | Substitute to end of line 🔧      |
| <kbd>s</kbd> (visual mode) | Visual Substitute | Substitute in visual selection 🔧 |

### 🔭 Telescope (Fuzzy Finder)

| Shortcut                          | Action       | Description                              |
| --------------------------------- | ------------ | ---------------------------------------- |
| <kbd>LEADER</kbd> + <kbd>ff</kbd> | Find Files   | Fuzzy find files in current directory 🔧 |
| <kbd>LEADER</kbd> + <kbd>fr</kbd> | Recent Files | Fuzzy find recent files 🔧               |
| <kbd>LEADER</kbd> + <kbd>fs</kbd> | Live Grep    | Find string in current directory 🔧      |
| <kbd>LEADER</kbd> + <kbd>fc</kbd> | Grep Cursor  | Find string under cursor 🔧              |
| <kbd>LEADER</kbd> + <kbd>ft</kbd> | Find TODOs   | Find TODO comments 🔧                    |

### 📝 TODO Comments

| Shortcut      | Action        | Description                      |
| ------------- | ------------- | -------------------------------- |
| <kbd>]t</kbd> | Next TODO     | Jump to next TODO comment 🔧     |
| <kbd>[t</kbd> | Previous TODO | Jump to previous TODO comment 🔧 |

### 🔤 Surround Operations

> **nvim-surround plugin** - Manipulate surrounding characters

| Operation  | Before                     | Command     | After                   |
| ---------- | -------------------------- | ----------- | ----------------------- |
| **Add**    | `surr*ound_words`          | `ysiw)`     | `(surround_words)`      |
| **Add**    | `*make strings`            | `ys$"`      | `"make strings"`        |
| **Delete** | `[delete ar*ound me!]`     | `ds]`       | `delete around me!`     |
| **Delete** | `remove <b>HTML t*ags</b>` | `dst`       | `remove HTML tags`      |
| **Change** | `'change quot*es'`         | `cs'"`      | `"change quotes"`       |
| **Change** | `<b>or tag* types</b>`     | `csth1<CR>` | `<h1>or tag types</h1>` |
| **Delete** | `delete(functi*on calls)`  | `dsf`       | `function calls`        |

---

<!-- markdownlint-enable MD033 -->
