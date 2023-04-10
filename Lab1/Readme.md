# Interaction First
\*\***Pratul Tandon (pt347), Trevor Morcott (trm75), Maria Teresa Parreira (mb2554)**\*\*

In this lab, you will modify a robotic creature (ConeBot) that is originally designed by [Dr. Rei Lee](https://infosci.cornell.edu/~reilee/), a friend of our lab. The [ConeBot](https://infosci.cornell.edu/~reilee/ConeBot/) is a shy robot that hides under a small traffic cone. It is adventuring the world by itself but hopes people don't notice it at all.

Today, you will work with a close relative of ConeBot, CloneBot. Though closely related, CloneBot's personality (robotality?) is quite the opposite of ConeBot. It is outgoing and loves to hangout with people. You will work with CloneBot and design its legendary adventure. 

This lab uses Wizard of Oz prototyping--that is, the Wizard (that is you) controls the robot and gives it the intelligence it does not have it. The point of Wizard of Oz prototyping is to gather data about how people will respond to an intelligent robot, so that you have the information you need to design the robot well.

## Prep
For this week's lab (and also the following week), you will work in groups of 3.

### For this lab, you will need:
1. Smart Phone (Laptop or Tablets also work) -- The main required feature is that the phone needs to connect to WiFi and display a webpage.
2. To work in a group of 3 (encouraged) or 4 people (if necessary).

\*\***^^^ List the names and NetID for your partners above. ^^^**\*\*

Maria Teresa Parreira (mb2554), Pratul Tandon (pt347), Trevor Morcott (trm75)

### Update your personal lab repo
1.  Log in to your github, go to `YourGithubUsername/Mobile_HRI_Lab_Hub/`. 
2.  Click "Sync fork" -> "Update branch"
<img src="https://user-images.githubusercontent.com/20778137/216361417-48d0e8b6-2d21-46e0-869c-b8aa801dfed4.png" width="600">
3. Now your Lab Hub should be updated with the latest lab.


## Lab Overview
For this assignment, you are going to:

A) [Build Your Clonebot](#part-a-build-your-clonebot)

B) [Plan](#part-b-plan) 

C) [Act out the interaction](#part-c-act-out-the-interaction) 

### Deliverables for this lab are: 
1. 5 Storyboards
2. Any reflections you have on the process
3. Video sketch of 3 prototyped interactions (selected from the 5 storyboards)
4. Submit the items above in the Lab1 folder of your class [Github page], either as links or uploaded files. **Each group member should have the updated lab page linked to their own Lab Hub.** Better yet, you could replicate the data in your own repo so that you don't lose anything if your partner modifies or deletes their files later.

### The Report
Just as you copied your Lab 0/Readme.md, create a new file "NetID_Readme.md" under your Lab 1 folder. Leave the original "Readme.md" intact.
This NetID_Readme.md page in your own repository should be edited to include the work you have done (the deliverables mentioned above). Following the format below, you can delete everything but the headers and the sections between the **stars**. Write the answers to the questions under the starred sentences. Include any material that explains what you did in this lab hub folder, and link it in your README.md for the lab.

Each group member must submit their own submission, even if most of the material is identical to their group members. Upload the link to your "NetID_Readme.md" to Canvas. 

Labs are due on Tuesdays before class. 

## Part A. Build Your Clonebot
Form your 3-4 person team.

Follow the instructions [here](https://cornell.box.com/s/i0ykqbfz3y1fj195jax0s28v1n1vsx4o) to build your robot!
The instructions are arranged in stages. At the beginning of each stage, each group must select one (and only one) representitive to pick up parts from us. 

After you finish your robot, plug in power from the USB battery pack. Follow the instructions below to connect to your robot.
1. Connect to WiFi "MobileHRI-x", where x is the number assigned to the ESP-32. (ESP-32 should flash once.)
2. Open a brower, in the address line, type in 192.168.4.1
3. You should be see a control interface. Try out different buttons and see what they do.

## Part B. Plan 

To stage an interaction with your CloneBot, think about:

_Setting:_ Where is this interaction happening? (e.g., an office, the kitchen) When is it happening?

_Players:_ Who is involved in the interaction? Who else is there? Reflect on the design of current day home mobile robots like Roomba. Think through all the people who are in the setting.

_Activity:_ What is happening between the actors?

_Goals:_ What are the goals of each player? (e.g., picking up a pen, opening the fridge). 

Leverage the possible motions of Clonebot and the extra degree of freedom provided by the motor on the top.

\*\***Describe your setting, players, activity and goals here.**\*\*

**STORYBOARDS**

**Scenario 1: Identifying wet floors and warning people**

1. **Setting:** Building Lobby
2. **Players:**
    1. Resident walking out of the building
    2. 3x ConeBot - wet floor warning specialist
3. **Activity:**
    3. Resident is walking out of the elevator into the building lobby where the floor has been cleaned recently, so it is wet and slippery
    4. ConeBots are surrounding the wet portion of the floor to warn people not to slip
    5. When the person approaches the zone, one of the cones intercepts the person and directs them around it
    6. The cones move as the wet floor is drying
4. **Goals:**
    7. Resident: Leave their building without slipping
    8. ConeBots: Prevent injuries while minimizing inconvenience to residents

**Scenario 2: Direct people to the closest available desk in a library**

1. **Setting:** Library at a university
2. **Players:**
    1. A student trying to find a seat at the library
    2. ConeBot - librarian extraordinaire
    3. Inactive participants (students at other tables)
3. **Activity:**
    4. The robot is directing students to tables in the library
    5. A student walks in looking for a desk to work on
    6. The robot approaches the student and guides them to a free seat, moving silently across the library
4. **Goals:**
    7. Student: Find a seat at the library
    8. ConeBots: Quickly and efficiently guide students to seats at the library while minimizing any inconvenience to other students studying already.

**Scenario 3: Help identify unattended victims in a crisis scenario**

1. **Setting**: A crisis scenario (collapsed building on fire) with multiple victims in need of assistance
2. **Players**:
    1. Victims awaiting assistance
    2. EmergencyBot - rescue specialist
    3. Paramedics/Firefighters
3. **Activity:**
    4. The EmergencyBot stands near the most urgent victims in need of assistance
    5. The paramedics attend to the victim
    6. The robot moves to a new victim (next on the priority list)
4. **Goals:**
    7. Victims: get assistance
    8. EmergencyBot: Quickly and efficiently guide firefighters/paramedics to unattended victims
    9. Firefighters/Paramedics: find the victims that need assistance more urgently and that have not been assisted

**Scenario 4: Phone charger bot**

1. **Setting:** This scene takes place in a college library at a table. A person is studying when their phone suddenly dies. 
2. **Players:**
    1. Student
    2. ChargeBot - power banking extraordinaire
    3. Inactive participants (students with charged phones)
3. **Activity:**
    4. The student is studying in the library diligently going over ROS software. All of a sudden, disaster strikes and their phones die
    5. The ChargeBot hears the students' pleas and comes to the rescue with a loanable phone charger for them to use
4. **Goals**:
    6. Student: keep studying without heading back to their dorm to grab their phone charger
    7. ChargeBots: Find students who might need a charger, deliver one to them, while not being disruptive to other students


**Scenario 5: Keeping people from entering places they are not supposed to**

1. **Setting:** This scene takes place in the same library, where there is a “rare book section” with restricted access. 
2. **Players:**
    1. A bored student that wants to explore the library.
    2. BouncerBot (guarding the door)
3. **Activity:**
    3. A graduate student is exploring the library and finds the door to the “rare book section”.
    4. BouncerBot is guarding the door.
    5. The student approaches the door and the robot moves to stop their progress.
    6. Student (confused) moves left then right exploring why the robot keeps moving in front of them.
    7. Student finally realizes it is guarding something and then walks away.
4. **Goals:**
    8. Student: just wants to explore.
    9. BouncerBots: prevent unauthorized personel from entering a restricted area




\*\***Include pictures of your storyboards here**\*\*

**Scenario 1**

![scenario1](https://user-images.githubusercontent.com/62056130/217375224-812c91e0-48b9-4fd1-9fda-4bc680ad6229.png)

**Scenario 2**

![scenario2](https://user-images.githubusercontent.com/62056130/217375368-552a5200-5b66-47eb-984a-c439758c8685.jpg)

**Scenario 3**

![scenario3](https://user-images.githubusercontent.com/62056130/217375419-9746095e-38c5-4493-9d1f-6543bf393c79.png)

**Scenario 4**

![scenario4](https://user-images.githubusercontent.com/62056130/217375446-cbb63c9e-c0ee-4657-9847-2fc3740aaec6.jpg)

**Scenario 5**

![scenario5](https://user-images.githubusercontent.com/62056130/217426036-c9d37aa1-407b-43f9-bc7c-3889f2bd3c1d.PNG)



## Part C. Act out the Interaction

Select 3 of the 5 storyboards to act out. Try physically enacting the 3 interactions you planned with your teammates. (Do not plug in the CloneBot just yet.) Record these video clips, and submit them (Unlisted Youtube links are fine).

Video here: https://drive.google.com/file/d/1FOQmerEaD2auYyprDs9FO398vi1e65Fd/view?usp=sharing

\*\***Are there things that seemed better on paper than acted out?**\*\*

\*\***Are there new ideas that occur to you or your collaborators that come up from the acting?**\*\*

-->  *We enjoyed storyboarding and acting out these scenarios. We ended up acting out the scenarios 2, 4, and 5.* 

*Scenario 2 and 4 were situated in a library. This limited the communication we could use for the robot because libraries are typically quiet. For the robot that guided students to their seat, we found it interesting to brainstorm methods that could be used to indicate a free seat. We ended up going with a pointing gesture, even though we don’t envision the robot itself as anthropomorphic. We had a similar challenge for Scenario 4, which was the ChargerBot that also operates in a library. Here, our critical interaction was to figure out how the user would summon the bot, since calling out loud in a library would not be viable.*

*The challenge for Scenario 5 was a bit different. Intercepting a human and preventing them from entering a room is mechanically straightforward, but it’s less clear how to best communicate with the human being interacted with. We ended up going with a white-board like design where the entire robot is a giant message board. The inspiration for this was the large boards on highways which display warning messages for drivers. Overall, the challenge here was making sure communication is unambiguous. From a practical point of view, we realize the scenarios we video are a bit far-fetched, but since we were able to act them out with a bit of creativity, we believe an implementation is within the realm of possibility.On the other hand, we weren’t able to video two other scenarios we thought were really interesting, because they involved disaster and risk scenarios. One of our takeaways was that experimental design and testing for robots in an emergency response setting is really challenging, even though robots could be very useful in such situations!*


## Your Weekly Dose of ROS

We are not quite finished with the lab from last week.

As I mention, ROS is managed through packages. We have this crazy file structure that looks like a python package but haven't really made a package.
In the last bit of today's lab, let's actually build our package.

Go back to the construct website and log in to your previous Rosject.

In your code editor, open the file `mobilehri_ws/src/my_package/setup.py`.

Replace what's inside with the following code snippet.

```python
from setuptools import setup

package_name = 'my_package'

setup(
    name=package_name,
    version='0.0.0',
    packages=[package_name],
    data_files=[
        ('share/ament_index/resource_index/packages',
            ['resource/' + package_name]),
        ('share/' + package_name, ['package.xml']),
    ],
    install_requires=['setuptools'],
    zip_safe=True,
    maintainer='user',
    maintainer_email='user@todo.todo',
    description='TODO: Package description',
    license='TODO: License declaration',
    tests_require=['pytest'],
    entry_points={
        'console_scripts': [
            'talker = my_package.hri_publisher:main',       # NEW!
            'listener = my_package.hri_subscriber:main',    # NEW!
        ],
    },
)

```

By adding entry points that linked to the main functions in our hri_publisher and hri_subscriber files, we basically create shortcuts for ROS to call our script in Terminal. 

Now, let's build our package. Open a terminal:
``` bash
cd ~/mobilehri_ws/
colcon build          # ignore the warning/err about setup.py being deprecated.
source install/setup.bash
```

Remember that we need to source ROS every time? In order to use your customized ROS packages, you must source them individually as well! To do so, source the setup.bash file within `workspace/install`.

Now, you can call your scripts through ROS the following way:

```bash
# In terminal 1
cd ~/mobilehri_ws/
source install/setup.bash
ros2 run my_package talker
```

```bash
# In terminal 2
cd ~/mobilehri_ws/
source install/setup.bash
ros2 run my_package listener
```

You may notice that the listener does not receive messages published before it is created. As Wendy mentioned in class, the messaging system established through publishers and subscribers are not reliable. They are in fact asynchronous. Publishers are unaware of the subscribers existence. 

To have a more reliable interaction, you will need a new type of mechanism called service and client. We will talk more about this later. 

