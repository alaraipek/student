---
toc: true
comments: false
layout: post
title: Collegeboard Quiz Notes
description: College Board Quiz Notes
type: tangibles
courses: { compsci: {week: 8} }
categories: [C1.4]
---

# Example Questions I Struggled With

## #3: Which of the following would be the best use of citizen science?

A. An experiment that requires all participants to be working in the same laboratory
B. An experiment that requires expensive equipment to conduct
C. An experiment that requires data measurements to be taken in many different locations
D. An experiment that requires specialized knowledge and training to conduct

Correct Answer: C
Explanation: Citizen science is the collection of data relating to the general public. Option C is the only option collecting and measuring data from the general public.

## #5: The ticket prices at a movie theater are given below. <image of table>

A table is shown with 2 columns and 4 rows. The first row of the table contains the column headers, from left to right, Type of Ticket and Price in dollars. The table is as follows: Regular, 12 Child ages 12 and below, 9 Senior ages 60 and above, 9 Below the table is the text: Additional 5 dollar fee for 3 D movies

A programmer is creating an algorithm to set the value of One word, ticket Price based on the information in the table. The programmer uses the integer  variable age for the age of the moviegoer. The Boolean variable One word, is 3 D is true when the movie is 3-D and false otherwise.

Which of the following code segments correctly sets the value of One word, ticket Price ?

Correct Answer: D
Answer D:
ticket price <--12
if age<=12 or age>=60
    ticket price <--9
else
    ticket price <--ticket price + 5
