---
toc: false
comments: false
layout: post
title: Test Corrections
description: Test Corrections 
type: tangibles
courses: { compsci: {week: 11} }
---


# AP Computer Science Principles: Test Corrections

## Question 9: 

Which of the following best describes one of the benefits of using an iterative and incremental process of program development?

a. It allows programmers to implement algorithmic solutions to otherwise unsolvable problems.

b. It eliminates the need for programmers to test completed programs.

c. It enables programmers to create programs that use the lowest-level abstractions available.

d. It helps programmers identify errors as components are added to a working program.

### Original Answer
Answer: C
Low level abstractions have nothing to do with the development process of iterations. 

### Corrected Answer 
iterations help programms find errors. 

- **Correct Choice:** D

---

## Question 26 

The grid below contains a robot represented as a triangle, initially facing up. The robot can move into a white or gray square but cannot move into a black region.

The figure shows a grid of squares with 5 columns and 4 rows. The square in the fourth row and first column contains an upward-facing triangle, representing a robot. The first row contains all white squares. The second row contains, left to right, white, black, black, black, white. The third row contains, left to right, white, black, gray, white, white. The fourth row contains, left to right, white, black, black, black, white.

The code segment below uses the procedure One word, Goal Reached, which evaluates to true if the robot is in the gray square and evaluates to falseotherwise.

The program consists of 4 lines. Begin program Line 1: REPEAT UNTIL, open parenthesis, one word Goal Reached, open parenthesis, close parenthesis, close parenthesis Line 2: open brace Line 3: MISSING CODE Line 4: close brace End program.

Which of the following replacements for missing code can be used to move the robot to the gray square?

### Original Answer
Answer: D  

This option is incorrect. This code segment moves the robot one square forward from its initial location and then rotates the robot right. From there, the robot cannot move forward and the body of the IF statement is never executed again.


### Corrected Answer
This option is correct. This code segment rotates right whenever there is an open square to the right. The robot will move forward from its initial location to the upper-left corner of the grid, then rotate right, then move forward to the upper-right corner of the grid, then rotate right, then move down two squares, then rotate right, then move forward to the gray square.

- **Correct Choice:** B

---

## Question 43 

Directions: The question or incomplete statement below is followed by four suggested answers or completions. Select the one that is best in each case.

An online retailer uses an algorithm to sort a list of n items by price. The table below shows the approximate number of steps the algorithm takes to sort lists of different sizes.

A table is shown with 2 columns and 7 rows. The first row of the table contains the column headers, from left to right, Number of Items, Number of Steps. The table is as follows: 10, 100 20, 400 thirty, 900 forty, 1,600 fifty, 2,500 sixty, 3,600

Based on the values in the table, which of the following best characterizes the algorithm for very large values of n ?

### Original Answer
Answer: B  
This option is incorrect. The number of steps of the algorithm is a polynomial, so the algorithm runs in reasonable time.

### Corrected Answer
This option is correct. The pattern in the table appears to indicate that there are n squared steps for a list containing n items. This number of steps is a polynomial and therefore the algorithm runs in reasonable time. 
- **Correct Choice:** A

---

## Question 48 
In a certain science experiment, 7 5 percent of trials are expected to be successful and 2 5 percent of trials are expected to be unsuccessful. The program below is intended to simulate the results of repeated trials of the experiment.

The program consists of 17 lines. Begin program Line 1: successful, left arrow, 0 Line 2: unsuccessful, left arrow, 0 Line 3: REPEAT 1000 TIMES Line 4: open brace Line 5: IF, open parenthesis,  MISSING CODE, close parenthesis Line 6: open brace Line 7: successful, left arrow, successful plus 1 Line 8: close brace Line 9: ELSE Line 10: open brace Line 11: unsuccessful, left arrow, unsuccessful plus 1 Line 12: close brace Line 13: close brace Line 14: DISPLAY, open parenthesis, successful, close parenthesis Line 15: DISPLAY, open parenthesis, open quotation, trials were successful comma, close quotation, close parenthesis  Line 16: DISPLAY, open parenthesis, unsuccessful, close parenthesis Line 17: DISPLAY, open parenthesis, open quotation, trials were unsuccessful period, close quotation, close parenthesis End program.

Which of the following can be used to replace missing code so that the simulation works as intended?

### Original Answer
Answer: B 
This option is incorrect. This option causes the experiment to be successful when RANDOM, open parenthesis 1 comma 100, close parenthesis produces a result from 1to 2 5, or 25% of the time.

### Corrected Answer

This option is correct. This option causes the experiment to be successful when RANDOM, open parenthesis 1 comma 100, close parenthesis produces a result from 1 to 7 5, or 75% of the time.

- **Correct Choice:** D

---


# Definition Search from Google

**Internet Engineering Task Force:** The Internet Engineering Task Force is a standards organization for the Internet and is responsible for the technical standards that make up the Internet protocol suite. It has no formal membership roster or requirements, and all its participants are volunteers.

**Binary Character Representation:** A text-editing application uses binary sequences to represent each of 200 different characters. The minimum number of bits needed to assign a unique bit sequence to each of the possible characters can be calculated as the log base 2 of 200, which equals `x`.

**Creative Commons License:** A Creative Commons license is one of several public copyright licenses that enable the free distribution of an otherwise copyrighted "work." A CC license is used when an author wants to give other people the right to share, use, and build upon a work that the author has created.

**Open Standards and Protocols:** Open standards and protocols allow different manufacturers and developers to build hardware and software that can communicate with hardware and software on the rest of the network.

**Internet Protocol Streaming Standards:**
- Internet protocol version 4 (IPv4) represents each IP address as a 32-bit binary number.
- Internet protocol version 6 (IPv6) represents each IP address as a 128-bit binary number. The result of using 128-bit addresses instead of 32-bit addresses can be described as follows:

   With 32-bit addressing, IPv4 has 2^32 possible addresses.
   With 128-bit addressing, IPv6 has 2^128 possible addresses.
   Since 2^32 times 2^96 equals 2^128, IPv6 has 2^96 times as many possible addresses as IPv4.

**NAND Gate:** In digital electronics, a NAND gate is a logic gate that produces an output which is false only if all its inputs are true; thus, its output is complementary to that of an AND gate. A LOW output results only if all the inputs to the gate are HIGH; if any input is LOW, a HIGH output results.

**Public Key Cryptography:** In public key cryptography, the sender uses the recipient’s public key to encrypt a message. To decrypt the message, the recipient's private key is needed.

**Symmetric-Key Algorithms:** Symmetric-key algorithms are algorithms for cryptography that use the same cryptographic keys for both the encryption of plaintext and the decryption of ciphertext. The keys may be identical, or there may be a simple transformation to go between the two keys.

**Cloud Computing:** Cloud computing is the on-demand availability of computer system resources, especially data storage and computing power, without direct active management by the user. Large clouds often have functions distributed over multiple locations, each of which is a data center.

**Crowdsourcing:** Crowdsourcing involves a large group of dispersed participants contributing or producing goods or services, including ideas, votes, micro-tasks, and finances, for payment or as volunteers.

**Palindrome:** A palindrome is a word, number, phrase, or other sequence of symbols that reads the same backward as forwards, such as "madam" or "racecar," the date and time "12/21/33 12:21," and the sentence: "A man, a plan, a canal – Panama."

**Digital Divide:** The digital divide is the unequal access to digital technology, including smartphones, tablets, laptops, and the internet. The digital divide creates a division and inequality around access to information and resources.

**Internet Communication:** Internet communication is a way of talking to people using the internet instead of telecommunications (like phone calls and text messaging). From WhatsApp and Telegram to email and virtual telephony, people can connect within minutes (if not seconds), irrespective of how far they're located.
