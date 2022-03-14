# Virtual Keyboard
A simple virtual keyboard created using OpenCV and Python which has 26 alphabets and a space bar.

# What have I done
The secret here is the area of the yellow paper I am wearing on my fingers. When I bring the paper near to the camera, the area of the paper as seen by the camera increases. When it is moved back the, the area of the paper as seen by the camera decreases. This is the simple idea that I have used to detect the click. The position of the click determines the key press that is to be simulated.<br>
The keyboard creation is a bit complicated process. I hope that the code will be able to explain it.

# Requirements
1. PyAutoGui<br>
2. OpenCV 3<br>

# Usage
First run the range-detector.py to set the range for the mask for colour segmentation. The easiest way to use it is to put the yellow paper in front of the camera and then slowly increasing the lower parameters(H_MIN, V_MIN, S_MIN) one by one and then slowly decreasing the upper parameters (H_MAX, V_MAX, S_MAX). When the adjusting has been done you will find that only the yellow paper will have a corresponding white patch and rest of the image will be dark. Then run the virtual_keyboard.py file.

    python3 range-detector.py -f HSV -w
    python3 virtual_keyboard.py

# Got a question?
If you have any questions that are bothering you please contact me on my https://www.linkedin.com/in/nishtha-singh-943b301b0
