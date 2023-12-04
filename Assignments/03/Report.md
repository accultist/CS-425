# Results for Assignment 03

## Assignment 03 Overview (from description)

This project focuses on task-based parallelism, which builds on your previous knowledge of threads, synchronization primitives, and other parallel-computing techniques.

For this project you will increase the performance of a simple Web server by parallelizing it.

For this project, due to its networking nature, please run all the executable programs on blue.cs.sonoma.edu.

## Improvement Iterations

Here's a table showing the improvements during the course of working on the provided files. Version 01 is unmodified, while subsequent versions had changes made. Modifications were only done to the lychrel.cpp file, all other files were left unchanged.

| Version | Time (Finish) |  File Requests |  Data Transferred | Speedup (real) |  Change Comments |
| :-----: | ----------- | ------------ | ----------- | :-----: | ------- | 
| 01 | 0m44.12s | 348 | 559.54 MB | &mdash; | Initial version - no changes |
| 02 | 0m25.97s | 297 | 559.54 MB | 1.70x | Implemented threading |
| 02.1 | 0m27.51s | 297 | 559.54 MB | 0.94x | Cleanup & comments |



## Initial Analysis
Program works as expected, taking the stock images sourced from the blue server. Untouched, the program pulls images although slowly one by one leading to a domino effect of images loading in. I believe most, if not all, of the optimizing will take place within server.cpp when creating multiple threads.

### Additional comments

## Version 2
Additional changes were made to server.cpp, most significantly adding threading to handle the requests made from the client to the server, and the response from the server. Minor changes were made to Connection.h to prevent any errors as shown in the Connection.h file.



