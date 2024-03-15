---
toc: false
comments: true
layout: post
title: CollegeBoard MCQ reflection
description: Learnings and reflections from completing the CollegeBoard 2020 Practice MC
type: tangibles
courses: { compsci: {week: 6} }
permalink: /plans/week2
---

## Learnings and notes:
- <mark>Binary bits</mark>: A bit is the smallest unit of data that a computer can process and store. A bit state is represented using 1s and 0s as each bit is always in one of two physical states. Usually, all 8 bits are used. However, in some cases, not all bits are required, as seen in Q49:
![Alt text](<../../images/AP CSP - Q49 mistake - Ankit.png>)

- <mark>Internet Protocol (IPv6)</mark>: The Internet Protocol (IP) is a protocol, or set of rules, for routing and addressing packets of data so that they can travel across networks and arrive at the correct destination. IPv6 is the most recent version of Internet Protocol (IP). It's designed to supply IP addressing and additional security to support the predicted growth of connected devices in IoT, manufacturing, and emerging areas like autonomous driving.

- <mark>Algorithm run-times</mark>: We can categorize the run time of an algorithm according to how the number of steps increases as the input size increases. According to CollegeBoard, accessing elements `2n` times, or `2` times per element, is considered reasonable run-time. Also, accessing elements `n^2` times, or `n` times per element, is considered reasonable run-time. This is seen in Q50, which I got wrong:
![Alt text](<../../images/AP CSP - Q50 mistake - Ankit.png>)

- <mark>Q67 - Error in numOccurences procedure</mark>: The question is seen below:
![Alt text](<../../images/AP CSP - Q67 mistake - Ankit.png>)

Explanation for option A (<strong>Correct</strong>): Correct. For this code segment, count is increased to 1 the first time "birch" is encountered in the list. However, count is reset to 0 when the code segment moves to the next list element. The last time "birch" is encountered in the list, count is again increased to 1, causing the procedure to return 1 instead of the intended result 2.

Explanation for option B (<strong>Correct</strong>): Correct. For this code segment, count is increased to 1 the first time "maple" is encountered in the list. However, count is reset to 0 when the code segment moves to the next list element. This causes the procedure to return 0 instead of the intended result 1.

Explanation for option C (<strong>Incorrect</strong>): Incorrect. Incorrect. For this code segment, count is increased to 1 when "oak" is encountered as the last element of the list. The loop then terminates and the procedure returns the intended result 1.

Explanation for option D (<strong>Incorrect</strong>): Incorrect. For this code segment, count is initialized to 0. Since "spruce" does not appear in the list, the procedure returns the intended result 0.

### Total score:
![Alt text](<../../images/AP CSP - CB MCQ 2020 score - Ankit.png>)