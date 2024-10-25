# Seam-Carving

Introduction

Seam carving is a content-aware image resizing technique that reduces the size of an image by removing seams of pixels with the lowest energy. This technique helps preserve the most important features of the image while resizing.
Features

Features

    Energy Calculation: Computes the energy of each pixel in the image, enabling effective seam identification.
    Seam Identification: Identifies the seam (path of pixels) with the lowest energy to minimize distortion.
    Seam Removal: Removes the identified seam from the image to achieve the desired dimensions.
    Resizing: Continuously removes seams until the image reaches the specified size.
    User Input: Allows users to specify the desired width or height for resizing.
    Multiple Energy Functions: Supports different methods for calculating energy, such as gradient magnitude and color histograms.

Demonstration

Before and after images showcasing the seam carving effect.

Vertical Seam Removal

![image](https://github.com/user-attachments/assets/a5fd7851-9a96-49bb-a0a9-60b8972aff66)


![image](https://github.com/user-attachments/assets/c4277ee1-de84-40f8-8e04-36216566b1d8)


Horizontal Seam Removal

![image](https://github.com/user-attachments/assets/1420848c-34c3-48de-a5de-2cad5600bb8d)

![image](https://github.com/user-attachments/assets/becca250-4f0c-4b67-be7d-e3f1f1896741)


Requirements

    OpenCV: Used for image processing tasks such as extracting and generating images.
    Python or C++: For implementing the seam carving algorithm.
    No C++ STL: The implementation must avoid using the C++ Standard Template Library (STL).

Usage Instructions

    Clone the repository:

    bash

git clone https://github.com/Archit-10/Image_Resizing_using_Seam_Carving_Algorithm.git
cd Image_Resizing_using_Seam_Carving_Algorithm

Install the required dependencies:

bash

pip install opencv-python  # For Python users

Run the algorithm:

bash

    python seam_carving.py --input path/to/image.jpg --output path/to/resized_image.jpg --new_width 300

Performance Metrics

    Time Complexity: O(NM) for finding the optimal seam, where N is the height and M is the width of the image.
    Memory Usage: Memory usage is proportional to the size of the image, as additional space is required for energy and cost matrices.

Challenges Faced

During development, I encountered challenges with seam identification in images with complex patterns. To address this, I implemented multiple energy functions to improve accuracy.
Future Improvements

    Optimize performance for larger images using parallel processing.
    Extend the algorithm to handle video resizing.
    Implement an interactive GUI for real-time resizing.

Testing

The implementation includes unit tests to validate the correctness of the energy calculation and seam removal processes. Performance benchmarks have been conducted to assess the algorithm's efficiency.
Tech Stack

    Programming Language: Python / C++
    Libraries: OpenCV

Contributions

Contributions are welcome! If you'd like to contribute to this project, please follow these guidelines:

    Fork the repository.
    Create a new branch for your feature or bug fix.
    Submit a pull request detailing your changes.    



