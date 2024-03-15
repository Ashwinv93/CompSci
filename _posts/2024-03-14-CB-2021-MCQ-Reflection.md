---
toc: False
comments: True
layout: post
title: 2021 MCQ Reflection
description: 
type: tangibles
courses: {'compsci': {'week': 26}}
---

## How I did:
I got a score of 61/70 which I felt was a good score under the time pressure we had, to finish during one class period. The majority of my mistakes can be attributed to rushing though the questions, or misunderstanding what questions were asking. Overall I feel this is an improvment to my last score of 55/67.

## Corrections

- ### Q14 Error in isIncreasing procedure
<img src="https://Ashwinv93.github.io/CompSci/images/Q14.png" alt="Description of Image"/>
Answer B was incorrect. By making thay change, the procedure will immediately return true any time it encounters a value that is greater than or equal to the preceding value. It will not check any subsequent values in the list. The correct answer would be C to swap lines 8 and 12

- ### Q15 Use drawLine procedure to draw figure
<img src="https://Ashwinv93.github.io/CompSci/images/Q15.png" alt="Description of Image"/>
Answer B is incorrect. The code segment draws five horizontal line segments, starting with the segment from (1, 0) to (2, 0) and ending with the segment from (1, 4) to (6, 4), which is not the graph the question was looking for. The correct answer was 

- ### Q37 Which is not a possible value displayed
<img src="https://Ashwinv93.github.io/CompSci/images/Q37.png" alt="Description of Image"/>
D is Incorrect. The string "daikon" is displayed for values of n that are less than or equal to 10. This was a very easy question looking back, not sure how I got this one wrong. Might be due to rushing. 

- ### Q45 Using botStepper procedure
<img src="https://Ashwinv93.github.io/CompSci/images/Q45.png" alt="Description of Image"/>
D was not correct here becuase in this code segment, the first call to botStepper moves the robot forward three squares, rotates it left so that it faces toward the top of the grid, moves it forward three squares, and rotates it right so that it faces right. The code segment then moves the robot forward one square. The second call to botStepper attempts to moves the robot forward four squares, off the edge of the grid, causing execution to terminate.

- ### Q55 Move element from end of list to beginning
<img src="https://Ashwinv93.github.io/CompSci/images/Q55.png" alt="Description of Image"/>
A is Incorrect. This code assigns the value of the last element of the list to the variable temp, then removes the last element of the list, then appends temp to the end of the list. The resulting list is the same as the original list.

- ### Q59 Data not provided by user device
<img src="https://Ashwinv93.github.io/CompSci/images/Q59.png" alt="Description of Image"/>
Answer A is incorrect. While Adrianna’s average running speed is useful in determining whether other users are considered compatible with Adrianna, this information is determined using data collected from Adrianna’s device. C would be a better answer because location data would be much more useful.

- ### Q63 Boolean expression equivalent to table
<img src="https://Ashwinv93.github.io/CompSci/images/Q63.png" alt="Description of Image"/>
For this question my answer A was correct, but B was not. The other answer was D, because  when input1 and input2 are both true, the expression (input1 AND input2) is true, so NOT (input1 AND input2) will evaluate to false. In all other cases, (input1 AND input2) will evaluate to false, so NOT (input1 AND input2) will evaluate to true.

- ### Q68 Error in remove duplicates code segment
<img src="https://Ashwinv93.github.io/CompSci/images/Q68.png" alt="Description of Image"/>
Answer B was incorrect here. The code segment will iterate over myList from right to left, removing the sixth element (20), the third element (30), and the second element (30). This results in the list [30, 10, 20], which contains no duplicates, as intended. The correct answers were A, which I had, and C since this list does not contain any pairs of adjacent elements that are equal in value, so no elements will be removed even though the value 40 appears twice in the list.

- ### Q70 Remove nth character from oldStr
<img src="https://Ashwinv93.github.io/CompSci/images/Q70.png" alt="Description of Image"/>
B was Incorrect. This code segment assigns the characters from the start of the string to one past position n to the variable left. The code segment then assigns the characters from one before position n to the end of the string to the variable right. It then concatenates left and right and assigns the result to newStr. For example, if oldStr is "best" and n is 3, the code segment assigns "best" to left, "est" to right, and "bestest" to newStr.

## Final Thoughts
My final thoughts after the exam are good. I have a good idea of what I need to work on before the AP test, and I think I can aim to get at least a 4 on the AP test. Psudo code and other code segments are my main weakness right now, so I will try to practice more with that.