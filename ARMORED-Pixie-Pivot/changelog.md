# PIXIE PIVOT CHANGELOG

## 1.1.0
03/September/2025

### ADDED
- New Toggle Key 'Anchor to Selection' [T]: Allows aligning to other elements while keeping your pivot point near your selection.

### FIXED
- Incorrect HUD position when the 3d region was not at the bottom left.
- Obscure case where release_check would say an update was available if the addon crashed (failed version check returned (0, 0, 0) istead of None).

### CHANGED
- Only draw HUDs in a single 3DView (the one that called Pixie Pivot).
- Mouse HUD is slightly bigger (0.8 of the Fixed HUD size instead of 0.7).

## 1.0.0
28/August/2025

### INITIAL RELEASE
