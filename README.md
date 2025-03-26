# Maze-Solving-6-DOF-Robotic-Arm
Solved a printed maze lying on a table with laser-mounted end-effector of a robotic arm MyCobot 600 Pro

This project showcases a vision-based robotic arm solving a maze with precision using a custom inverse kinematics solver.

🔹 **Computer Vision & Mapping:** Utilized OpenCV in Python to process live camera feed and applied linear algebra equations to accurately transform coordinates from camera space to robot space.

🔹 **Custom Inverse Kinematics:** Developed a geometric inverse kinematics solver for precise end-effector control, ensuring accurate movement along the maze path. This was achieved by constraining the last two joint angles, which are typically unnecessary for maintaining the end-effector’s downward orientation.

🔹 **Custom URDF Model:** Designed and built a URDF file from scratch to accurately represent the 6-DOF robotic arm, enabling precise simulation and control.
