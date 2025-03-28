# Live Sketch App using OpenCV and NumPy

## Project Overview

This project is a real-time sketch generator that transforms live video feed from your webcam into a pencil-like sketch using computer vision techniques. Built with Python, it leverages the power of OpenCV for image processing and NumPy for efficient array operations. The application processes each frame of the video in real-time, applying a series of transformations—sharpening, grayscale conversion, inversion, and Gaussian blurring—to create a sketch effect.

## Features

** Real-Time Processing **: Converts live webcam feed into a sketch instantly.

** Custom Image Processing Pipeline **: Includes sharpening with a custom kernel, grayscale conversion, and Gaussian blur for a smooth sketch effect.

** Dual Display **: Shows both the original video feed and the sketch side-by-side.

** Interactive Exit **: Press 'q' to stop the application gracefully.

## Technologies Used

** Python **: Core programming language.

** OpenCV **: For capturing video and applying image processing techniques.

** NumPy **: For efficient manipulation of image arrays.

** Matplotlib **: Imported for potential visualization (optional extension).

## How It Works

** Video Capture **: Uses cv2.VideoCapture(0) to access the webcam feed.

** Frame Processing **:

- Resizes the frame to maintain aspect ratio.

- Applies a sharpening filter using a custom 3x3 kernel to enhance edges.

- Converts the image to grayscale and inverts it.

- Applies Gaussian blur to smooth the inverted image.

- Combines the grayscale and blurred images to produce the final sketch.

** Display **: Shows the live sketch and original feed using cv2.imshow().

** Exit **: Releases the camera and closes windows when 'q' is pressed.