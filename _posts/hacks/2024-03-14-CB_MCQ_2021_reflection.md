---
toc: false
comments: true
layout: post
title: CollegeBoard MCQ reflection v2.0
description: Learnings and reflections from completing the CollegeBoard 2021 Practice MC
type: tangibles
courses: { compsci: {week: 6} }
permalink: /plans/week3
---

# Popcorn Hack completion:
Click [here](https://ankit-177.github.io/ankit_tri2//missed-questions) to access the completed popcorn hacks.

## CollegeBoard 2021 MCQ missed questions:
- <mark>Q55</mark>: 
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q55 - Ankit.png>)

- Selected answer - <mark>(A)</mark>: Incorrect. This code segment assigns the value of the last element of the list to the variable temp, then removes the last element of the list, then appends temp to the end of the list. The resulting list is the same as the original list.
- Correct answer - <mark>(C)</mark>: Correct. This code segment assigns the value of the last element of the list to the variable temp, then removes the last element of the list, then inserts temp as the first element of the list.

- <mark>Q67</mark>:
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q67 question - Ankit.png>)
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q67 answer - Ankit.png>)

- Selected answers - <mark>(A)</mark> and <mark>(C)</mark>: 
A is correct. For this spinner, there is a `1/4` chance of "blue". The remaining `3/4` of the time, "orange" and "purple" are equally likely. If the first call to RANDOM returns 1 (which occurs `1/4` of the time), the code segment prints "blue". Otherwise, if the second call to random returns 1 (which occurs `1/2` of the time that "blue" does not occur), the code segment prints "orange". The other `1/2` of the time that "blue" does not occur, the code segment prints "purple".
C is incorrect. This code segment simulates a spinner in which there is a `1/4` chance of "blue", a `1/4` chance of "orange", and a `1/2` chance of "purple". However, the given spinner has a `1/4` chance of "blue", a `3/8` chance of "orange", and a `3/8` chance of "purple".
- Other correct answer - <mark>(D)</mark>: Correct. For this spinner, there is a `1/4` chance of "blue". The remaining `3/4` of the time, "orange" and "purple" are equally likely. The variable spin is set to a random value between 1 and 4, inclusive. If spin is 1 (which occurs `1/4` of the time), the code segment prints "blue". Otherwise, spin is set to a random value between 1 and 2, inclusive. If spin is 2 (which occurs `1/2` of the time that "blue" does not occur), the code segment prints "orange". The other `1/2` of the time that "blue" does not occur, the code segment prints "purple".

- <mark>Q68</mark>:
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q68 - Ankit.png>)

- Selected answers - <mark>(A)</mark> and <mark>(B)</mark>:
A is correct. The code segment will iterate over myList from right to left, removing each element that is equal in value to the element immediately preceding it. For this list, the code segment will remove the sixth element (10), the fourth element (20), and the second element (10). This results in the list [10, 20, 10], which still contains duplicates.
B is incorrect. The code segment will iterate over myList from right to left, removing the sixth element (20), the third element (30), and the second element (30). This results in the list [30, 10, 20], which contains no duplicates, as intended.
- Other correct answer - <mark>(C)</mark>: Correct. The code segment will iterate over myList from right to left, removing each element that is equal in value to the element immediately preceding it. This list does not contain any pairs of adjacent elements that are equal in value, so no elements will be removed even though the value 40 appears twice in the list.

- <mark>Q36</mark>:
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q36 - Ankit.png>)

- Selected answer - <mark>(A)</mark>: Incorrect. Personal information found online can be redistributed via social media posts, e-mail, and other methods.
- Correct answer - <mark>(D)</mark>: Personal information can be found in a variety of places where authentication measures may not be used, including social media sites. Personal information placed online can be collected, aggregated, distributed, and exploited.

## Learnings and notes:
- <mark>Binary bits</mark>: A bit is the smallest unit of data that a computer can process and store. A bit state is represented using 1s and 0s as each bit is always in one of two physical states. Usually, all 8 bits are used. However, in some cases, not all bits are required, as seen in Q31:
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ Q31 - Ankit.png>)

## Total score:
![alt text](</ankit_tri2/images/AP CSP - 2021 MCQ total score - Ankit.png>)