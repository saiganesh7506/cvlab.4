# Bit Plane Slicing using Python

## Overview
This project demonstrates **bit-plane slicing** on a grayscale image using Python. It displays the original image alongside its eight bit planes (Bit Plane 0 through Bit Plane 7).

Bit-plane slicing separates an 8-bit grayscale image into individual binary images. Each pixel in a bit plane is either 0 or 1; for visualization, the notebook maps these values to black (0) and white (255).

## Tools and Libraries
- Python
- OpenCV (`cv2`) — image loading
- NumPy — pixel/bit operations
- Matplotlib — displaying the original image and bit planes
- Jupyter Notebook / Google Colab

## Notebook Contents
The notebook demonstrates two approaches:

1. **Vectorized extraction:** Uses bitwise shifting and masking (`(img >> i) & 1`) to extract each bit plane.
2. **Manual extraction:** Uses nested loops and arithmetic (`(pixel // (2 ** k)) % 2`) to extract each bit plane.

Both approaches plot the original grayscale image and the eight extracted bit planes.

## Setup

Install the required packages if they are not already available:

```bash
pip install opencv-python numpy matplotlib
```

## Image Input
The notebook currently refers to image files at these paths:
- `/content/cvlab4.jpg`
- `/content/drive/MyDrive/COMPUTER VISION/image16.jpg`

These are Google Colab paths. Upload your image to Colab or update the paths in the notebook to match where your image is stored. The image should be readable by OpenCV; it is loaded as grayscale.

## How to Run
1. Download or clone this repository.
2. Open the `.ipynb` notebook in Jupyter Notebook or Google Colab.
3. Upload the required image, or edit the image path in the relevant code cell.
4. Run the cells in order.
5. View the original image and its eight bit-plane visualizations.

## Expected Output
A figure containing a grayscale original image and eight corresponding bit-plane images, labeled Bit Plane 0 to Bit Plane 7.

## Repository Contents
- `README.md` — project description and run instructions
- `.ipynb` — notebook containing the bit-plane slicing implementation

## output
<img width="1189" height="887" alt="image" src="https://github.com/user-attachments/assets/27eae084-41eb-4d04-b9ff-8819dc200f9b" />

