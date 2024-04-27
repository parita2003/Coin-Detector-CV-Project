# Coins Detector

This Jupyter notebook (`coins_detector.ipynb`) is used to detect and classify coins in an image. It utilizes computer vision techniques to identify different coins based on their sizes and shapes.

## How the Detection Works

1. **Image Preprocessing:** 
   - The input image is loaded and converted to grayscale for easier processing.
   - A median blur is applied to reduce noise in the image.

2. **Thresholding:** 
   - Otsu's thresholding is used to binarize the image, separating the coins from the background.
   - A second thresholding step is applied to refine the binarization.

3. **Contour Detection:**
   - Contours are found in the binarized image, representing the boundaries of the coins.

4. **Coin Classification:**
   - For each contour:
     - The minimum enclosing circle is calculated to get the radius and center.
     - Based on the area of the circle, coins are classified into different denominations (e.g., 500, 100, 50, 10, 5, 1).

5. **Visualization:** 
   - The detected coins are overlaid on the original image, along with their denominations.

## Dependencies

- OpenCV (`cv2`)
- NumPy
- Matplotlib

## How to Use

1. Ensure you have the necessary libraries installed.
2. Run each cell in the notebook sequentially.
3. The final output will display the original image with overlaid detected coins and their denominations.

## Result

![image](https://github.com/parita2003/Coin-Detector-CV-Project/assets/126491686/fb93b504-1d2b-492e-b09d-cca9e9011647)


