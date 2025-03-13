# Definitions

## Odometry Pods
Odometry pods are basically just wheels that roll when your robot moves. They capture distance and rotation, and
when given a starting position, can tell you where you are on a field. They are also referred to as
deadwheels or encoders. 

## Field Relative Drive
A field relative drive is commonly used in FTCLib competitions. Instead of the forward direction being where the 
robot is facing, the "forward" direction is always set to the way the robot is facing when you start the opmode.
After it's started, even if the robot is rotated, forward will still be the original direction. 


## Max Robot Speed MPS
This is the maximum speed the robot can travel in meters per second. Set this initially based on the test
and then lower as needed. Often you will NOT need the robot to be going extremely fast for competitions, 
and a slower more smooth motion nets more points per game. 

## Max Robot Speed RPS
This is the maximum speed the robot can rotate per second. Again determined by testing, and can be
lowered if needed. 

## Meters per Tick
Odometry Wheels operate in "ticks" (also sometimes called resolution). A tick is a very small increment. A standard odometry wheel can have
thousands of ticks per full revolution of the wheel. But ticks on their own are useless in determining how far
something has gone in real world units, thus the need for a "meters per tick" measurement. 

## Dead Wheel Radius Centimeters
The radius of your "dead wheels", or odometry wheels. 

## track Width Centimeters
The distance between your two parallel odometry pods in centimeters.

## Perpendicular Offset Centimeters
Distance (must be positive) between the center of your robot and the third odometry pod. 

## PIDs
PIDs are broken down into two "controllers", each having a P I and D value. There is a translation
controller and a rotation controller, which control translation and rotation respectively. 
The P value controls proportional movement. A higher P value will make the robot "correct faster".
The D value dampens movement, meaning when a robot gets close to its target position, it will start to slow down.
The I value adds a little "push" to the robot to help it reach its target position, if it is close but not
quite at the target. 



