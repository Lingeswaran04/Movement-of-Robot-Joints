# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```python
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot
![WhatsApp Image 2023-11-07 at 08 13 46_eb317ea6](https://github.com/Lingeswaran04/Movement-of-Robot-Joints/assets/119103865/aa392712-2565-4e08-8ebe-4202a9072ff2)


### 2. robot.driveJoints(0,0,0,0,0,0)
![image](https://github.com/Lingeswaran04/Movement-of-Robot-Joints/assets/119103865/7a609aec-cfe0-4b27-ac44-ffad03c4d9eb)


### 3. Movement of Joint1
![image](https://github.com/Lingeswaran04/Movement-of-Robot-Joints/assets/119103865/d16689e1-7213-4635-b956-19df1dfd856d)


### 3. Movement of Joint2
![image](https://github.com/Lingeswaran04/Movement-of-Robot-Joints/assets/119103865/23d70445-7b77-4ea2-a574-a2face030415)


### 3. Movement of Joint3
![image](https://github.com/Lingeswaran04/Movement-of-Robot-Joints/assets/119103865/9115dfe8-3ff9-4d2a-9f8f-ded43652038f)

## Result 
Thus the different robots joints are moved with the help of python list.


