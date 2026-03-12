# PIXIE PIVOT CHANGELOG

## 1.2.1
12/March/2026

### Fixed
- AttributeError `build_element_styles` when resetting certain Prop Groups.

## 1.2.0
12/March/2026

### Added
- Support for targeting mesh elements while in Object Mode.
- Snap/align between multiple objects (still limited to mesh objects).
- Lock Cursor Location → Prevents the 3D cursor from changing location while still allowing it to rotate/align in place.
- Bounding Box Calculation preferences: Accurate (default) vs Fast.

### Changed
- Converted the add-on into an extension.

Removed
- Anchor to Selection → Too much dev time; may re-add if the API exposes transform_orientation and transform_pivot_point results. Replaced with simpler **Lock Cursor Location**.
- Release Checking → It was pretty useless anyway (no updating and version notifications were super hidden).


## 1.1.4
09/Febuary/2026

### CHANGED
- Setting the Origin no longer forces GLOBAL Orientation and MEDIAN_POINT Pivot, instead it keeps your previous settings.


## 1.1.3
11/October/2025

### FIXED
- Error when enabling `anchor_to_selection` and no selection was available.


## 1.1.2
06/October/2025

### ADDED
- Behavior Preference **Double Tap Resets To** with pivot reset options.

### CHANGED
- Pressing 'DD' now resets the pivot to the previous non-cursor settings instead of always reseting to GLOBAL Orientation and MEDIAN_POINT pivot point.


## 1.1.1
06/September/2025

### FIXED
- AttributeError → `view3d_utils` was not being imported correctly from `bpy_extras`.


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
