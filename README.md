# Eye-Tracking
Meant for reporting L/R gazes; specifically developed considering online proctoring 

You need to have yolov3.weight and DLib's 68_face_landmark.dat file in the same folder to run the code.

Process:
1. Using DLib extract our ROI(both eyes)
2. Apply a whitening vignette to offset the the eye shadows.
3. Use minmaxloc to identify the brightest portion of ROI which will be the white portion of our eye. The movement of this point helps track gazes.

The code can only identify a gaze but not it's direction.
