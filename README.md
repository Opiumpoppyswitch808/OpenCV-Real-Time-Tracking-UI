# Interactive Video Processing and Object Tracking with OpenCV

This project is a hands-on exploration of computer vision and user interface interaction using Python and the OpenCV library. It serves as a practical demonstration of my skills in handling real-time video, processing frames, and implementing interactive controls—key components in many AI and deep learning applications.

-----

## Problem Statement and Goal of Project

The primary goal of this project was to build a series of interactive demonstrations to showcase a strong, practical understanding of the OpenCV library. Rather than focusing on a single high-accuracy model, I aimed to illustrate my ability to work with different facets of computer vision, including:

  * Real-time video capture and processing.
  * User input handling (mouse and keyboard) for interactive applications.
  * Basic object tracking using color segmentation.
  * Building simple graphical user interfaces (GUIs) directly within OpenCV.

This portfolio piece is designed to highlight my foundational skills in computer vision and my approach to exploratory, hands-on learning.

-----

## Solution Approach

I implemented several distinct modules within a Jupyter Notebook to demonstrate various OpenCV functionalities. Each component can be run independently to observe a specific capability.

1.  **Interactive Drawing Canvas:**

      * I created a blank canvas using NumPy and leveraged OpenCV's `namedWindow` and `setMouseCallback` functions to capture mouse events.
      * This allows a user to draw various shapes in real-time, including **circles, lines, rectangles, and free-form ellipses** (simulating a paintbrush).
      * Keyboard input is used to dynamically change the drawing color (by pressing 'r', 'g', or 'b'), demonstrating my ability to create a responsive user experience.

2.  **Color-Based Object Tracking:**

      * To demonstrate object tracking, I implemented a system that processes a live webcam feed.
      * Each frame is converted from the default BGR color space to **HSV (Hue, Saturation, Value)**, which is more robust for color segmentation.
      * I defined a specific color range (for the color blue) and used `cv2.inRange()` to create a binary mask, isolating only the pixels corresponding to the object of interest.
      * This mask is then applied back to the original frame to visually highlight the tracked object.

3.  **UI Controls and Interactivity:**

      * To show my understanding of UI elements, I implemented an **OpenCV trackbar**. This interactive slider allows the user to dynamically adjust the background color of a window, providing immediate visual feedback.
      * I also included an advanced rectangle drawing feature with a "reset" function tied to a right-mouse click, showcasing more complex event handling.

4.  **Video File I/O (Experimental):**

      * The notebook contains sections dedicated to reading video frames from a local `.mp4` file and writing processed frames to a new `.avi` video file. This demonstrates my ability to handle both live and pre-recorded video data.
      * Additionally, I explored using the `yt-dlp` library to fetch and analyze video streams from web URLs like YouTube, showing my initiative in working with diverse and online data sources.

-----

## Technologies & Libraries

  * **Python**
  * **OpenCV (`cv2`)**: The core library for all computer vision tasks, including video I/O, image manipulation, and UI creation.
  * **NumPy**: Used for creating and manipulating the image arrays (canvases and frames).
  * **Matplotlib**: Utilized for displaying images and outputs within the Jupyter Notebook.
  * **yt-dlp (Experimental)**: Explored for downloading video content from the web.

-----

## Description about Dataset

This project does not rely on a formal dataset. The primary data sources are:

  * A **live webcam feed** for real-time object tracking and video processing.
  * Local video files (e.g., `.mp4`) for demonstrating file reading capabilities.
  * Online video streams (e.g., YouTube URLs) for experimental data fetching.

-----

## Installation & Execution Guide

To run this project on your local machine, please follow these steps:

1.  **Clone the repository:**

    ```bash
    git clone <your-repository-url>
    cd <your-repository-name>
    ```

2.  **Create a virtual environment (recommended):**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the required libraries:**
    A `requirements.txt` file should be created with the following content:

    ```
    opencv-python
    numpy
    matplotlib
    yt-dlp
    ```

    Then, run:

    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Jupyter Notebook:**

    ```bash
    jupyter notebook write_read_video_ui_track.ipynb
    ```

    Execute the cells sequentially to see each demonstration. *Note: The interactive cells will open a separate OpenCV window.*

-----

## Key Results / Performance

As this is a skills-demonstration project, the key results are the successful implementations of the various interactive features:

  * A fully functional interactive paint application allowing users to draw different shapes and lines with color selection.
  * A real-time object tracker capable of identifying and isolating blue objects from a live webcam feed.
  * An interactive window with a trackbar for dynamically changing visual properties.
  * Successful demonstration of reading from and writing to video files, showcasing data handling capabilities.
-----

## Additional Learnings / Reflections

This project was a valuable exercise in deepening my understanding of OpenCV's rich feature set beyond simple image loading and filtering. Implementing the interactive drawing and tracking functionalities from scratch reinforced my understanding of event-driven programming and real-time data flow.

The sections on video I/O and experimenting with `yt-dlp` were intentionally included to demonstrate my curiosity and willingness to explore different data sources, even if they aren't fully polished models. I believe this shows a capacity for independent learning and a proactive approach to solving practical computer vision challenges.

-----

## 🙏 Acknowledgments

This project represents my initial steps into the practical application of computer vision. The foundational knowledge and guidance for this work were derived from the outstanding OpenCV course taught by **Alireza Akhavanpour** on the **Maktabkhooneh** platform. His ability to deconstruct complex topics into clear, actionable steps was instrumental in the successful implementation of this project.
-----

## 👤 Author

## Mehran Asgari

## **Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com).

## **GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari).

-----

## 📄 License

This project is licensed under the Apache 2.0 License – see the `LICENSE` file for details.

-----

💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*
