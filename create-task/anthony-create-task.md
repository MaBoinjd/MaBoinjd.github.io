---
title: Anthony Create Task
permalink: /create-task/anthony
layout: default
---

## Program Code

[Link to code on GitHub](https://github.com/tonyhieu/csp-anthonys-harem/blob/main/api/templates/5.html)

## Video

[Link to video](https://drive.google.com/file/d/1UFv2jMzpngi4QZ3bXwmZ6ert5TJ1hVvi/view?usp=sharing)

## Written Responses

### 3a

i. Describe the overall purpose of the program

The program gathers a list of inputs and a list of outputs. Then, it randomizes each input to an output, creating random pairings. It does so in the style of Amidakuji, meaning that the top row of inputs must go down their respective lines and reach an output. Each time the vertical line meets a horizontal line, the input must "switch" to the new vertical line and go down it.

ii. Describe what functionality of the program is demonstrated in the video

The video shows the program taking a list of inputs and outputs. Then, it shows the user adding "legs" to the Amidakuji. The user calculates the pairings by clicking "Calculate Pairings," and the inputs are randomly assigned to an output. After, the user selects which path they'd like to see in order to see how the input got to the output. 

iii. Describe the input and output of the program demonstrated in the video

The user input includes two things: the set of inputs and outputs, and the legs. By clicking each of the legs, the user sees the output of how each path is formed. The set of inputs and outputs are randomized and the user receives the output of random pairings.

### 3b

i. The first program code segment must show how data have been stored in the list

![3bi Code](/assets/images/Screen Shot 2022-02-20 at 12.27.32 PM.png)

ii. The second program segment must show the data in the same list being used

![3bii Code](/assets/images/Screen Shot 2022-02-20 at 12.30.13 PM.png)

iii. Identify the name of the list being used in the response

lines

iv. Describe what the data contained in the list represent in your program

The data in the lines list represents one vertical line in the Amidakuji. Each element in the list represents either no horizontal line (represented by -1) or a horizontal line (represented by the index of the vertical line).

v. Explains how the selected list manages complexity in your program code

This 2D array of vertical lines and the positions in which they switch to a different line allows the program to actually match an input to an output through the path set by the user. Since the path defined by Amidakuji involves switching to the corresponding vertical line once a ghost leg is touched, storing the information of where the legs is extremely helpful in navigating the lines.

### 3c

i. The first program must be a student-developed procedure that:
- [x] Defines the procedure's name and return type (if necessary)
- [x] Contains and uses one or more parameters that have an effect on the functionality of the procedure
- [x] Implements an algorithm that includes sequencing, selection, and iteration

![3ci Code](/assets/images/Screen Shot 2022-02-20 at 12.38.27 PM.png)

ii. The second program code segment must show where your student-developed procedure is being called in your program

![3cii Code](/assets/images/Screen Shot 2022-02-20 at 12.40.18 PM.png)

iii. Describe in general what the identified procedure does and how it contributes to the overall functionality of the program

The procedure draws the path connecting a selected top input (given by the parameter startingLine) to the bottom output using the user-placed horizontal lines on the board.

iv. Explain in detailed steps how the algorithm implemented in the identified procedure works

The algorithm uses the lines list mentioned in **3b** to identify the line and its corresponding horizontal lines. Then, it goes down the list, changing its position (denoted by currentLine) whenever a non -1 value is found. For each position where it is possible to have a horizontal line, the algorithm will draw a red line going down to that position (herein referred to as a notch), and if that notch contains a horizontal line, then the algorithm will move to the left or right depending on whether or not the new vertical line is greater (to the right) or less than (to the left) the current line. After going through all of the notches, the program ends.

## 3d

This section will use this picture as the assumed board state

![3d Board](/assets/images/Screen Shot 2022-02-20 at 12.53.49 PM.png)

i. Describe two calls to the procedure identified in writted response **3c**

First call: findPath(0) <br />
Second call: findPath(1)

ii. Describe what condition(s) is being tested by each call to the procedure

The same conditions will be tested in both calls. The only difference will be in which line they start on. findPath(0) will start on Line 0, or the leftmost line, while findPath(1) will start on Line 1, or the middle line. The paths these two go on will be different, as an input starting on Line 0 will go to Line 1 and end on Line 2, or the rightmost line. However, an input starting on Line 1 will go to Line 0 and end back on Line 1. Each one will test different conditions, as the horizontal lines are in different places, so the if statements will be comparing different things.

iii. Identify the result of each call

Result of the first call: 

![First Call Result](/assets/images/Screen Shot 2022-02-20 at 12.58.47 PM.png)

Result of the second call:

![Second Call Result](/assets/images/Screen Shot 2022-02-20 at 12.59.35 PM.png)
