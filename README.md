﻿# PacmanChallenge
 
 ### Pacman Questions
  With the given .txt file, is there a need to keep track of the board with how many objects are on the board( ex. Ghost, fruits, etc)? Do  they repopulate to always have 4 ghosts. 
  
  Need to study how to read/run a .txt file. 
  
  Should we have the read cycle end as soon as Pacman runs out of lives, or allow negatives? (Making the assumption the program with end "if" pacman runs out of lives. 
  
  Also,to make sure, do we want to count just his total lives gained, or total lives left at the end of the game? Or both?
  
### Pacman Goals 
    Studying on how to read a .txt file within a console app
      -Resources found
        https://stackoverflow.com/questions/31310026/how-to-read-from-a-text-file-and-then-write-to-another-in-one-console-applicatio
        https://support.microsoft.com/en-us/help/816149/how-to-read-from-and-write-to-a-text-file-by-using-visual-c
  
    To set up three classes/tables to account for the Player, PlayerInput, ScoringData, and LifeData :
      -Player will inherit from PlayerInput(if time look to see if there is anything repeating a lot)
      -PlayerInput will have Total values like IsAlive(bool), TotalLives(default 3), TotalPoints(default 5000), TotalLivesGained
      -ScoringData is for ObjectsEaten like Fruits(several values), Dots, and VulnerableGhost(multipling worth)
      -LifeData is for LiveOrDeath objects liek GainLife(add life), GhostOfDeath(subtract life)
      
    Then begin Program.cs file: 
      -Add a method for each Dot eaten(add 10 points)    
      -GhostOfDeath method for each one InviniableGhost hit(subtract 1 lives until 0)
      -Add methods for fruits eatens(add var points)
      -Work on methods for doubling up point values for VunerableGhost(* 2 per Ghost probably use an "if")
      -GainLife (once TotalPoints reaches an interval of 10,000 points add a life, probably also an *if)
    
###Concerns
  
    -Would it by easier to put in one file rather the seperation?
    -Reading the Txt file other that copy /paste(but I'm not certain if that will work or not)
    -Data types used.
    -Turn Ints to negative numbers
      -https://stackoverflow.com/questions/1348080/convert-a-positive-number-to-negative-in-c-sharp
   

  
  
