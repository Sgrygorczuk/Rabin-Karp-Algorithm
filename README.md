Course CSc 220 Algorithms Fall Semester 2016
Homework Project 4
Given 11/30/2016, Due 12/14/2016
Write a function that implements the Rabin-Karp algorithm and tests a long string
against an array of possible pattern strings.
int substring(char * text, int k, int m, (char *) patterns[]);
The function returns -1 if no pattern was found, and i if pattern[i] was found in
text. Here text is a \0-terminated string, and patterns is an array of k pointers to
\0-terminated strings of length m.
The size of the hash table that you use for the Rabin-Karp algorithm should be a
prime number p greater than 1000, and the base of the polynomial should be a random
integer between 1 and p−1 remember to reduce numbers modulo p after each arithmetic
operation during the computation of the hash function, so you have no