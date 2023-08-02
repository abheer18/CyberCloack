# Cyber Cloak using OpenCV
This repository contains code for creating a "Cloak of Invisibility" effect using OpenCV. The concept is inspired by the famous invisibility cloak from the Harry Potter series, where a person wrapped in the cloak becomes invisible. In this implementation, we use computer vision techniques to make a selected color range (in this case, green) appear transparent, effectively giving the illusion of invisibility.

## How it Works
The code uses the computer vision library OpenCV to perform the following steps:

Capture the background: Before starting the main video loop, the code captures a single frame from the camera to use it as the background for later processing.

Color Filtering: The program uses trackbars to adjust the upper and lower bounds of the green color range in the HSV color space. This allows you to customize the range of colors to be filtered.

Create a Mask: The selected green color range is then filtered to create a binary mask, where the green color is white (255) and everything else is black (0).

Noise Removal: The mask goes through a series of morphological operations, such as closing and opening, to remove small noise and fill gaps.

Generate the Invisible Effect: The code applies the mask to the stored background to make the selected green color region transparent. It then combines the transparent region with the current frame to give the illusion of invisibility.

## How to Use
Clone the repository to your local machine.

Make sure you have Python and OpenCV installed.

Run the cloak_of_invisibility.py script.

Adjust the trackbars to select the desired green color range for the cloak. You may need to fine-tune the trackbars to get the best results based on your environment.

Stand in front of the camera wearing green clothing (or holding a green object), and you should see the "Cloak of Invisibility" effect in action.

## Additional Notes
It is recommended to use a solid green-colored object for the best results. Avoid wearing clothing or holding objects with colors similar to the background, other colors  can also be used by setting their HSV color code in the color trackbars.

The code may require some adjustments to work optimally in different lighting conditions or with complex backgrounds.

The "Cloak of Invisibility" effect is purely for fun and entertainment purposes. It demonstrates the power of computer vision techniques in manipulating video streams.

Acknowledgments
The code is based on the works of the computer vision community and the OpenCV library. Special thanks to the developers and contributors of OpenCV for providing a powerful and accessible computer vision platform.

Feel free to contribute, modify, or use this code for educational and non-commercial purposes. Happy experimenting and have fun with your own "Cloak of Invisibility"!



