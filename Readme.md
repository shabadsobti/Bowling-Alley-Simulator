# Bowling Alley Score Simulator

I have written this bowling alley simulator in C++.
*Note: This program assumes that the input entered is correct, since it takes in input (Pin State) from the hardware of the bowling alley.*

I have written the program such that the input is taken in from cin to make the program more interactive. 


### How it Works
##### Frame Class
* scoreThrow1 : An int that keeps track of the number of pins knocked down on throw 1
* scoreThrow2 : An int that keeps track of the number of pins knocked down on throw 2
* isStrike : A Boolean that tells us whether that frame was a strike or not
* isSpare : A Boolean that tells us whether that frame was a spare or not
* totalFrameScore() : Returns an int with the sum of the pins knocked on the 1st and 2nd throw

##### Player Class
* name : A string that stores the name of the player
* Frame frames[11] : Makes an array of 11 frames for the player (10 + 1 to account for the fill balls)
* calculateScore() : Returns an int which is the total score for that player


The Driver.cpp file contains the main function is responsible for taking in the input, initializing Players and inserting the values into players, and printing out the scroeboard.

### Compiling and Running

```sh
$ cd campusinterviewbowling
$ clang++ Frame.cpp Player.cpp Driver.cpp
$ ./a.out
```
