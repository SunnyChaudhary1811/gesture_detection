Gesture Detection in Videos

This project implements gesture detection in videos using background subtraction.

Requirements:

Python 3.x
OpenCV-python (Install using pip install opencv-python)
NumPy (Install using pip install numpy)
Usage:

Place your test video (test_video.mp4) in the same directory as this script (detect_gesture_background_subtraction.py).
Modify the file path in the script if needed (refer to test_video_path and output_video_path variables).
Run the script using python detect_gesture_background_subtraction.py.
Output:

The script will generate an output video (output_video.avi) with bounding boxes and "DETECTED" annotations around potential gestures identified in the video.

How it Works:

The script uses background subtraction to isolate moving objects from the background.
It assumes the largest contour in the foreground mask represents the hand or gesture.
A bounding box is drawn around the largest contour, and "DETECTED" is displayed to indicate a potential gesture.
Limitations:

This approach might not be perfect for complex gestures or videos with cluttered backgrounds.
It relies on the hand being the most prominent moving object in the foreground.
Further Improvements:

Could explore different background subtraction algorithms or parameters for better results in specific scenarios.
Consider combining this approach with color segmentation for the hand region if the background is static and the hand color is distinct.


Used google gemini and chatgpt to improve code