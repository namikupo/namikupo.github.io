---
title: "Super cool blog post title thingie"
---
this is a super duper cool first post

So just to write it down:
Algorithm-based compression.
The idea is to take data, and compress it by generating an algorithm that generates the data.
As a basic example, for a program that consists of the bits "11110000" i'd want to generate an algorithm that generates the bits "11110000".
I'm imagining that it's some sort of equation, which given a number generates a value between 0 and 1. By rounding either up or down it'll generate the numbers.
The expression would either have to generate a single bit/byte, repeating the operation until the data is generated.
A downside of doing it this way, is that it would require potentially many iterations of the algorithm to generate the data. Long time/much power.
This would mean that the compressed file contains no data, but the algorithm/expression to generate it.
I believe this has the potential to reduce files sizes.

x = d, where x is the algorithm and d is the data
d will be a series of values between 0 and 1.
x will be an expression that generates a series of values between 0 and 1

Ideal use would be something like:
Terminal: AlgoCompression compress data.type
Output: dataAlgorithm.AC

Terminal: AlgoCompression generate dataAlgorithm.AC
Output: data.type

could verify output via checksums