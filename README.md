# Text/Binary Conversion

A text based application that takes formatted ASCII or binary characters and converts them to the other, respectively. The goal of this project was to:

- Read and write text from files using BufferedReader/BufferedInputStream and DataOutputStream/PrintWriter
- Use switch statements to code flow
- Learn to use a ByteBuffer

## Introduction

ASCII characters are represented as 8 bit binary numbers, which are abstracted away from text files. This program attempts to lift that abstraction and allows for easy conversion between text and binary files. It takes 3 arguments: the conversion type, the input file, and the output file.

`convertBinaryToText` does as the name suggests. The code scans through the file for however long its specified length is, and learns to interpret the binary text using a **ByteBuffer**. Based on the initial character, the code knows whether the following bits are integers, doubles, longs, arrays, strings, etc. and makes the appropriate changes.

`convertTexttoBinary` also does as the name suggests. The code scans through the file until it reaches the end, and uses keywords to help in the conversion. The keywords range from numbers like int, float, long, etc. and strings.

***The two functions are antitheses.*** If a file is converted from text to binary, then back to text, the content will remain unchanged.

I have provided some test files that I used while creating the program. Their structure is ideal with how my code runs. If yours is formatted differently, my code will not run properly.

## Runtime Example

## Aknowledgements

An early project of CS210. The credit for this idea goes to Professor David Garrison of Binghamton University. The implementation of the code was my own.
