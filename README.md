Download link :https://programming.engineering/product/lab-introduction-robot-arm-ur3/


# Lab-Introduction-Robot-Arm-UR3
Lab Introduction: Robot Arm UR3
Scope & Objective

The purpose of this lab is to familiarize you with the UR3 robot arm with its industrial programming interface called the teach pendant and some basic operation. In this lab, you will:

Learn how to turn on and activate the UR3, and work with the teach pendant to create a simple program for the UR3

Use the teach pendant to turn on and off the suction cup gripper and use the gripper in a program

Demonstrate a sequence of motions that places one block on top of another.

Background

Robot arms can be used to manipulate objects in the workspace repetitively with speed and precision. Being familiar with a standard robot arm equips one with the ability to operate, design and develop robot solutions relevant to applications in numerous engineering domains including industrial automation, remote teleoperation, rescue missions, medical procedures etc.

Through the lab sessions in this course, you will be using a collaborative robot arm UR3 from Universal Robots. The UR3 has a compact form factor appropriate for tight workspaces. Designed as a collaborative table-top robot, perfect for light assembly tasks and automated workbench scenarios. The compact table-top cobot weighs only 24.3 lbs (11 kg) but has a payload of 6.6 lbs (3 kg), 360-degree rotation on all wrist joints, and infinite rotation on the end joint. These unique features make the UR3 cobot the a flexible, lightweight collaborative table-top robot to work side-by-side with a human operator.

References

UR3 Owner’s Manual:

https://www.universal-robots.com/download/?option=52870#section52851

UR3 Software Manual:

https://www.universal-robots.com/download/?option=53077#section53064

Universal Robots Academy https://www.universal-robots.com/academy/


Pre-lab

Before you come to lab it is very important that you go through the training videos found at Universal Robots website https: / /www. universal-robots. com/ academy/. These training sessions get into some areas that we will not be using in this class (for example you will not be changing safety settings) but go through all of the assignments as they will help you get familiar with the UR3 and its teach pendant. You also may want to reference these sessions when you are in lab.

Lab Activities

Using the teach pendant, each team will “program” the UR3 to pick and place blocks. The program may do whatever you want, but all programs must check three predefined locations for two blocks and stack one block on top of another at a fourth predefined position. You will use the gripper’s suction feedback to determine if a block is located at one of the three starting block locations. The blocks must be aligned with each other in the stack of two.

The Pre-Lab asked you to go through the basic UR3 training at Universal Robots website. This training should have shown you how to make simple programs to move the UR3. Initially your TA will demonstrate how to turn on and enable the UR3 as well as how to use the emergency stop button. Then use this lab time to familiarize yourself with the UR3 robot. First play around with simple programs that move the robot between several points.

To turn on the suction for the suction cup gripper, Digital output 0 needs to be set high. Set low to turn off the suction. Also, Digital input 0 indicates if the suction cup is gripping something. It will return 1 if it is gripping an object and O if not. Modify your above program (or make a new one) to add activating on and off the suction cup gripper.

Create a program that defines four spots on the robot’s table. Three of these spots are where it is possible a block will be initially located and with a certain orientation. There will only be two blocks. The user will place the blocks in two of the positions. The goal for the robot is to collect the two blocks and stack them on top of each other in the fourth define place on the robot’s table. So, you will need to use the suction cup gripper’s feedback that indicates whether an object is being gripped or not. Then with some “If” instructions complete this task such that the user can put the two blocks in any of the three starting positions. When you are finished, you will demo your program to your TA showing that your program works when two blocks are placed and aligned in the three different configurations and does not have a problem if only one block or even no blocks are placed at their starting positions. Tips for creating this program:

To turn on the suction cup, use the Set command and select Digital Output O and turn it on or true. Set it to off or false to turn off the suction.

Digital Input O indicates if something has been gripped by the suction cup. Go to the 1/0 tab and turn on and off Digital Output 0 and check which


state of Digital Input O indicates gripped and upgripped.

In the Structure tab under Advanced besides “If … else”, you may also want to use the Assignment to create a global worker variable that, for example, stores the number of blocks collected. In addition, the SubProg item creates a subroutine that you may call when performing the same steps. The subroutine’s scope allows it to see the variables you create with the Assignment item.

You may want to name your Waypoints. This makes your program easier to read. In addition, if the robot needs to go to the same point multiple times in your program you can command it to go to the same waypoint name.

Under the Structure tab you can use the Copy and Paste buttons to copy a line of code and past it in a different subsection of your code. This cuts down on extra typing. Also note the Move up and down buttons along with the Cut and Delete buttons. Suppress is like commenting out a line of code.

When you add an “If” statement and then click on the Command tab, tap in the long white box to pull up the keyboard for entering the if condition.

Demo this working program to your TA. Your TA may ask you to improve your positioning if the stack does not end up aligned well.

Report

None required. Look at Lab 1 and start the reading assignment for Lab 2’s pre-lab.

Demo & Grading

Show your TA the program you created.

20 points, completing the above tasks by the end of your two-hour lab session.

80 points, successful demostration.
