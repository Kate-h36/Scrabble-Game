# Scrabble-Game

This is a simple C program that calculates the score of two players in a game of Scrabble. 
The program prompts the users to input words played by each player and computes the total score for each player 
based on the point values of the tiles used in the words.

 * [Rules of the Game](https://github.com/Kate-h36/Scrabble-Game/blob/main/README.md#rules-of-the-game)
 * [Quick Start](https://github.com/Kate-h36/Scrabble-Game/blob/main/README.md#quick-start)
 * [Examples](https://github.com/Kate-h36/Scrabble-Game/blob/main/README.md#examples)
 * [Usage](https://github.com/Kate-h36/Scrabble-Game/blob/main/README.md#istallation)
 * [Description of Algorithm](https://github.com/Kate-h36/Scrabble-Game/blob/main/README.md#description-of-algorithm)

## Rules of the Game 

in the game of Scrabble, players create words to score points, 
and the number of points is the sum of the point values of each letter in the word.
For example, if you wanted to score the word `Code`
you would note that in general Scrabble rules, character `С` is worth `3`points
the `o` is worth `1` point, the `d` is worth `2` points 
and the `e` is worth `1` point
Summuring this you get that word `Code` is worth `3 + 1 + 2 + 1 = 7` points.

## Quick Start

1. Enter the words played by Player 1 and press Enter.
2. Enter the words played by Player 2 and press Enter.
3. The program will compute and print the score for each player and declare the winner.

## Examples

```
$ ./scrabble
Player 1: Question?
Player 2: Question!
Tie!
```
```
$ ./scrabble
Player 1: Oh,
Player 2: hai!
Player 2 wins!
```
```
$ ./scrabble
Player 1: COMPUTER
Player 2: science
Player 1 wins!
```
```
$ ./scrabble
Player 1: Scrabble
Player 2: wiNNeR
Player 1 wins!
```

##  Usage 

### Prerequisites
* C compiler(clang, gcc e.t.c)
* CS50 Library for C languge. 
 Detailed installation process can be found here: https://cs50.readthedocs.io/libraries/cs50/c/

### Istallation
1. Clone the Repository
```
git clone https://github.com/Kate-h36/Scrabble-Game.git
```
2. Compile and link the program
```
clang -o scrabble scrabble.c -lcs50
```
3. Run the program 
```
make scrabble
./scrabble
```

## Description of Algorithm

The program uses an algorithm to calculate the score for each player. For each word played by a player, the program loops through each letter in the word and looks up its point value in a predefined array. The program then sums the point values for each letter in the word represening each character using ASCII, as a number. Finally, the program adds the word score to the player's total score. The player with the highest total score is declared the winner.
