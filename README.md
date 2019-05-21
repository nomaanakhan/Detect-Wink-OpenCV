# Detect-Wink-OpenCV
This project detects winks in pictures or live videos.

In DetectWink1 I use OpenCV's Haar feature-based cascade classifiers to detect faces and once a face is detected if only eye detected on that face then infer that the person is winking.

DetectWink2 is the same but it performs histogram equalization on the picture before making any detections

For my approach I modified the cascade detection values for eyes to be larger. If no eyes are detected in the picture, then I use smaller values for eyes. I also modified the scale factor to 1.15. 

DetectWink1 detects 22 winks on the sample pictures.

DetectWink2 detects 15 winks on the sample pictures.

### To Run

On Pictures \n
python DetectWink1 folder_name 

On a User's Camera Video \n
python DetectWink1
