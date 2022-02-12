# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1:
Use from robomaster import robot.

Step2:
Choose the x,y,z - axis movement distance(meters).

Step3:
Give ep_chassis.move to move straight.

Step4:
Give time.sleep() for a break.

Step5:
Give ep_chassis.drive_speed to have a circular movement.

## Program
```
##Developed by: Anusha R
##Register number:212221230006

from robomaster import robot
import time

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis

    ep_chassis.move(x=2, y=0, z=0, xy_speed=14).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=90, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=2, y=0, z=0, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=90, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=2, y=0, z=0, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=90, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=2, y=0, z=0, xy_speed=4).wait_for_completed()

    ep_chassis.move(x=0, y=0, z=90, xy_speed=4).wait_for_completed()

   

    ep_robot.close()
```

## MobileRobot Movement Image:

![robo](./mb.jpeg)

## MobileRobot Movement Video:

https://youtube.com/shorts/P3YG3rxl1Zw?feature=share


## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.



```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
