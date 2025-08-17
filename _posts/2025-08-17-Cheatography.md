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

<!-- Search Bar Styles -->
<style>
/* Global Enhancements */
body {
  line-height: 1.7;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
}

/* Enhanced Search Container */
.search-container {
  position: sticky;
  top: 70px;
  z-index: 1000;
  background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
  padding: 25px;
  border-radius: 15px;
  box-shadow: 0 8px 32px rgba(0,0,0,0.15);
  margin-bottom: 40px;
  border: none;
  backdrop-filter: blur(10px);
}

.search-box {
  width: 100%;
  padding: 18px 25px;
  font-size: 16px;
  border: none;
  border-radius: 50px;
  outline: none;
  transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
  box-sizing: border-box;
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(10px);
  box-shadow: 0 4px 20px rgba(0,0,0,0.1);
}

.search-box:focus {
  transform: translateY(-2px);
  box-shadow: 0 8px 30px rgba(0,0,0,0.2);
  background: rgba(255, 255, 255, 1);
}

.search-box::placeholder {
  color: #666;
  font-style: italic;
}

.search-stats {
  margin-top: 15px;
  color: rgba(255, 255, 255, 0.9);
  font-size: 14px;
  text-align: center;
  font-weight: 500;
  text-shadow: 0 1px 2px rgba(0,0,0,0.1);
}

.clear-search {
  position: absolute;
  right: 35px;
  top: 50%;
  transform: translateY(-50%);
  background: linear-gradient(135deg, #ff6b6b, #ee5a52);
  color: white;
  border: none;
  border-radius: 50%;
  width: 30px;
  height: 30px;
  cursor: pointer;
  font-size: 14px;
  font-weight: bold;
  display: none;
  transition: all 0.3s ease;
  box-shadow: 0 2px 10px rgba(238, 90, 82, 0.3);
}

.clear-search:hover {
  transform: translateY(-50%) scale(1.1);
  box-shadow: 0 4px 15px rgba(238, 90, 82, 0.5);
}

/* Enhanced Table Styles */
table {
  margin: 25px 0;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  background: white;
  border-collapse: separate;
  border-spacing: 0;
}

thead th {
  background: linear-gradient(135deg, #2c3e50, #34495e);
  color: white;
  font-weight: 600;
  padding: 16px 20px;
  text-transform: uppercase;
  letter-spacing: 0.5px;
  font-size: 13px;
  position: relative;
}

thead th:first-child {
  border-radius: 12px 0 0 0;
}

thead th:last-child {
  border-radius: 0 12px 0 0;
}

tbody tr {
  transition: all 0.3s ease;
  border-bottom: 1px solid #f1f3f4;
}

tbody tr:hover {
  background: linear-gradient(135deg, #f8f9ff, #e8f4f8);
  transform: scale(1.002);
  box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}

tbody tr:last-child:hover td:first-child {
  border-radius: 0 0 0 12px;
}

tbody tr:last-child:hover td:last-child {
  border-radius: 0 0 12px 0;
}

tbody td {
  padding: 14px 20px;
  vertical-align: top;
}

/* Enhanced Heading Styles */
h1 {
  text-align: center;
  background: linear-gradient(135deg, #667eea, #764ba2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
  font-size: 2.5em;
  font-weight: 700;
  margin: 30px 0;
  text-shadow: 0 2px 4px rgba(0,0,0,0.1);
}

h2 {
  background: linear-gradient(135deg, #667eea, #764ba2);
  color: white;
  padding: 20px 25px;
  border-radius: 12px;
  margin: 40px 0 25px 0;
  font-size: 1.6em;
  font-weight: 600;
  box-shadow: 0 4px 15px rgba(102, 126, 234, 0.3);
  position: relative;
  overflow: hidden;
}

h2::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
  transition: left 0.8s;
}

h2:hover::before {
  left: 100%;
}

h3 {
  color: #2c3e50;
  border-left: 5px solid #3498db;
  padding: 12px 20px;
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
  border-radius: 0 8px 8px 0;
  margin: 30px 0 20px 0;
  font-size: 1.3em;
  font-weight: 600;
  box-shadow: 0 2px 8px rgba(0,0,0,0.05);
}

h4 {
  color: #34495e;
  font-size: 1.1em;
  font-weight: 600;
  margin: 25px 0 15px 0;
  padding-bottom: 8px;
  border-bottom: 2px solid #ecf0f1;
}

/* Enhanced Blockquote */
blockquote {
  background: linear-gradient(135deg, #e8f5e8, #f0f8f0);
  border-left: 5px solid #27ae60;
  padding: 20px 25px;
  margin: 25px 0;
  border-radius: 0 12px 12px 0;
  box-shadow: 0 2px 10px rgba(39, 174, 96, 0.1);
  position: relative;
}

blockquote::before {
  content: '"';
  font-size: 4em;
  color: rgba(39, 174, 96, 0.1);
  position: absolute;
  top: -10px;
  left: 20px;
  font-family: serif;
}

/* Enhanced KBD styling - Note: No click functionality */
kbd {
  background: linear-gradient(135deg, #f8f9fa, #e9ecef);
  border: 2px solid #ced4da;
  border-radius: 6px;
  box-shadow: 0 3px 0 #adb5bd, 0 0 0 1px rgba(0,0,0,0.1);
  color: #495057;
  display: inline-block;
  font-family: 'SF Mono', 'Monaco', 'Inconsolata', 'Roboto Mono', monospace;
  font-size: 0.9em;
  font-weight: 600;
  line-height: 1;
  padding: 6px 10px;
  margin: 0 3px;
  text-shadow: 0 1px 0 rgba(255,255,255,0.8);
  transition: all 0.2s ease;
  /* Preserve original case - no text-transform */
}

kbd:hover {
  transform: translateY(-1px);
  box-shadow: 0 4px 0 #adb5bd, 0 2px 8px rgba(0,0,0,0.15);
}

/* Highlight Effects */
.highlight {
  background: linear-gradient(135deg, #fff3cd, #ffeaa7);
  padding: 3px 6px;
  border-radius: 6px;
  font-weight: 700;
  border: 2px solid #f39c12;
  box-shadow: 0 2px 8px rgba(243, 156, 18, 0.3);
  animation: highlightPulse 1.5s ease-in-out;
}

@keyframes highlightPulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.05); }
}

.hidden-row {
  display: none;
}

/* Responsive Design */
@media (max-width: 768px) {
  .search-container {
    margin: 15px -10px 25px -10px;
    border-radius: 0;
    top: 0;
  }
  
  h1 {
    font-size: 2em;
  }
  
  table {
    font-size: 14px;
  }
  
  thead th, tbody td {
    padding: 10px 12px;
  }
}

/* Custom Scrollbar */
::-webkit-scrollbar {
  width: 8px;
}

::-webkit-scrollbar-track {
  background: #f1f1f1;
  border-radius: 4px;
}

::-webkit-scrollbar-thumb {
  background: linear-gradient(135deg, #667eea, #764ba2);
  border-radius: 4px;
}

::-webkit-scrollbar-thumb:hover {
  background: linear-gradient(135deg, #5a67d8, #6b46c1);
}
</style>

<!-- Search Bar -->
<div class="search-container">
  <div style="position: relative;">
    <input 
      type="text" 
      id="searchInput" 
      class="search-box" 
      placeholder="🔍 Search shortcuts, actions, or descriptions... (try 'split', 'SUPER+B', 'terminal')"
      autocomplete="off"
    >
    <button id="clearSearch" class="clear-search" title="Clear search">×</button>
  </div>
  <div id="searchStats" class="search-stats"></div>
</div>

# 🎮 Personal Keybindings Cheat Sheet

<div style="text-align: center; margin: 30px 0; padding: 20px; background: linear-gradient(135deg, #f8f9fa, #e9ecef); border-radius: 12px; border: 2px solid #dee2e6;">
  <p style="font-size: 1.2em; color: #495057; margin: 0; font-weight: 500;">
    ⚡ A comprehensive reference for all my customized keyboard shortcuts across different applications
  </p>
  <p style="font-size: 0.95em; color: #6c757d; margin: 10px 0 0 0; font-style: italic;">
    💡 Boost your productivity with lightning-fast navigation and control
  </p>
</div>

> 📝 **Legend & Quick Guide**:
>
> <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 15px; margin: 15px 0;">
>   <div style="background: #e8f4f8; padding: 12px; border-radius: 8px; border-left: 4px solid #3498db;">
>     <strong>🔑 Key Symbols:</strong><br>
>     <kbd>SUPER</kbd> = Windows/Cmd key<br>
>     <kbd>LEADER</kbd> = Leader key sequence
>   </div>
>   <div style="background: #fff3e0; padding: 12px; border-radius: 8px; border-left: 4px solid #ff9800;">
>     <strong>⚙️ Configuration:</strong><br>
>     Actions marked with 🔧 are custom configurations
>   </div>
> </div>
>
> <div style="background: #f0f8e8; padding: 15px; border-radius: 8px; border-left: 4px solid #4caf50; margin-top: 15px;">
>   <strong>💡 Pro Tips:</strong>
>   <ul style="margin: 8px 0 0 0; padding-left: 20px;">
>     <li>Use <kbd>Ctrl</kbd>/<kbd>Cmd</kbd> + <kbd>F</kbd> to quickly focus the search box above</li>
>     <li>Search by application name, key combination, or action description</li>
>     <li>Press <kbd>Esc</kbd> to clear search and show all shortcuts</li>
>   </ul>
> </div>

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

<!-- Search Functionality -->
<script>
// Enhanced search functionality (without click-to-copy)
const searchInput = document.getElementById('searchInput');
const clearButton = document.getElementById('clearSearch');
const searchStats = document.getElementById('searchStats');
let allRows = [];
let totalResults = 0;
let searchHistory = [];

// Initialize when DOM is loaded
document.addEventListener('DOMContentLoaded', function() {
  // Get all table rows except headers
  allRows = Array.from(document.querySelectorAll('tr')).filter(row => {
    return !row.querySelector('th') && row.cells && row.cells.length > 0;
  });
  
  updateSearchStats();
  initializeEnhancements();
});

// Initialize additional enhancements (without click-to-copy)
function initializeEnhancements() {
  // Add loading animation to search box
  searchInput.addEventListener('focus', function() {
    this.style.transform = 'translateY(-2px)';
  });
  
  searchInput.addEventListener('blur', function() {
    this.style.transform = 'translateY(0)';
  });
  
  // Add smooth scroll to first result
  searchInput.addEventListener('keydown', function(e) {
    if (e.key === 'Enter' && totalResults > 0) {
      const firstVisibleRow = allRows.find(row => !row.classList.contains('hidden-row'));
      if (firstVisibleRow) {
        firstVisibleRow.scrollIntoView({ 
          behavior: 'smooth', 
          block: 'center' 
        });
        // Add temporary highlight to first result
        firstVisibleRow.style.animation = 'highlightPulse 2s ease-in-out';
        setTimeout(() => {
          firstVisibleRow.style.animation = '';
        }, 2000);
      }
    }
  });
}

// Debounce function to improve performance
function debounce(func, wait) {
  let timeout;
  return function executedFunction(...args) {
    const later = () => {
      clearTimeout(timeout);
      func(...args);
    };
    clearTimeout(timeout);
    timeout = setTimeout(later, wait);
  };
}

// Remove previous highlights with animation
function removeHighlights() {
  document.querySelectorAll('.highlight').forEach(el => {
    el.style.transition = 'all 0.3s ease';
    el.style.opacity = '0';
    el.style.transform = 'scale(0.8)';
    
    setTimeout(() => {
      const parent = el.parentNode;
      parent.replaceChild(document.createTextNode(el.textContent), el);
      parent.normalize();
    }, 300);
  });
}

// Enhanced highlight with animation
function highlightText(element, searchTerm) {
  if (!searchTerm.trim()) return;
  
  const textNodes = [];
  const walker = document.createTreeWalker(
    element,
    NodeFilter.SHOW_TEXT,
    null,
    false
  );
  
  let node;
  while (node = walker.nextNode()) {
    textNodes.push(node);
  }
  
  textNodes.forEach(textNode => {
    const text = textNode.textContent;
    const regex = new RegExp(`(${searchTerm.replace(/[.*+?^${}()|[\]\\]/g, '\\$&')})`, 'gi');
    
    if (regex.test(text)) {
      const highlightedHTML = text.replace(regex, '<span class="highlight" style="opacity: 0; transform: scale(0.8);">$1</span>');
      const wrapper = document.createElement('div');
      wrapper.innerHTML = highlightedHTML;
      
      while (wrapper.firstChild) {
        textNode.parentNode.insertBefore(wrapper.firstChild, textNode);
      }
      textNode.remove();
    }
  });
  
  // Animate highlights
  setTimeout(() => {
    document.querySelectorAll('.highlight').forEach((highlight, index) => {
      setTimeout(() => {
        highlight.style.transition = 'all 0.4s cubic-bezier(0.4, 0, 0.2, 1)';
        highlight.style.opacity = '1';
        highlight.style.transform = 'scale(1)';
      }, index * 50);
    });
  }, 100);
}

// Enhanced search function with animations
function performSearch() {
  const searchTerm = searchInput.value.toLowerCase().trim();
  
  // Add to search history
  if (searchTerm && !searchHistory.includes(searchTerm)) {
    searchHistory.unshift(searchTerm);
    searchHistory = searchHistory.slice(0, 10); // Keep last 10 searches
  }
  
  removeHighlights();
  totalResults = 0;

  if (!searchTerm) {
    // Show all rows with fade-in animation
    allRows.forEach((row, index) => {
      row.classList.remove('hidden-row');
      row.style.opacity = '0';
      row.style.transform = 'translateY(10px)';
      
      setTimeout(() => {
        row.style.transition = 'all 0.3s ease';
        row.style.opacity = '1';
        row.style.transform = 'translateY(0)';
      }, index * 20);
    });
    
    clearButton.style.display = 'none';
    updateSearchStats();
    return;
  }

  clearButton.style.display = 'block';

  // Search with animations
  allRows.forEach((row, index) => {
    const rowText = row.textContent.toLowerCase();
    const isMatch = rowText.includes(searchTerm);
    
    if (isMatch) {
      row.classList.remove('hidden-row');
      highlightText(row, searchTerm);
      totalResults++;
      
      // Animate visible rows
      row.style.opacity = '0';
      row.style.transform = 'translateX(-20px)';
      
      setTimeout(() => {
        row.style.transition = 'all 0.4s cubic-bezier(0.4, 0, 0.2, 1)';
        row.style.opacity = '1';
        row.style.transform = 'translateX(0)';
      }, index * 30);
    } else {
      // Animate hiding rows
      row.style.transition = 'all 0.3s ease';
      row.style.opacity = '0';
      row.style.transform = 'translateX(20px)';
      
      setTimeout(() => {
        row.classList.add('hidden-row');
        row.style.transform = 'translateX(0)';
      }, 300);
    }
  });

  updateSearchStats();
}

// Enhanced search statistics with animations
function updateSearchStats() {
  const statsText = !searchInput.value.trim() 
    ? `Ready to search ${allRows.length} shortcuts`
    : totalResults === 0 
      ? 'No results found - try different keywords'
      : `Found ${totalResults} result${totalResults !== 1 ? 's' : ''} • Press Enter to jump to first`;
  
  const statsColor = !searchInput.value.trim() 
    ? 'rgba(255, 255, 255, 0.8)'
    : totalResults === 0 
      ? '#ff6b6b'
      : '#00d4aa';
  
  // Animate stats update
  searchStats.style.transition = 'all 0.3s ease';
  searchStats.style.opacity = '0';
  searchStats.style.transform = 'translateY(-10px)';
  
  setTimeout(() => {
    searchStats.textContent = statsText;
    searchStats.style.color = statsColor;
    searchStats.style.opacity = '1';
    searchStats.style.transform = 'translateY(0)';
  }, 150);
}

// Enhanced clear search with animation
function clearSearch() {
  searchInput.value = '';
  
  // Animate clear button
  clearButton.style.transform = 'translateY(-50%) scale(0.8) rotate(90deg)';
  clearButton.style.opacity = '0.5';
  
  setTimeout(() => {
    clearButton.style.display = 'none';
    clearButton.style.transform = 'translateY(-50%) scale(1) rotate(0deg)';
    clearButton.style.opacity = '1';
  }, 200);
  
  removeHighlights();
  
  // Show all rows with stagger animation
  allRows.forEach((row, index) => {
    row.classList.remove('hidden-row');
    row.style.opacity = '0';
    row.style.transform = 'translateY(10px)';
    
    setTimeout(() => {
      row.style.transition = 'all 0.3s ease';
      row.style.opacity = '1';
      row.style.transform = 'translateY(0)';
    }, index * 15);
  });
  
  updateSearchStats();
  searchInput.focus();
}

// Event listeners
if (searchInput) {
  searchInput.addEventListener('input', debounce(performSearch, 250));
}

if (clearButton) {
  clearButton.addEventListener('click', clearSearch);
}

// Enhanced keyboard shortcuts
document.addEventListener('keydown', function(e) {
  // Ctrl/Cmd + F to focus search
  if ((e.ctrlKey || e.metaKey) && e.key === 'f') {
    e.preventDefault();
    if (searchInput) {
      searchInput.focus();
      searchInput.select();
      // Add focus animation
      searchInput.style.transform = 'translateY(-3px) scale(1.02)';
      setTimeout(() => {
        searchInput.style.transform = 'translateY(-2px) scale(1)';
      }, 200);
    }
  }
  
  // Escape to clear search
  if (e.key === 'Escape' && document.activeElement === searchInput) {
    clearSearch();
  }
  
  // Ctrl/Cmd + K for quick search (popular shortcut)
  if ((e.ctrlKey || e.metaKey) && e.key === 'k') {
    e.preventDefault();
    if (searchInput) {
      searchInput.focus();
      searchInput.select();
    }
  }
});

// Add CSS for additional animations
const additionalStyles = `
  .search-container:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 40px rgba(0,0,0,0.2);
  }
  
  /* Smooth transitions for interactive elements */
  table tr, .search-container, kbd {
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
`;

// Inject additional styles
const styleSheet = document.createElement('style');
styleSheet.textContent = additionalStyles;
document.head.appendChild(styleSheet);
</script>

---
