# Choreographing Movement

Pratul Tandon (pt347), Trevor Morcott (trm75), Maria Teresa Parreira (mb2554)

It is about time to have a functioning mobile robot! Starting from this lab, you should prioritize either robot building and/or study design.

## Prep
### Watch the following tutorials:
- [How to crimp wires](https://www.youtube.com/watch?v=SaU00MMjzn0&ab_channel=GrizzlyBuilds)

- [Beginner's Guide on Soldering](https://www.makerspaces.com/how-to-solder/)


- [How to Solder Wires Together](https://youtu.be/NSqPHQ1zQco)



### For this lab, you will need:
1. Your laptop
2. Cardboard
3. Utility knife
4. Your hoverboard base

### Deliverables for this lab are:

0. Photos of your robot prototype
1. A video of your robot moving around
2. A sketch of a series movements based on your final project
3. A video showing your robot perform the movements in item #2.
4. Reflect upon your design, what would you do differently?


## Lab Overview
For this assignment, you are going to:

A) [Build your chassis](#part-a-build-your-chassis)

B) [Move it around](#part-b-move-it-around)

C) [Plan a movement](#part-c-plan-a-movement)

D) [Optional Spinning your LiDAR](#part-d-optional-spinning-your-LiDAR)

Labs are due on Tuesdays before class. Make sure this page is linked to on your main class hub page.

## Part A. Build your chassis
If you haven't already, now is a good time to actually mockup a low fidelity version robot for your final project. At least, you should have a chassis that safely host all the hardware you have (ODrive, wheels, battery, etc).

Feel free to use any material we have in lab to build your chassis. Things you might find useful are cardboard, gluegun, zip ties, duo locks, etc.

## Part B. Move it around
Once you build your chassis, test it out! Power on your hoverboard and connect your controller. Drive your robot around! (Take a video while you do that!)

A few questions to consider:
- when your robot accelerate, is the chassis stable?
- what are all the possible motions (action space) your robot can perform? (e.g. rotating in place, moving foward/backward, ...)
- reflect on your design and think what would you do differently next time.

## Part C. Plan a movement
Based on your scenario, sketch out a sequence of movement in a storyboard format.
Then, control your robot to execute that sequence of movement. (Take a video while you do that!)


## Part D. Optional spinning your LiDAR
If you plan to use LiDAR for your final project, or are simply curious about how it works, let's set it up!

```
# Install LiDAR SDK
# In your RPi terminal
sudo apt install cmake pkg-config
cd ~
git clone https://github.com/YDLIDAR/YDLidar-SDK.git
cd YDLidar-SDK
mkdir build
cd build
cmake ..
make
sudo make install
```

```
cd ~/mobilehri_ws/src/mobilehri2023
git checkout ydlidar_ros2_driver
cd ~/mobilehri_ws
colcon build

chmod 0777 src/ydlidar_ros2_driver/startup/*
sudo sh src/ydlidar_ros2_driver/startup/initenv.sh

```
Now, plug in your LiDAR.
```
# start your LiDAR
source install setup.bash
ros2 launch ydlidar_ros2_driver ydlidar_launch.py
```

To visualize your LiDAR reading, open foxglove studio in vnc viewer. Then, click 3D in the left panel.

### Again, deliverables for this lab are:

0. Photos of your robot prototype
1. A video of your robot moving around

https://user-images.githubusercontent.com/62056130/226578749-254951e4-9c08-4a73-a72d-0ea4f99b5582.MOV



https://user-images.githubusercontent.com/62056130/228691598-1f682a38-d69c-4e7d-a432-fffcb24e855d.MOV



2. A sketch of a series movements based on your final project

![CamScanner 03-21-2023 11 05](https://user-images.githubusercontent.com/62056130/226578561-a3961db8-a3f3-4331-94df-c88dc0366a10.jpg)


3. A video showing your robot perform the movements in 2.

https://user-images.githubusercontent.com/62056130/226578509-11362788-3a12-4734-b3ba-de9e67f347f3.MOV


4. Reflect upon your design, what would you do differently?

* In order to have a package carrying robot, we need a stable base. We want a wide base but also some height, so we will have to think how to best do this with an external design that does not stand out too much from the environment where we plan to deploy the robot

* We still need to work on motion control, it reacts rather abruptly. This might lead to unwanted falls; options could be add some filter for a smoother transition from stop to motion (but not the other way around, as we want to cause a fall - so, we need a sudden stop when in motion)

* Similarly, we need to build a base to isolate the metal from the chassis.

* We also need to ensure that the hardware can be placed on the robot (raspberry pi but also camera/microphone etc, for data collection)

* LiDAR is an interesting data collection method, particularly for automatic navigation, but we should not need it as we are planning to wizard-of-oz our robot while running the studies

* Generally on robot design, we will reconsider the anthropomorphic look of the robot

* We need to ensure that we signal “oh the robot is struggling” through non-verbal robot comunication/robot motion. This means we will probably have to fine-tune this motion a little in order to ensure that the users perceive the message appropriately. For now, we just have to make sure we can adjust motion speed and direction, to ensure we can make changes to the movement easily when running pilot studies.





