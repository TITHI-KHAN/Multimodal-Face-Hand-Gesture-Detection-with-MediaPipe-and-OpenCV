# Multimodal Face, Hand Gesture Detection with MediaPipe and OpenCV

## To run the code, please either use "Visual Studio" or "Jupyter Notebook from Anaconda Navigator".

### For the project video, please check the "Project Video" file. Thank you.

<br>

## Code Explanation:

This Python script demonstrates real-time detection of both face and hand gestures using OpenCV and MediaPipe. Here's a step-by-step explanation:

**1.** Import necessary libraries:
   - `cv2`: OpenCV library for computer vision tasks.
   - `mediapipe as mp`: MediaPipe library for hand gesture detection.
   
**2.** Initialize the MediaPipe hands module and the drawing utilities.

**3.** Define a function `detect_face(frame)` to detect faces in the input frame using the Haar Cascade classifier for face detection. It draws rectangles around detected faces.

**4.** Define a function `detect_hand(frame)` to detect hand gestures in the input frame using the MediaPipe hands module. It draws landmarks and connections on detected hands.

**5.** Define the main function `main()`:
   - Initialize a video capture object from the default camera.
   - Start a loop to continuously capture frames from the camera.
   - Read a frame from the video capture object.
   - Detect face in the frame using `detect_face()` function.
   - Detect hand gestures in the frame using `detect_hand()` function.
   - Display the frame with face and hand detections.
   - Break the loop when 'q' is pressed.
   - Release the video capture object and destroy any OpenCV windows.

**6.** Call the `main()` function when the script is executed.

## Key Points:
- The script utilizes the MediaPipe library for hand gesture detection and OpenCV for face detection.
- It demonstrates real-time detection of both face and hand gestures simultaneously.
- Face detection is performed using the Haar Cascade classifier, while hand gesture detection is done using the MediaPipe hands module.
- Detected faces are highlighted with rectangles, and hand landmarks and connections are drawn on detected hands.
- The script captures frames from the default camera, processes them for face and hand detection, and displays the results in real-time.
