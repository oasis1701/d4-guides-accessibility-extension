# Mobalytics Accessibility Extension for Diablo 4

A Chrome extension that makes Diablo 4 build guides on [Mobalytics.gg](https://mobalytics.gg) accessible to screen reader users.

## Overview

Mobalytics.gg provides excellent Diablo 4 build guides, but the visual paragon board layouts are not accessible to screen reader users. This extension converts those visual boards into navigable HTML tables that work with screen readers like NVDA, JAWS, and VoiceOver.

## Current Features

### Paragon Board Accessibility

- **Converts visual paragon boards to accessible tables** - Navigate nodes using standard table navigation
- **Board rotation support** - Tables are rotated to match the visual orientation, so "rotated right once" means the table layout matches what sighted users see
- **Gate connections** - Gates show which board they connect to (e.g., "Gate to Board 2: Castle / Exploit")
- **Node information** - Each node shows its type (Normal, Magic, Rare, Legendary) and stat bonus (Str, Int, Dex, Will, Damage, etc.)
- **Selection indicators** - Selected nodes are marked with an asterisk (*) and announced as "selected"
- **Glyph information** - Glyph sockets show the equipped glyph name
- **Board stats summary** - Shows total stats for each board (Str, Int, Dex, Will)
- **Selected nodes summary** - Lists count of selected nodes by type
- **Skip links** - Quickly navigate between boards

### Screen Reader Optimizations

- Clean announcements without redundant text
- Proper heading hierarchy for navigation
- Logical reading order that matches visual layout

## Installation

1. Download or clone this repository. For example, If you're using NVDA, press B to find the code menu on this page, press enter, then find the link "download ZIP", and press enter.
2. Extract/unzip the folder to your preferred location. Note, The extracted folder should remain where it is, for your browser to use at any time.
3. Open Chrome or brave,  and go to `about://extensions`
3. Enable "Developer mode", (IT is a toggle)
4. Press enter on  "Load unpacked" button
5. Select the `Mobalytics Accessibility Chrome Extension` folder

## Usage

1. Navigate to any Diablo 4 build guide on Mobalytics.gg
2. The extension automatically converts paragon boards when the page loads
3. Use your screen reader's table navigation to explore the boards
4. Use heading navigation to jump between boards

## What about Skill points?

When you open a build guide in Mobalytics.gg, underneath the Skill Tree heading, you will find a Leveling path checkbox. Check this to receive a text based leveling path of each skill point.
Please note, this path is most accurate if you're viewing a leveling guide. End game builds assume you'll have enough skill points and might not have an accurate leveling path
I will try to make the skill tree accessible for faster end game build reading.

## Planned Features

I will add more features to cover more inaccessible sections as we find them.


## Technical Notes

- The extension only activates on mobalytics.gg
- Original visual boards are hidden but preserved in the DOM
- Board data is parsed from the page's existing HTML structure

## Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

## License

MIT License

## Author
Hadi Rezaei