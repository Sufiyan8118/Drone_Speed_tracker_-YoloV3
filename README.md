# Drone_Speed_tracker_-YoloV3
Designing a real-time detection and tracking techniques to monitor the trajectory of a high-speed drone as it approaches your location. 
Problem Statement- Designing a real-time detection and tracking techniques to monitor the trajectory of a high-speed drone as it approaches your location. The drone starts its journey from a distance of 2500 metres, positioned at an altitude of 1000 metres, and travels at a velocity ranging from 50 to 75 kilometres per hour. Your duty entails computing the distance between the drone and yourself, as well as ascertaining its velocity. The drone has dimensions of 1 metre in length and 0.5 metres in width, while its height is 1.5 metres.

Hardware Requirements-

Cameras- Multiple high resolution cameras to capture drone.
GPS module- To detect the location of drone.
RADAR unit- To calculate the speed at which drone is approaching us.
High end Computing set up- GPU
Software Requirements-
1)Libraries and Frameworks: OpenCV, TensorFlow/PyTorch, NumPy, Time.

Assumptions- Good weather, Steady wind.
Challenges: Possible environmental elements, such as lighting and weather conditions, might impact the accuracy of detection.

Detection and Tracking Approach-

Object Detection: We will use a pre-trained deep learning model (e.g., YOLO, Faster R-CNN) fine-tuned for drone detection.
Distance Calculation: Use stereo vision (two cameras set apart at a known distance) to estimate the distance to the drone. Alternatively, use RADAR for more accurate distance measurement.
Speed Calculation: Track the drone's position over consecutive frames to calculate its speed using the difference in position over time.
