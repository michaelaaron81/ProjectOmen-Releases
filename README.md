# Project Omen

A desktop application for editing and managing RPG game data files.

## Download

**[Download Latest Release](https://github.com/michaelaaron81/ProjectOmen-Releases/releases/latest)**

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

## Support

For issues or questions, please open an issue on this repository.

---

## Updating Releases (Developer Notes)

### Prerequisites
- GitHub CLI installed and authenticated: `gh auth login`
- Installer built in main project: `npm run dist` from `D:\Omen\rpr-parser-editor`

### Steps to Create a New Release

1. **Build the installer** in your main project:
   ```powershell
   cd D:\Omen\rpr-parser-editor
   npm run dist
   ```
   This creates `release\Project Omen Setup X.X.X.exe`

2. **Create the GitHub release**:
   ```powershell
   cd D:\Omen\ProjectOmen-Releases
   gh release create vX.X.X "D:\Omen\rpr-parser-editor\release\Project Omen Setup X.X.X.exe" --title "Project Omen vX.X.X" --notes "Release notes here"
   ```

3. **Example**:
   ```powershell
   gh release create v0.0.2 "D:\Omen\rpr-parser-editor\release\Project Omen Setup 0.0.2.exe" --title "Project Omen v0.0.2" --notes "Bug fixes and improvements"
   ```

### Notes
- This repository only contains the README and binary releases
- Source code is kept private in the main ProjectOmen repository
- The auto-generated source archives from GitHub only contain this README
