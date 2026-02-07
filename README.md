# Project Omen

A desktop application for editing and managing RPR game data files.

## Download

**[Download Latest Release](https://github.com/michaelaaron81/ProjectOmen-Releases/releases/latest)**

Or download directly: **[Project Omen Setup 0.0.7.exe](https://github.com/michaelaaron81/ProjectOmen-Releases/raw/main/Project%20Omen%20Setup%200.0.7.exe)**

### Installation

1. Download the setup.exe from the releases page
2. Run the installer
3. Windows may show a security warning (this is normal for unsigned software)
   - Click "More info"
   - Click "Run anyway"
4. Follow the installation prompts

## Features

- Visual editor for game data with structured forms
- Drag & drop reordering
- Raw text editor with find/replace
- Keyboard navigation
- Auto-save functionality
- Offline-first design

## Release Notes

### v0.0.7 (February 7, 2026)

**Character Sheet Experience Improvements:**
- Added independent zoom control for character sheet (Ctrl+scroll to zoom 0.5x-2.5x)
- Zoom level is now persisted when closing/reopening the sheet
- Chat panel can now be docked beside the sheet or floating/draggable anywhere
- Docked chat sits as an independent 380px panel next to the sheet (not inside it)
- Floating chat can be dragged by its title bar and resized from the bottom-right corner
- Added "Chat" toggle button in sheet header to show/hide chat
- Undock (↗) and Dock (☰) buttons to switch between modes
- Removed dependency on chat layout settings - simpler dock/float model

**Technical:**
- Cleaned up chat layout logic for better maintainability
- Fixed syntax errors in perk description parsing
- Chat state persists across docked/floating modes

### v0.0.6 (February 4, 2026)

**Character Sheet Enhancements:**
- Added comprehensive perk selection system with detailed cards showing bonuses and costs
- Implemented point tracking system (Attributes, Skills, and Perks)
- Perks now hide from available list when chosen
- Added cost enforcement - perks are disabled when insufficient points remain
- Improved modal layout with proper scrolling and centering
- Fixed window resizability and movability for Electron builds

**UI Improvements:**
- Enhanced perk cards display parsed bonuses (e.g., "Body +2", "Athletics +1")
- Added available points indicator showing remaining/total for each resource type
- Better visual hierarchy with themed colors and consistent spacing
- Character name field at top of character sheet

**Technical:**
- Converted chat state to React Context for proper synchronization
- Fixed DiceConfig/DiceRules/Gear export order in raw editor
- Text-based roll format: "Name has rolled Skill (formula) for a total of X"
- Point buy system with escalating costs

### Notes
- This repository only contains the README and binary releases
- Source code is kept private in the main ProjectOmen repository
- The auto-generated source archives from GitHub only contain this README
