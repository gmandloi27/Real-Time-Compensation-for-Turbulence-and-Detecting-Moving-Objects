**Real-Time Compensation for Turbulence & Moving Object Detection**

***Overview***

This project processes a video file to:

1. Correct atmospheric turbulence using a sharpening filter.

2. Detect moving objects using background subtraction (MOG2).

3. Visualize results in Jupyter Notebook using Matplotlib.

4. Optionally save processed video output as output.avi.

***Requirements***

Ensure you have the following dependencies installed:

1. pip install opencv-python numpy matplotlib

***Usage***

1. Place Your Video File

Ensure a video file (e.g., video.mp4) is in the same directory as the script.

2. Run the Script in Jupyter Notebook

video_path = "video.mp4"  # Change if needed
process_video(video_path, save_output=True)

3. Output

The original video frames and detected moving objects will be displayed in Jupyter Notebook.

If save_output=True, the corrected video will be saved as output.avi.

***Functionality Details***

1. correct_turbulence(frame)

2. Applies a sharpening filter to enhance image clarity.

3. detect_moving_objects(frame, background_subtractor)

4. Uses cv2.createBackgroundSubtractorMOG2() to detect moving objects.

5. process_video(video_path, save_output=False)

6. Reads video frames, applies processing, and displays results.

7. Saves the output video if save_output=True.

***Notes***

1. The script processes up to 100 frames to prevent long execution in Jupyter.

2. Ensure OpenCV and Matplotlib are installed.

***Author***

*Gaurav Mandloi*
