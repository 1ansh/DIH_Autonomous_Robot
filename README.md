# Autonomous_Robot
*Abstract:*
We aim to design a self-driving robot that will run on the
track detecting traffic lights, stop sign along with collision
avoidance system. We may use Image Processing Techniques
to extract the data obtained using a Camera.
Lane detection techniques are being used for the traversal of
robot. For this purpose, Image processing is being used
which after being processed, return the commands to run
the robot accordingly.

*System Design:*
The system consists of three subsystems:
•Input Unit Camera Ultrasonic Sensors Raspberry Pi Board Arduino Board
•Processing Unit Computer
•Control Unit Fire Bird V Robot

*Object Detection:*
This project adapted the shape-based approach and used 
Haar feature-based cascade classifiers for object detection. 
Since each object requires its own classifier and follows the
same process in training and detection, this project only focused
on stop sign and traffic light detection.
This project extensively uses computer vision and that is achieved
with the help of OpenCV. OpenCV is a library of programming functions
for Computer vision. This project uses OpenCV for two different approaches.
Firstly, for object detection (with the help of Haar-cascade classifiers) and
secondly, for distance measurement.

*Obstacle Detection:*
The obstacle detection is an important requirement of this autonomous RC Car.
In this project, the Car gets the information from surrounding area through the
mounted ultrasonic sensors. Ultrasonic sensor transmits the ultrasonic waves from
its sensor head and again receives the ultrasonic waves reflected from an object.
Ultrasonic sensor is most suitable for obstacle detection and it is of low cost and
has high ranging capability.

*Robot’s Locomotion:*
With the help of lane detection, we can get the gradient of lane and by as a relation
we can get the direction of motion. Now we will pass a character(corresponding to the direction)
to the robot.
The robot, after receiving the character will move accordingly.
Simultaneous processing of stop sign detection, traffic light detection and obstacle detection 
will also be performed. The robot will move taking all processes into consideration and will 
show the results when required.
