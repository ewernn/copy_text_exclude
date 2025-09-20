# Copy Text Exclude - Firefox Extension

A Firefox extension that lets you copy text from webpages while excluding specific portions you don't want.

## How to Use

1. **Enter Exclusion Mode**: Press `Cmd+Shift+E` (Mac) or `Ctrl+Shift+E` (PC)
   - The page border turns blue when active

2. **Mark Text to Exclude**: Click and drag to select text you DON'T want
   - Selected text gets strikethrough styling
   - Select multiple portions as needed - they all stay marked

3. **Select What to Copy**:
   - Select the specific text/section you want to copy (it will skip the strikethrough parts)
   - OR press `Cmd+A`/`Ctrl+A` to select all (the entire page minus strikethrough parts)

4. **Copy**: Press `Cmd+C` (Mac) or `Ctrl+C` (PC)
   - Copies your selection WITHOUT the strikethrough portions
   - The border flashes green to confirm
   - All exclusions automatically clear after copying
   - Extension exits exclusion mode

5. **Exit Without Copying**: Press `Escape` or `Cmd+Shift+E` again

## Installation

### Temporary Installation (for testing):
1. Open Firefox and navigate to `about:debugging`
2. Click "This Firefox" on the left sidebar
3. Click "Load Temporary Add-on"
4. Navigate to the `copy_text_exclude` folder and select `manifest.json`
5. The extension is now installed temporarily (until Firefox restarts)


## Example

If you have a webpage with:
```
This is a paragraph with some unwanted advertisement text in the middle that you don't want to copy.
```

1. Press `Cmd+Shift+E` to enter exclusion mode
2. Select "unwanted advertisement text" (it gets strikethrough)
3. Select the whole sentence (or press Cmd+A for entire page)
4. Press `Cmd+C`

Your clipboard will contain:
```
This is a paragraph with some in the middle that you don't want to copy.
```

## Features

- **Visual feedback** with strikethrough text for exclusions
- **Mark multiple exclusions** before copying
- **Works with partial or full page selection**
- **Auto-clears and exits** after successful copy
- **Clean copy** without excluded portions
- **Privacy-focused** - Only requires active tab access, no data collection