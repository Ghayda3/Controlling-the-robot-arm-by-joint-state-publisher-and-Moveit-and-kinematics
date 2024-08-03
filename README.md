# Controlling-the-robot-arm-by-joint-state-publisher-and-Moveit-and-kinematics

## Step 1: Create a ROS (Catkin) workspace 
with the command: "mkdir catkin_ws"
### then you can enter the new folder using the command: 
"cd catkin_ws"
### then we are going to create a source (make sure it it exactly src inside thr catkin work space):
"mkdir src"
### now make sure that you are inside the catkin_ws folder (not inside the src folder) then we can start to compile by running the command: 
"catkin_make"

![1](https://github.com/user-attachments/assets/6a3cfb51-1dee-452d-a180-bf6efc754268)
#
 
now if we run the command ls we see that we have two new folders (build and devel)

![2](https://github.com/user-attachments/assets/a5f441f0-ee9f-44e2-b9bf-f27a523cffb1)
#

#Installing the package arduino_robot_arm
### Add the “arduino_robot_arm” package to “src” folder cd src then copy this command: 
"sudo apt install git"

![3](https://github.com/user-attachments/assets/c185448b-fd8c-45d2-b7b8-57a4e4c86756)
#

### git clone https://github.com/smart-methods/arduino_robot_arm 

![4](https://github.com/user-attachments/assets/a614edf7-f6c0-437d-a771-392ba92b9038)
#

### run the command: 
"sudo apt-get install ros-noetic-moveit"

![5](https://github.com/user-attachments/assets/2d04cb84-8536-4999-89b3-edbd5bf8a935)
#

### run the command: 
"sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui"

![6](https://github.com/user-attachments/assets/f2f2121c-c949-4b33-97e2-0cf19c22fc6e)
#

### run the command: 
"sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher"

![7](https://github.com/user-attachments/assets/55717512-0b42-443b-97a9-c1f557d75dd9)
#

### run the command: 
"sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control"

![8](https://github.com/user-attachments/assets/6da8b6a8-0590-471d-8c63-bc6777210261)
#

### compile the package: 
"catkin_make"

![9](https://github.com/user-attachments/assets/9936303c-3b1b-40ea-9175-01c6cf150699)
#

## Step 2: Controlling the motors
#

### now we can control the motors by this commend: 
"roslaunch robot_arm_pkg check_motors.launch"

when you run this command the widows will apears

![10](https://github.com/user-attachments/assets/41e46d26-2a79-41ef-9240-812d9fd3dd5a)
#

### You can move it

![11](https://github.com/user-attachments/assets/4bf6ff93-05d8-4342-b454-278d9be069a6)
#

## Step 3: Gazebo
### run the command: 
"roslaunch robot_arm_pkg check_motors_gazebo.launch"

![12](https://github.com/user-attachments/assets/c316fe79-1130-4057-b0e4-464a0e7b1e05)
#

## Step 4: MoveIt controlling

### run the command: 
"roslaunch moveit_pkg demo.launch"

![13](https://github.com/user-attachments/assets/919ce3bd-2c22-4bb9-95ff-f915acc48660)
