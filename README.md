# Car-out-

A Python-based application for counting cars in video streams using OpenCV.

## Architecture Overview

The `Car-out-` repository is structured to perform real-time car detection and counting from a video file. The core functionality is encapsulated within the `cars_counter.py` script, which leverages OpenCV for video processing and contour analysis. The application uses Haar cascades for object detection and processes each frame to identify and count cars.

- **cars_counter.py**: The main Python script that handles video capture, frame processing, car detection, and counting.
- **haarcascade_cars.xml**: A pre-trained Haar cascade classifier for detecting cars in images.
- **video.mp4**: An example video file used for testing the car counting functionality.

## Tech Stack

- **Programming Language**: Python
- **Libraries/Frameworks**:
  - OpenCV (`cv2`): For video capture, image processing, and contour detection.
  - NumPy: For numerical operations on arrays and matrices.

## Getting Started / Setup Guide

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/car-out-.git
   cd car-out-
   ```

2. **Install Dependencies**

   Ensure you have Python installed, then install the required libraries:

   ```bash
   pip install opencv-python numpy
   ```

3. **Run the Application**

   Execute the `cars_counter.py` script to start counting cars in the provided video file:

   ```bash
   python cars_counter.py
   ```

4. **Customization**

   - To use a different video file, replace `'video.mp4'` with your desired video path in the `cars_counter.py` script.
   - Adjust parameters such as `min_contour_width`, `min_contour_height`, and `offset` to fine-tune car detection accuracy based on your specific use case.

## Notes

- The application is designed for counting cars in static environments. For dynamic or complex scenes, further enhancements may be required.
- Ensure the video file path is correct and accessible by the script to avoid runtime errors.