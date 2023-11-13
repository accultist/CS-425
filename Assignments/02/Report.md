# Results for Assignment 02

## Assignment 02 Overview (from description)

This project is to reinforce your learning of threads and synchronization for computational applications.  In this assignment, you will convert a serial program that searches for the largest non-Lychrel number (i.e., the number that makes the most iterations without diverging) from provided lists of numbers to a multi-threaded version.

Additionally, you're asked to implement a dynamically-scheduled version of the threaded application to maximize throughput (i.e., minimize the running time of the application).  You're permitted to employ any (and all) optimization techniques we've discussed in class. 

## Improvement Iterations

Here's a table showing the improvements during the course of working on the provided files. Version 01 is unmodified, while subsequent versions had changes made. Modifications were only done to the lychrel.cpp file, all other files were left unchanged.

| Version | Time (real) |  Time (user) |  Time (sys) | Speedup (real) |  Changes |
| :-----: | ----------- | ------------ | ----------- | :-----: | ------- | 
| 01 | 0m17.840s | 1m55.522s | 0m0.060s | &mdash; | Initial version - no changes |
| 02.1 | 0m17.223s | 1m53.579s | 0m0.061s | 1.04x | Incorporated "else" clause before output |
| 02.2 | 0m17.080s | 1m53.816s | 0m0.041s | 1.01x | Slight reformatting of "else" clause modified |


## Initial Analysis

### Additional comments




