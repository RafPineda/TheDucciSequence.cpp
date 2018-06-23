# TheDucciSequence.cpp
Part of a "Daily Challenge" on
https://www.reddit.com/r/dailyprogrammer/comments/8sjcl0/20180620_challenge_364_intermediate_the_ducci/

A Ducci sequence is a sequence of n-tuples of integers.
Given an "n"-tuple sequence, 
  for example: (0, 653, 1854, 4063),
The Ducci Sequence will take the absolute difference between neighboring integers, and output it as a new sequence of equal tuples.
 The first and last numbers in a tuple are considered neighbors for this.
 
  Given (0, 653, 1854, 4063), 
 the next expected output is [0; 653; 1854; 4063].
 
  For this code, input is expected to be in a correct format:
  (x1, x2, x3 .. xn)
  Where there must be at least 1 integer value.
  
    TheDucciSequence will then output all new produced tuples until it either hits a tuple of all zeroes such as [0, 0, 0]
  or reaches a complete loop.
 
 
 Here is an example: 
Given the input (0, 653, 1854m 4063)

The program will output:

---
[0; 653; 1854; 4063]
[653; 1201; 2209; 4063]
[548; 1008; 1854; 3410]
[460; 846; 1556; 2862]
[386; 710; 1306; 2402]
[324; 596; 1096; 2016]
[272; 500; 920; 1692]
[228; 420; 772; 1420]
[192; 352; 648; 1192]
[160; 296; 544; 1000]
[136; 248; 456; 840]
[112; 208; 384; 704]
[96; 176; 320; 592]
[80; 144; 272; 496]
[64; 128; 224; 416]
[64; 96; 192; 352]
[32; 96; 160; 288]
[64; 64; 128; 256]
[0; 64; 128; 192]
[64; 64; 64; 192]
[0; 0; 128; 128]
[0; 128; 0; 128]
[128; 128; 128; 128]
[0; 0; 0; 0]
24 steps

---

24 steps being the amount of tuples produced before the sequence either enters an infinite loop, or reaches all zeroes.
Tuples can be of various lengths before entering a loop as shown at https://en.wikipedia.org/wiki/Ducci_sequence#Examples


More information about the Ducci Sequence can be found at https://en.wikipedia.org/wiki/Ducci_sequence 
