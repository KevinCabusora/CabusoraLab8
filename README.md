CabusoraLab8
============
C2C Kevin Cabusora, Dr. York, 12 December 2014

Maze Solving Robot

##Prelab

###Goal

The basic design I have for this robot is for it to go forwards until the sensor reads out the voltage threshold I found in Part 7.  Then, it will stop.  I will do a wall-hugger method, where it will check

###Pseudocode
```
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
```

## Required Functionality

### Schematic
![Schematic](https://github.com/KevinCabusora/CabusoraLab8/blob/master/Rough%20Schematic.JPG)

### Code
![Code](https://github.com/KevinCabusora/CabusoraLab8/blob/master/RequiredFunctionality)

### Demonstration
Demoed to Dr. York on 12 December 2014.

### Design/Debugging
Since I was stretched for time, I went for an initial moveForward through the initial stretch of the maze.  I then made a turn left.  Then, my robot would move incrementally left and right slightly in an attempt to dodge the walls and not crash.  Unfortunately, I believe I may have switched the wiring on my sensors since instead of veering away from the walls, it would consciously move towards them.  Besides that, my robot eventually made it to the end wall.  Due to the shortness of time, editing the move time and delay time constants was my main problem.

### Documentation
C2C Erica Lewandowski advised me to take small steps in my robot, which was very useful.  Dr. Coulston suggested turning down the lights due to sensitivity issues.  C2C Kyle Jonas advised on how to do basic while loops of how to decide where the robot would go and to slow down my duty cycle.
