# Project Omen

A desktop application for editing and managing RPR game data files.

## Download

**[Download Latest Release](https://github.com/michaelaaron81/ProjectOmen-Releases/releases/latest)**

Or download directly: **[Project Omen Setup 0.0.6.exe](https://github.com/michaelaaron81/ProjectOmen-Releases/raw/main/Project%20Omen%20Setup%200.0.6.exe)**

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
