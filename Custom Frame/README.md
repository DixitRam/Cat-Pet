# Custom Frame Instructions

Want to add your own custom pet? Follow these instructions to create a custom sprite sheet.

## Recommended Free Tools
- **Piskel** (Online/Offline): Great for beginners.
- **LibreSprite**: A powerful free alternative to Aseprite.
- **GIMP**: Advanced image editing.

## 1. File Specifications
- **Format**: PNG (Transparent background)
- **Dimensions**: `256px` (width) x `128px` (height)
- **Grid Unit**: Typically `32px` x `32px` (but some frames vary slightly).

## 2. Sprite Layout
The extension reads specific coordinates `(X, Y)` for each animation frame. You must place your artwork at these exact locations.

### Running Animations (8 Directions)
Each direction has **2 frames** that loop for the walking animation.

| Direction | Size (WxH) | Frame 1 Pos (X, Y) | Frame 2 Pos (X, Y) |
| :--- | :--- | :--- | :--- |
| **Right** | 32x28 | `95, 0` | `96, 33` |
| **Left** | 32x28 | `129, 64` | `128, 99` |
| **Up** | 32x32 | `32, 64` | `32, 96` |
| **Down** | 32x32 | `193, 96` | `224, 63` |
| **Top-Left** | 32x32 | `34, 0` | `33, 30` |
| **Top-Right** | 32x32 | `0, 64` | `0, 96` |
| **Bot-Left** | 32x32 | `160, 96` | `128, 96` |
| **Bot-Right**| 32x32 | `160, 33` | `162, 62` |

### Idle Animations
These play when the cat stops moving.

| State | Size | Position (X, Y) |
| :--- | :--- | :--- |
| **Still** (Stop) | 32x32 | `96, 96` |
| **Transition** | 32x32 | `96, 63` |
| **Breathing 1**| 32x32 | `64, 0` |
| **Breathing 2**| 32x32 | `64, 32` |

### Other Areas
Any other parts of the sprite sheet not listed above are reserved **For Future Use**. Please leave them blank or transparent.

## 3. How to Install Your Custom Cat
1. Create your sprite sheet using the coordinates above.
2. Name the file `Frames.png`.
3. Replace the existing file at:
   `/Frames/Frames.png`
4. Reload the extension in your browser.

**Note**: Deviating from these pixel coordinates will cause the cat to "jump" or clip during animations. Reference `sprite_template.svg` (in the root folder) for a visual guide.
