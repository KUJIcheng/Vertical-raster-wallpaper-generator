# Rasterized Wallpaper Effect with Highlights and Shadows

This Python script processes a given wallpaper image to create a rasterized frosted glass effect. The output image simulates the appearance of vertical slices with added effects such as Gaussian blur, highlights, and shadows for a polished look.

## Features

- **Rasterized Frosted Glass Effect**: Converts the input image into vertical slices.
- **Gaussian Blur**: Applies a customizable blur radius to each slice.
- **Highlights**: Adds a gradient highlight effect to the left side of each slice.
- **Shadows**: Adds a gradient shadow effect to the right side of each slice for a realistic overlay.

## Prerequisites

Ensure you have the following Python packages installed:
- `Pillow` (Python Imaging Library)

Install the required package using:
```bash
pip install pillow
```

# Usage
## Function Definition
```bash
def raster_blur_effect(input_path, output_path, slice_count=15, blur_radius=10, highlight_intensity=0.1, shadow_intensity=0.1):
    """
    Convert the input wallpaper into a rasterized frosted glass effect with added highlights and shadows.

    Parameters:
        input_path (str): File path of the input wallpaper.
        output_path (str): File path for saving the output wallpaper.
        slice_count (int): Number of vertical slices. Default is 15.
        blur_radius (int): Radius of the Gaussian blur. Default is 10.
        highlight_intensity (float): Intensity of the highlight effect. Default is 0.1.
        shadow_intensity (float): Intensity of the shadow effect. Default is 0.1.
    """
```
## Example Call
```bash
raster_blur_effect(
    input_path='input_wallpaper.jpg',
    output_path='output_wallpaper.jpg',
    slice_count=15,      # Number of slices
    blur_radius=10,      # Gaussian blur radius
    highlight_intensity=0.1,  # Highlight intensity
    shadow_intensity=0.1      # Shadow intensity
)
```
# Parameter Descriptions
- **input_path**: Path to the input image file.
- **output_path**: Path to save the processed image.
- **slice_count**: Number of vertical slices. A higher count results in narrower slices.
- **blur_radius**: Controls the amount of Gaussian blur applied to each slice.
- **highlight_intensity**: Intensity of the highlight gradient on the left side of each slice (range: 0.0 to 1.0).
- **shadow_intensity**: Intensity of the shadow gradient on the right side of each slice (range: 0.0 to 1.0).

# Output
The processed image is saved to the specified output path with effects applied as per the given parameters.

# Customization
- Increase or decrease **slice_count** for more or fewer slices.
- Modify **blur_radius** for sharper or smoother blurring.
- Tweak **highlight_intensity** and **shadow_intensity** for subtle or prominent highlights and shadows.