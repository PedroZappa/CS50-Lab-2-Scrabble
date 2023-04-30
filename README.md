---
layout: default
title: Scrabble
---

# CS50-Lab-2: Scrabble

## Table of Contents
- [Getting Started](#getting-started)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Overview of the Program](#overview-of-the-program)

## Getting Started
This is a C program called scrabble.c that allows two players to play a game of Scrabble. The program calculates the score for each word entered by the players and declares the winner based on the scores. 

## Prerequisites
To run the program, you need a C compiler installed on your computer. You can use GCC or any other C compiler of your choice.

## Usage
To compile the program, open the terminal and navigate to the directory where the file is saved. Then, type:

```sh
gcc -o scrabble scrabble.c
``` 

and press enter. To run the program, type:

```sh
./scrabble
``` 

and press enter.

## Overview of the Program
The program prompts the players to enter their words, calculates the scores using the POINTS array, and compares the scores to declare the winner. The POINTS array contains the points assigned to each letter of the alphabet. The program handles errors, such as when a player enters an invalid word or when the words entered are of different lengths.

The `compute_score` function takes a word as input and returns the score for that word. The function uses a score tracker to keep track of the score and computes the score for each character in the word. If the character is uppercase, the function adds the corresponding score from the POINTS array. If the character is lowercase, the function adds the corresponding score from the POINTS array.

The `main` function gets input words from both players, scores both words using the `compute_score` function, and prints the winner based on the scores.
