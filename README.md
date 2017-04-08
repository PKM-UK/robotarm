# robotarm
Code for controlling a two-jointed SCARA type arm

# Structure
## Class descriptions

**Controller:** the main class of a program using the arm.  Takes user input in the form of interactive controls or program input, drives the calculation of arm position from desired end effector target, and feeds control data to the arm's representation (animated canvas or servo signals).

**Arm:** an abstract representation of a two-jointed arm in an abstract coordinate space.  Takes input in the form of desired end effector location and does IK to deduce arm joint angles.

**Representation:** a way to mnifest the abstract arm's movement in meatspace.  Either an animated canvas in a Tkinter window, or outputting servo signals over the GPIO pins for servos to drive a physical arm.
