CabusoraLab8
============

Maze Solving Robot

##Prelab

###Goal

The basic design I have for this robot is for it to go forwards until the sensor reads out the voltage threshold I found in Part 7.  Then, it will stop.  I will do a wall-hugger method, where it will check

###Pseudocode
Initialize connections

Define movements, times, interrupts

Begin routine, have robot move forwards

If front IR sensor reads less than 5 inches,
  then stop, take reading of right IR sensor
    then taking reading of left IR sensor
  compare voltage readings
    
    If right > left 
      then rotate 90 degrees to left
    Else rotate 90 degrees to right
Else keep moving forwards
