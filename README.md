# Robotic-Hand-With-6-DOF
<img src="https://github.com/AHMRezaul/Robotic-Hand-With-6-DOF/blob/main/roboticArm.png"  width="100" height="100" />

## Overview
A robotic hand built using servo motors and arduino as the main components with a steel frame. It can be used to perform basic hand movements that can lift a small object.
One of the motors is used to grab the object with a gripper. Another motor is used to move the arm up and down while a third motor is used to move the motor sideways. 
The arm can be controlled using a remote controller application from any computing device. Alternatively, the arm can be automated and will keep performing a given task as long as
no new instructions are given.

## Procedure
In the terminal enter "python armControl.py". This will open up a GUI window where you give inputs and output angles are calculated.
Inverse Kinematics is calculated in the file invKin.py. It is called by armControl.py. Arm control has a GUI that can be used to control X Y Z roll pitch yaw. To see whether the output of the Inverse Kinematics is correct, a live Matplotlib 3d graph is used. invKin.py has functions forwardKinematics() and getAngles() and some other helper functions. Given, the joint angles q1, q2, q3, q4 q5 and q6, forwardKinematics() calculates the joint coordinates along with the end effector's coordinates. This helps us to draw the arm in matplotlib. Matplotlib window automatically pop up when you run armControl.py.

## Some instructions
```
python armControl.py 
```
A GUI having control of X,Y,Z,roll,pitch,yaw will be initiated. A matplotlib window will be initiated. Play with GUI buttons to see inverse kinematics in action.
![](https://github.com/AHMRezaul/Robotic-Hand-With-6-DOF/blob/main/1.png)
![](https://github.com/AHMRezaul/Robotic-Hand-With-6-DOF/blob/main/2.png)
![](https://github.com/AHMRezaul/Robotic-Hand-With-6-DOF/blob/main/3.png)

## Demo Video
A demo video of the robot hand in work can been seen here: https://github.com/AHMRezaul/Robotic-Hand-With-6-DOF/blob/main/robothand.mp4
