# Waste-Classifier

This script demonstrates a waste classification model using computer vision techniques. The model is designed to classify different types of waste into specific categories, such as recyclable, hazardous, food waste, and residual waste. The waste classification is performed in real-time using a webcam feed.

Here's how the script works:

Importing Libraries and Resources: The script imports the necessary libraries, including cvzone for overlaying images and cv2 for image processing. It also loads the waste images and bin images from the specified directories.

Initializing the Webcam and Classifier: The script initializes the webcam using OpenCV's VideoCapture function and creates an instance of the Classifier class, which loads a pre-trained waste classification model and its corresponding label file.

Overlaying Images: Within the main loop, the script captures frames from the webcam feed and resizes them. It then overlays the resized frame onto a background image, which serves as the display window. The overlay includes images of the waste items and bins based on the classification results.

Waste Classification and Bin Selection: The script uses the Classifier class to predict the waste category from the captured frame. The classID obtained from the prediction is used to select the appropriate waste image and bin image for overlaying onto the background image. The classDic dictionary maps the waste categories to the corresponding bin categories.

Displaying the Output: The resulting background image, with the waste and bin overlays, is displayed in a separate window using OpenCV's imshow function. The image is continuously updated in real-time.

By running this script and pointing the webcam towards waste items, you can observe the classification results and see the appropriate bin image overlayed on the display. This model can be a useful tool in waste management and recycling processes, aiding in the efficient sorting and disposal of different types of waste.
