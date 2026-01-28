# Ghostty EUI Themes

Ghostty terminal themes based on the [Elastic UI Framework](https://eui.elastic.co) color palette.

## Themes

### EUI Dark (`eui-dark`)
A dark theme using EUI's fullShade (`#07101F`) as the background with light foreground text. Best for extended terminal use.

### EUI Light (`eui-light`)
A light theme using EUI's body background (`#F6F9FC`) with dark text. Matches the default Elastic/Kibana interface appearance.

## Color Mapping

| ANSI Color | EUI Token | Purpose |
|------------|-----------|---------|
| Black (0) | darkestShade | Subdued backgrounds |
| Red (1) | danger | Errors, destructive actions |
| Green (2) | success | Positive messages, additions |
| Yellow (3) | warning | Warnings, caution |
| Blue (4) | primary | Main brand, links, CTAs |
| Magenta (5) | accent | Notifications, selections |
| Cyan (6) | accentSecondary | Secondary highlights |
| White (7) | lightShade/mediumShade | Light text, borders |

Bright colors (8-15) use lighter variants from EUI's visualization and severity palettes.

## Installation

### Option 1: User Config Directory
Copy the theme files to your Ghostty themes directory:

```bash
mkdir -p ~/.config/ghostty/themes
cp eui-dark eui-light ~/.config/ghostty/themes/
```

### Option 2: Reference by Path
Reference the theme directly in your Ghostty config:

```
theme = /path/to/eui-dark
```

## Usage

Add to your `~/.config/ghostty/config`:

```
# For dark theme
theme = eui-dark

# For light theme
theme = eui-light

# Auto-switch based on system appearance
theme = dark:eui-dark,light:eui-light
```

## Preview Colors

**EUI Dark:**
- Background: `#07101F` (fullShade)
- Foreground: `#E3E8F2` (lightText)
- Primary/Blue: `#0B64DD`
- Accent/Magenta: `#BC1E70`
- Cyan/Teal: `#008B87`

**EUI Light:**
- Background: `#F6F9FC` (body)
- Foreground: `#1D2A3E` (textParagraph)
- Uses text-optimized color variants for better contrast

## License

These themes are based on the Elastic UI color palette. Elastic UI is licensed under the Elastic License 2.0.
