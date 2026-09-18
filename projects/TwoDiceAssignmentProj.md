---
layout: project
type: project
image: img/Twodicepig.png
title: "Two Dice Pig Game"
date: 2026-09-17
published: True
labels:
  - Assignment
summary: "A two dice pig game assignment I did in ICS 111."
---

<img class="img-fluid" src="..img/Twodicepig.png">

## What is it about?

The two dice pig game was an assignment that I had to do for ICS 111 using Java. The game lets you have two players, name the players, set the winning score, and then actually play the game in a panel. It's basically a dice game where two players roll the dice and can either hold their number, roll again, get doubles, or lose all their points.

## Experience
This was the first assignment that had me use a full panel with user typed names, score tracking, and buttons to roll or hold. Before this, I hadn't built anything that combined user input, live score updates, and interactrive buttons all in one GUI, so it was a good introduction to putting all those pieces together and getting them to actually respond to each other.

Below is an example of some of the scoring code:
```ruby
   if (die1 == 1 && die2 == 1) {
     currentPlayer.setScore(0);
     turnScore = 0;
     rollResult += "Double Ones. Score reset to 0 :(.";
     swapPlayers();
   } else if (die1 == 1 || die2 == 1) {
     turnScore = 0;
     rollResult += "Rolled a one. Sorry turn is over.";
     swapPlayers();
   } else if (die1 == die2) {
     turnScore += 2 * die1;
     rollResult += "Doubles! Roll again with double points :D";
     dice.roll();
     doRules();
     return;
   } else {
     turnScore += die1 + die2;
     rollResult += "Points added. Total turn score is " + turnScore + ".";
   }
```
## Thoughts
I think this part of the assignment was one of the more interesting parts to work through, since there were several different outcomes to account for depending on the roll. Making sure double ones reset the score, a single one ended the turn, doubles let you roll again, and a normal roll just added points all had to work correctly together without messing up. It also helped me to get more comfortable with recursive calls, sincne rolling doubles meant the method needed to call itself again to let the player keep rolling.
