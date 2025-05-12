# Maze Solving-6-DOF-Robotic-Arm
Solved a printed maze lying on a table with laser-mounted end-effector of a robotic arm MyCobot 600 Pro

**Video Link**: [Video link](https://youtu.be/8pNSNreSBco)

![Maze_Solving](https://raw.githubusercontent.com/Sjschhabra/Maze-Solving-6-DOF-Robotic-Arm/refs/heads/main/media/Screenshot%202025-04-01%20150416.png)
![Robot](https://raw.githubusercontent.com/Sjschhabra/Maze-Solving-6-DOF-Robotic-Arm/refs/heads/main/media/Screenshot%202025-03-12%20184611.png)

This project showcases a vision-based robotic arm solving a maze with precision using a custom inverse kinematics solver.

🔹 **Computer Vision & Mapping:** Utilized OpenCV in Python to process live camera feed and applied linear algebra equations to accurately transform coordinates from camera space to robot space.
The custom transformation function to get the vector V connecting the robot origin to the point under camera is:

          𝑉 = 𝑂 + 𝑐 ⋅ 𝑅 ⋅ 𝑣

  where,
  O (Vector): Translation from the robot origin to the camera origin.
  R (Square Matrix): Rotation matrix aligning the camera frame with the robot frame.
  c (constant): Scaling factor to convert pixel coordinates to real-world units.
  v (Vector): Point in camera space.


🔹 **Custom Inverse Kinematics:** Developed a geometric inverse kinematics solver for precise end-effector control, ensuring accurate movement along the maze path. This was achieved by constraining the last two joint angles, which are typically unnecessary for maintaining the end-effector’s downward orientation.

🔹 **Custom URDF Model:** Designed and built a URDF file from scratch to accurately represent the 6-DOF robotic arm, enabling precise simulation and control.
