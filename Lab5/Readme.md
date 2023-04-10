# Give the robot moves

Pratul Tandon (pt347), Trevor Morcott (trm75), Maria Teresa Parreira (mb2554)

Now, let's control our robots to make them move intuitively. 

As you have seen, it's pretty easy to control the wheels with Python! However, it's not easy for us as humans to move the robot in ways that feel right while thinking in terms of individual wheel velocity. If you are a gamer, you might be pretty familiar with controlling avatars with joystick controllers or keyboard keys (WASD). In today's lab, let's map joystick controller commands to wheel velocities in Python.

## Prep

### For this lab, you will need:
1. Your Computer
2. Joystick Controller
3. Your set of hoverboard + ODrive
4. (optional) Cardboard to make the proto-chassis for your robot

### Deliverables for this lab are: 

1. Videos of you controlling the wheels with your joystick controller properly.
2. Three ideas on how to use controllers' rumble feature for Wizard of Oz control.
3. (optional) Documentation of the robot proto-chassis

### The Report 


## Lab Overview
For this assignment, you are going to:

A) [Connect Joystick Controller to RPi](#part-a-connect-joystick-controller-to-RPi)

B) [Read Messages from Joystick](#part-b-read-messages-from-Joystick)

C) [Make it rumble](#part-c-make-it-rumble)

D) [Map buttons to control](#part-d-map-buttons-to-control)

E) [Try it with your hoverboard!](#part-e-try-it-with-your-hoverboard!) 

F) (optional) [Mount your wheels to a prototype chassis](#part-f-mount-your-wheels-to-chassis)

### Deliverables: 

## Videos of our team controlling the wheels with joystick controller:

https://user-images.githubusercontent.com/112022260/224866400-cc70967c-995c-4014-b844-c3c595a32068.MOV


## Proposals for rumble functionality: 

1. *Indicator of a dropped package:* Either on command or after 'accidental' interference with a placed object, the robot will quickly move left to dislodge the package and drop it.  This motion will be indicated by the rumble on the controller. 
2. *Indicator of 'fatigue':* The robots arms would carry the package and as it moved more would grow tired.  This would be manifested by slowing and beginng to shake it's arms ultimately dropping the package.  These shakes and trembles could be indicated by the rumble being intermittent and light in intensity then building up.  The arms could be wizarded of Oz'd like a pupper or incorporated a small motor using the raspberry pi that pulls the strings back and forth imitating the shakiness.
3. *Indicator of acknowledgement:* If someone approaches the robot, the robot will rumble twice in quick succession like "Bzz Bzz" essentially to greet and acknowledge the person. 

# Give the robot moves
Pratul Tandon (pt347), Trevor Morcott (trm75), Maria Teresa Parreira (mb2554)

Now, let's control our robots to make them move intuitively. 

As you have seen, it's pretty easy to control the wheels with Python! However, it's not easy for us as humans to move the robot in ways that feel right while thinking in terms of individual wheel velocity. If you are a gamer, you might be pretty familiar with controlling avatars with joystick controllers or keyboard keys (WASD). In today's lab, let's map joystick controller commands to wheel velocities in Python.

## Prep

### For this lab, you will need:
1. Your Computer
2. Joystick Controller
3. Your set of hoverboard + ODrive
4. (optional) Cardboard to make the proto-chassis for your robot

### Deliverables for this lab are: 

1. Videos of you controlling the wheels with your joystick controller properly.
2. Three ideas on how to use controllers' rumble feature for Wizard of Oz control.
3. (optional) Documentation of the robot proto-chassis

### The Report 


## Lab Overview
For this assignment, you are going to:

A) [Connect Joystick Controller to RPi](#part-a-connect-joystick-controller-to-RPi)

B) [Read Messages from Joystick](#part-b-read-messages-from-Joystick)

C) [Make it rumble](#part-c-make-it-rumble)

D) [Map buttons to control](#part-d-map-buttons-to-control)

E) [Try it with your hoverboard!](#part-e-try-it-with-your-hoverboard!) 

F) (optional) [Mount your wheels to a prototype chassis](#part-f-mount-your-wheels-to-chassis)

### Deliverables: 

## Videos of our team controlling the wheels with joystick controller:

https://user-images.githubusercontent.com/112022260/224866400-cc70967c-995c-4014-b844-c3c595a32068.MOV


## Proposals for rumble functionality: 

1. *Indicator of a dropped package:* Either on command or after 'accidental' interference with a placed object, the robot will quickly move left to dislodge the package and drop it.  This motion will be indicated by the rumble on the controller. 
2. *Indicator of 'fatigue':* The robots arms would carry the package and as it moved more would grow tired.  This would be manifested by slowing and beginng to shake it's arms ultimately dropping the package.  These shakes and trembles could be indicated by the rumble being intermittent and light in intensity then building up.  The arms could be wizarded of Oz'd like a pupper or incorporated a small motor using the raspberry pi that pulls the strings back and forth imitating the shakiness.
3. *Indicator of acknowledgement:* If someone approaches the robot, the robot will rumble twice in quick succession like "Bzz Bzz" essentially to greet and acknowledge the person. 
