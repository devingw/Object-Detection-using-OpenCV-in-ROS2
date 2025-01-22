# Object-Detection-using-OpenCV-and-YOLOv3-in-ROS2

## Overview

This code does real-time object detection on a moving robot.

These images visualise the work done by this repository:

<div style="display: flex; justify-content: space-between;">
  <img src="/images/stopsign.png" alt="Image 1" width="40%" />
  <img src="/images/person.png" alt="Image 2" width="40%" />
</div>



## Useful Links

1. YOLO (You Only Look Once). (https://docs.ultralytics.com/)
2. TurtleBot3. (https://emanual.robotis.com/docs/en/platform/turtlebot3/overview/)
3. Rviz2. (https://docs.ros.org/en/rolling/p/rviz2/)

## How it works

This project makes use of the TurtleBot3 robot.

To launch the simulation environment run the following:

```
ros2 launch tortoisebot_bringup simulation.launch.py
```
For the real-time object detection aspect of the project, YOLOv3 ([see link](#useful-links)) has been utilised.

The `src/object_detection` package handles the object detection.

Note that the files relating to the YOLOv3 model used in this project are not available in this repository, however, they must be downloaded for this to work.

### Launching and Testing 

To run the pipeline execute:

```
ros2 run object_detection object_detection_node
```

To move the robot around execute:
```
ros2 run teleop_twist_keyboard teleop_twist_keyboard
```



### Credits

Credits to The Construct for providing a platform to do this.

