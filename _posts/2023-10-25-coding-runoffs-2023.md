---
layout: post
title:  Coding Runoffs 2023
date:   2023-10-25
categories: problem-sets
---

# Procedure

Every team will be given exactly 40 minutes to work on the coding challenges listed below. At the end of the 40 minutes, a USB flash drive will be used to collect solutions. Be sure to put all code files into a ZIP file or a folder named with the people in the team and have the individual solution code files labeled with the appropriate problem it addresses.

Teams are allowed to use personal computers and can use any code editor, online or local. We recommend using replit.com for ease.

There are intentionally more problems assigned than time will allow for most people to complete; it is normal to not have every problem solved. Solutions will be graded first on passing all test cases with partial credit for passing most but not all test cases or slight formatting errors in the output used as a tie breaker.

Other rules:
- External help of any sort is not allowed including but not limited to reading documentation, checking StackOverflow, asking ChatGPT, working with other teams, or seeking assistance from someone not competing
- Third party libraries and packages may not be used
- Allowed languages: C (version C11), C++ (version C++14), C# (version 6.0), Java (version 10), Javascript (NodeJS version 8.10), Python (version 3.6), Ruby (version 2.5), Swift (version 4.2)
- AI code writing extensions like Github Copilot and Kite are banned.
- We will not give unrealistic inputs. They will be of the correct data types and within reasonable ranges for computing. The point is logically solving the problem rather than data sanitization.

# Problem 1

Prime numbers are numbers that are not divisible by any numbers except itself and 1. Ex. 17, 31, 11.

Prime factors are the prime numbers which can be multiplied to create a given integer. Ex. the prime factors of 234 are 2, 3, 3, and 13 since those numbers are prime numbers and multiply to 234.

Given a number, list all prime factors including duplicates so that their product is the input number.

List the integers from smallest to largest, including duplicates, separated by spaces, with no other formatting like brackets or commas.

## Example 1

Input
```txt
459
```

Output
```txt
3 3 3 17
```

Explanation

| The prime factors of 459 are listed. They all multiply to 459. |

## Example 2

Input
```txt
2837
```

Output
```txt
2837
```

Explanation

| 2837 is a prime number, so it simply returns itself. |

# Problem 2

Number bases are ways to represent numbers using a limited set of symbols. We normally use base-10 which uses 10 symbols to represent numbers (0-9). Many people are familiar with binary which is base-2 as it uses just 0 and 1.

Given an integer from 2-9 and another integer in base-10, return the second number converted into the base of the first number.

## Example 1

Input
```txt
2
50
```

Output
```txt
110010
```

Explanation

| The first number, 2, indicates base-2. 50 in base-2 is 110010. |

## Example 2

Input
```txt
7
294382
```

Output
```txt
2334154
```

Explanation

| The first number, 7, indicates base-7. 294382 in base-7 is 2334154. |

# Problem 3

Given a sequence which represents tic-tac-toe board, return which side won. The board will be represented as a string going left to right then down. Spaces represent the next row and a period will represent an empty spot.

ALL test cases will have a winning player and a physically possible board setup.

## Example 1

Input
```txt
XOX OOX XO.
```

Output
```txt
O wins
```

Explanation

| The board will appear as follows:<br />XOX<br />OOX<br />XO.<br /><br />The O player then wins with 3-in-a-row down the middle. |

## Example 2

Input
```txt
OOX .X. X..
```

Output
```txt
X wins
```

Explanation

| The board will appear as follows:<br />OOX<br />.X.<br />X..<br /><br />The X player then wins with 3-in-a-row down the middle by the diagonal. |

# Problem 4

Rotating a letter is simply moving up in the alphabetical order by the desired rotation. For example, if I have the letter “a” and the rotation number is 3, the result would be “d” since three letters up from a is d. a > b > c > d.

Given a number and a string of text, shift the letters up by the given number. The rotation number will be taken first then the string.

All input will be lowercase letters.

## Example 1

Input
```txt
5
hello world
```

Output
```txt
mjqqt btwqi
```

## Example 2

Input
```txt
-1
jakob is cool
```

Output
```txt
izjna hr bnnk
```

# Problem 5

Given a list of words, sort them in reverse alphabetical order.

## Example 1

Input
```txt
bee hello groundhog book cranky
```

Output
```txt
hello groundhog cranky book bee
```

## Example 2

Input
```txt
grumble cup mouse instinct chariot phone
```

Output
```txt
phone mouse instinct grumble cup chariot
```

# Problem 6

Given a list of words, list all letters used in order of most to least shared.

Note how this is not about the most used letter but rather how many words in the list use the letter. If there is a tie, order the letters alphabetically. If a letter is never used, do not include it in the output.

## Example 1

Input
```txt
branch leaf stone rock water air
```

Output
```txt
arecnotbfhiklsw
```

## Example 2

Input
```txt
jump run skip hop twist flip
```

Output
```txt
pisufhjklmnortw
```
