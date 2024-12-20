# LabelImg - Fixed Version

This repository contains important fixes for the LabelImg tool, specifically addressing float-to-integer conversion issues that were causing problems in the original implementation.

## Key Fixes

The main fixes in this fork address float-related issues in coordinate handling and canvas rendering. These problems were causing various stability issues and drawing inaccuracies in the original version.

### Fixed Files
- `labelImg.py`: Converted float coordinates to integers for stable GUI rendering
- `canvas.py`: Fixed float-to-integer conversions for accurate shape drawing and selection

## Installation Options

### Option 1: Manual File Replacement
If you already have LabelImg installed and just want to apply the fixes:

1. Navigate to these directories on your system:
   - For `labelImg.py`:
     ```
     C:\Users\<your_username>\AppData\Roaming\Python\Python312\site-packages\labelImg
     ```
   - For `canvas.py`:
     ```
     C:\Users\<your_username>\AppData\Roaming\Python\Python312\site-packages\libs
     ```
2. Replace these files with the fixed versions from this repository
3. Restart LabelImg for the changes to take effect

### Option 2: Full Repository Clone
If you prefer to install the entire fixed version:

1. Clone this repository:
   ```bash
   git clone https://github.com/s3koni/labelImg-float-fix
   ```
2. Follow the standard LabelImg installation instructions

## Technical Details

The fixes primarily involve:
- Converting float coordinates to integers before GUI operations
- Ensuring consistent integer-based calculations in the canvas drawing system
- Maintaining precision while avoiding float-related rendering artifacts

## Compatibility

These fixes have been tested with:
- Python 3.12
- Latest PyQt version
- Windows 10/11

## Contributing

While this is a maintenance fork focused on stability, contributions and issue reports are welcome. Please ensure any pull requests maintain the integer-based coordinate system implemented in these fixes.

## Original Project

This is a fork of the original LabelImg project, created to maintain a stable version with critical fixes. The original project can be found at https://github.com/HumanSignal/labelImg.

## License

This project maintains the same license as the original LabelImg project.
