<div align = center>

# AltTab

[![Screenshot](screenshot.png)](screenshot.png)

**AltTab** brings the power of Windows alt-tab to macOS

> **Note:** This is a personal fork that adds a Windows-style taskbar feature. For the official AltTab, visit [lwouis/alt-tab-macos](https://github.com/lwouis/alt-tab-macos).

</div>

## Features

### Windows-style Taskbar

This fork adds a **persistent Windows-style taskbar** at the bottom of the screen:

- Shows all open windows with app icons and titles
- Click to focus any window instantly
- Hover to preview window thumbnails
- Per-screen taskbar for multi-monitor setups
- Filter by current Space or show all windows
- Automatically adjusts maximized windows to leave room for the taskbar
- Fully customizable: height, icon size, font size, and more

Configure in **Preferences → Appearance → Taskbar**.

## Building from Source

### Prerequisites

- macOS 10.13+
- Xcode 12+
- [CocoaPods](https://cocoapods.org/)

### Build

```bash
# Install dependencies
pod install

# Build Debug version
xcodebuild -workspace alt-tab-macos.xcworkspace -scheme Debug -configuration Debug build

# Build Release version
xcodebuild -workspace alt-tab-macos.xcworkspace -scheme Release -configuration Release build
```

### Run

```bash
# Open the built app (Debug)
open ~/Library/Developer/Xcode/DerivedData/alt-tab-macos-*/Build/Products/Debug/AltTab.app

# Or use Xcode to build and run
open alt-tab-macos.xcworkspace
# Then press Cmd+R in Xcode
```
