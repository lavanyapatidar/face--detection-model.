Face Detection (Python)
This small project is a simple way to detect faces in a webcam video using Python tools. The goal is only to understand how image processing works with easy steps.
Problem Definition
Many programs today need a face detection feature, but making a full AI model is too difficult for beginners and requires dedicated GPU. So this project tries to create a basic version of face detection using simple techniques already available in OpenCV. It is not 100% accurate, but it works enough to show how the idea functions.
Requirement Analysis
The program should:
•	open the webcam
•	capture video frames
•	convert the frame to grayscale
•	blur the image to remove noise
•	use the default OpenCV face detector
•	draw boxes around detected faces
•	show CLEAR or ALERT depending on detection
Top Down Design / Modularization
To make everything simple, the project is divided into small parts:
1.	Open and read from the camera
2.	Resize the frame to a fixed width
3.	Convert to grayscale
4.	Apply blur
5.	Run face detection using Haar Cascade
6.	Check basic shape conditions like area and aspect ratio
7.	Draw boxes on the face
8.	Display the result window
Algorithm Development (Short Explanation)
1.	Start program
2.	Load the face cascade file
3.	Open camera
4.	Read frame
5.	Preprocess (gray + blur)
6.	Apply face detection
7.	For each detected face:
o	calculate area and aspect ratio
o	draw box around it
8.	Show ALERT if a face is found
9.	Continue until "q" is pressed
10.	End program
Implementation
This project uses:
•	OpenCV (cv2) for webcam and image actions
•	simple Python code
•	Haar Cascade model which comes with OpenCV
•	if-else conditions and loops
•	basic drawing functions
Testing and Refinement
The program was tested with:
•	normal room lighting
•	different people
•	different distances from the camera
•	small and large faces
Some faces may not get detected depending on:
•	lighting
•	angle of face
•	fast movement
Changing values like scaleFactor or minNeighbors can help improve results.
Expected Outcome
The program will:
•	display webcam window
•	draw green boxes around detected faces
•	show CLEAR when no face is found
•	show ALERT when one or more faces are found
