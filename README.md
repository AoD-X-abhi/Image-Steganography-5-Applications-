# Image Steganography in Python

This repository contains a Python-based Image Steganography project that implements five different applications of hiding data within images. The input images can be in formats such as `.jpg`, `.jpeg`, `.png`, etc. The project uses Python libraries such as `os`, `numpy`, `wave`, `cv2`, and `PIL` for encoding and decoding data in images.

## Applications

1. **RGB to RGB**
   - **Description**: Hides one RGB image within another RGB image.
   - **Functionality**: Embeds the RGB pixel values of a hidden image within the RGB values of a cover image by adjusting the least significant bits, ensuring minimal distortion to the cover image.

2. **Grayscale to RGB**
   - **Description**: Hides a grayscale image inside an RGB image.
   - **Functionality**: Encodes grayscale pixel values into the cover RGB image's color channels. Since grayscale images are single-channel, they occupy less space and are less intrusive when hidden in a colored image.

3. **Text to RGB**
   - **Description**: Embeds text data within an RGB image.
   - **Functionality**: Converts text characters to binary and hides this data within the RGB pixel values of an image. This method is efficient for embedding large text data discreetly.

4. **Text to Grayscale**
   - **Description**: Hides text data inside a grayscale image.
   - **Functionality**: Embeds binary-encoded text characters within the grayscale pixel values, making it suitable for images with simple color palettes.

5. **Audio to RGB**
   - **Description**: Embeds audio data (e.g., `.wav` file) within an RGB image.
   - **Functionality**: Extracts audio wave data and encodes it within the RGB values of the cover image, creating a unique way to store audio data within an image.

## Prerequisites

Ensure the following libraries are installed:

| Library                  | Description                                      | Logo |
|--------------------------|--------------------------------------------------|------|
| `os`                     | Standard Python library for operating system interactions. | ![Python](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg) |
| `numpy`                  | Library for numerical computations in Python.    | ![NumPy](https://upload.wikimedia.org/wikipedia/commons/3/31/NumPy_logo_2020.svg) |
| `wave`                   | Standard Python library for reading and writing WAV files. | ![Python](https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg) |
| `opencv-python (cv2)`    | Library for image processing and computer vision. | ![OpenCV](https://upload.wikimedia.org/wikipedia/commons/3/32/OpenCV_logo_with_text.png) |
| `Pillow (PIL)`           | Library for image handling in Python.           | ![Pillow](https://upload.wikimedia.org/wikipedia/commons/e/e0/Pillow_logo.svg) |

You can install them via:
```bash
pip install numpy opencv-python pillow

