 # MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

Step1: 
 Take the Ep core robot insert the battery and check the battery percentage 

<br/>

Step2: Turn on the robot and connect the robot to the computer through WIFI 

<br/>

Step3: Open visual studio and import robomaster package and do all the code 

<br/>

Step4: Take the measurment of the track on each and every turn and gives the valuse through code in (m)

<br/>

Step5: run the program to see the robot movement 

<br/>

## Program
### Code For Robot Movement
```python
import time
from robomaster import camera
if _name=='__main_':
    ep_robot=robot.Robot()
    ep_robot.initialize(conn_type='ap')

    ep_chassis= ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera= ep_robot.camera

    print('video streaming started ...')
    ep_camera.start_video_stream(display=True,resolution= camera.STREAM_360P)


    ep_chassis.move(x=2.4,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0.5,y=0,z=80,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=1,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0,y=0,z=90).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.3,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")
    
    ep_chassis.move(x=0,y=0,z=-28,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=255,effect="on")

    ep_chassis.move(x=1.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=255,effect="on")
    
    ep_chassis.move(x=0,y=0,z=36).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=1.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=204,effect="on")

    ep_chassis.move(x=0,y=0,z=98).wait_for_completed()
    ep_led.set_led(comp = "all",r=204,g=225,b=255,effect="on")

    ep_chassis.move(x=2.04,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=204,effect="on")

    ep_chassis.move(x=0,y=0,z=85).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0.5,y=0,z=0,xy_speed=1.3).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=128,b=128,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![robomaster](https://github.com/Kishorerz/mobilerobot-openloopcontrol/assets/144451216/4ad4ef18-0271-4b26-8614-5d57fdea53a4)
![vlcsnap-2023-12-22-01h15m56s442](https://github.com/Kishorerz/mobilerobot-openloopcontrol/assets/144451216/ec03b6c7-db70-4459-9915-0bfa5314ee36)
![vlcsnap-2023-12-22-01h16m11s696](https://github.com/Kishorerz/mobilerobot-openloopcontrol/assets/144451216/47d7e6aa-9d4a-4992-9aa1-a73cf219a438)

![vlcsnap-2023-12-22-01h16m53s968](https://github.com/Kishorerz/mobilerobot-openloopcontrol/assets/144451216/3db07203-bef9-430a-bce7-4b1dde56d480)

<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:

Upload your video in Youtube and paste your video-id here

(![robomaster](https://github.com/akash7812/mobilerobot-openloopcontrol/assets/146819826/3842c86a-ac11-4522-948f-5a3ee32901c3)
(https://youtu.be/NmZDwi1Hzgs?si=EiUi7BLM7sTR43-t)


<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


<br/>
<br/>

```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```

