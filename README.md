This script creates a Virtual Painter application that uses a webcam to track hand movements and enables drawing or erasing on a virtual canvas. It leverages OpenCV, Mediapipe, and Tkinter for hand tracking, real-time video processing, and color selection.

Key Features:

1. HAND TRACKING:
Uses MediaPipe Hands to detect and track hand landmarks.

Differentiates between drawing mode (index finger up) and selection mode (index and middle fingers up).



2. DRAWING AND ERASER:

Draw with a brush of adjustable color and thickness.

Erase using a virtual eraser by switching to the "Eraser" tool.



3. COLOR SELECTION:

Offers predefined color choices (red, green, blue).

Includes a custom color picker using Tkinter's askcolor.



4. UNDO/REDO FUNCTIONALITY:

Maintains an undo stack (last 10 states) and a redo stack.

Enables reverting or reapplying changes to the canvas.



5. UI ENHANCEMENTS:

Displays a color palette for tool and color selection.

Icons for eraser and clear canvas options.

Shows FPS and the currently active tool on the screen.



6. PERFORMANCE OPTIMIZATION:

Uses cv2.threshold and bitwise operations to blend the drawing canvas with the live video feed.



7.KEYBOARD SHORTCUTS:

Press q to quit.

Press z for undo, y for redo, and s to save the current canvas state.




MAIN WORKFLOW:

Hand Landmarks: Detect hand gestures and determine if the user is drawing or selecting tools/colors.

Drawing on Canvas: The virtual brush follows the index finger's position, allowing users to draw freehand shapes.

Palette Interaction: Detects hand positions over the palette to change colors, pick custom colors, erase, or clear the canvas.

Undo/Redo: Saves the canvas states for easy undo/redo functionality.


How To Use:

1. Run the script.


2. Use your index and middle fingers to select tools or colors from the palette.


3. Draw on the canvas by moving your index finger.


4. Switch to the eraser by selecting the eraser icon.


5. Clear the canvas, undo, or redo actions as needed.



This implementation combines computer vision with intuitive hand gestures, making it an engaging tool for drawing and creative exploration.

