# Moz-Mac Firefox Theme
## by Thomas McMahon / @twistermc / twistermc.com
A modern glass-like theme for Firefox on macOS with dynamic light/dark mode support

## Features
- Automatic light/dark mode switching based on system preferences
- Glass-like transparency effects
- Native macOS appearance
- Transparent URL bar with opaque focus state
- Translucent sidebar and bookmarks
- Window state awareness (inactive window styling)

## Installation
1. Go to `about:support` in Firefox
2. Find the Profile Folder and click "Show in Finder"
3. Open the `chrome` directory (create it if it doesn't exist)
4. Create a folder called `moz-mac`
5. Download `userChrome.css` and save it to the `moz-mac` folder
6. Go back one directory and open/create `userChrome.css`
7. Add this line at the beginning: `@import "moz-mac/userChrome.css";`

## Required Firefox Settings
1. Open `about:config` in Firefox
2. Set these preferences to `true`:
   - `toolkit.legacyUserProfileCustomizations.stylesheets`
   - `layout.css.backdrop-filter.enabled`
   - `gfx.webrender.all` (optional)
3. Restart Firefox

## Customization
If you know how Firefox CSS works, you can customize the theme by adjusting the variables at the top of the CSS file:

### Transparency Settings (0 = transparent, 1 = opaque)
```css
--window-transparency: 0.0;     /* Overall window transparency */
--toolbar-transparency: 0.6;     /* Toolbar and tabs transparency */
--content-transparency: 0.5;     /* Content area transparency */
--urlbar-transparency: 0.0;     /* URL bar transparency when not focused */
--bookmark-transparency: 0.7;    /* Bookmarks and menus transparency */
```

### Visual Effects
```css
--blur-strength: 10px;          /* Strength of the blur effect */
--glass-saturation: 1.8;        /* Color saturation for glass effect */
--glass-brightness: 1.1;        /* Brightness for glass effect */
```

## Version History
- v2.1.0 - Added window state awareness, improved glass effects, better sidebar transparency
- v2.0.0 - Major update to make it compatible with newer versions of Firefox.
- v1.0.0 - Initial Release

## Compatibility
- Tested on Firefox 115+
- Test on macOS
- Requires macOS Catalina or later for best blur effects

## Troubleshooting
- If transparency isn't working, make sure all required `about:config` settings are enabled
- If the theme doesn't load, verify the file paths and CSS import statement
- For the best experience, use the "System theme" in Firefox's theme settings

## Contributing
Feel free to submit issues and pull requests to improve the theme!
