---

## Angiogram Image Processing with Python

This Python script demonstrates how to process angiogram images using the OpenCV library. Angiogram images are commonly used in medical imaging to visualize blood vessels, particularly in the context of coronary angiography.

### How the Code Works

1. **Importing Libraries**: The code starts by importing the necessary libraries:
   - `cv2` for computer vision operations
   - `numpy` for numerical computations
   - `matplotlib` for image visualization

2. **Class Definition - `AngiogramProcessor`**:
   - The `AngiogramProcessor` class is defined to encapsulate the image processing functionality.
   - It initializes with the path to an angiogram image.

3. **Image Processing Steps**:
   - The `load_image` method loads the angiogram image.
   - The `convert_to_grayscale` method converts the image to grayscale.
   - The `equalize_histogram` method enhances image contrast using histogram equalization.
   - The `smooth_image` method applies Gaussian smoothing to reduce noise.
   - The `threshold_and_process` method creates a binary mask of blood vessels using adaptive thresholding.

4. **Image Visualization**:
   - The `show_original_image` method displays the original angiogram image.
   - The `show_veins_mask` method displays the binary mask of blood vessels.

5. **Connected Component Analysis**:
   - The `keep_connected_components` method retains only the largest connected components in the vessel mask.
   - It uses connected component analysis to identify and keep the significant vessel structures.

6. **Processing and Display**:
   - The `process_and_show` method orchestrates the entire image processing pipeline.
   - It displays both the original image and the processed vessel mask side by side.

7. **Example of Use**:
   - In the provided example, an angiogram image is loaded, processed, and displayed using the `AngiogramProcessor` class.

### Why This Code Is Useful

- This code is useful for medical image processing, particularly in the context of angiography.
- It allows visualization and analysis of blood vessels in angiogram images.
- The code enhances image quality, removes noise, and highlights the vascular structures.

### How to Use This Code

1. Replace `image_path` with the path to your own angiogram image.
2. Customize the processing parameters as needed.
3. Run the script to visualize the original image and the vessel mask.
4. Adjust the threshold and connected component size thresholds for your specific images.
5. Integrate this code into larger projects for automated angiogram analysis.

---
