## MuJoCo mini project

**Goal**: Inside simulation environment, locate and track down the 3D coordinates of a floating ball, then have the robot arm reach toward the ball's position.

**Method Description**: Use YOLOWorld, a text-conditioned object detection model, on two cameras to locate a floating ball in MuJoCo simulation environment. This ball's world coordinate, computed by triangulation, is used to guide the movement of the robot arm. The movement is computed using Inverse Kinematics.

**Installation**: 

Download YOLO World weights and place at `yolo_world/yolov8s-worldv2.pt`, or let `ultralytics` auto-download by running the notebook once with an internet connection. The project was developed on Python 3.13.5.
```
pip install -e
```
All codes are in ```main.ipynb```.
## Final Visualization

https://github.com/user-attachments/assets/01cb8182-204f-4c36-8192-18bb07ee4831

https://github.com/user-attachments/assets/87473e5e-2e9c-4fa5-a076-1b6484dae4e5


## Acknowledgment

The robot arm .xml files, the code skeleton, and some code snippets were taken from [HaoxiangYou/MujocoTutorialsTutorials](https://github.com/HaoxiangYou/MujocoTutorials/). Claude assists in getting cameras' intrinsics and extrinsics.

