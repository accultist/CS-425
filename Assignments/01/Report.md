# Results for Assignment 01

## Improvement Iterations

Here's a table showing the improvements I did to make the application go faster.  Versions 01-09 are composed of optimization when compiled with g++ via command line.

| Version | Time | Speedup | Memory (KB) | Changes |
| :-----: | ---- | :-----: | :------: | ------- |
| 01 | 9.51s | &mdash; | 1041304 | Initial version - no changes |
| 02 | 3.27s | 2.91x | 1041332 | Compiled with O1 basic optimization level |
| 03 | 2.18s | 1.50x | 1041328 | Compiled with O2 moderate optimization level |
| 04 | 2.16s | 1.01x | 1041300 | Compiled with O3 high optimization level |
| 05 | 3.83s | 0.56x | 1041324 | Compiled with Os size optimization |
| 06 | 1.87s | 2.05x | 1041332 | Compiled with Ofast O3 optimization w/ some more aggressive optimizations |
| 07 | 9.74s | 0.19x | 1041336 | Compiled with flag 'march=native' which generates code optimized for the host machine architecture |
| 08 | 9.45s | 1.03x | 1041320 | Compiled with link-time optimization |
| 09 | 9.91s | 0.95x | 1041332 | Compiled with flag 'funroll-loops' which unrolls loops in the code |

## Profiling Analysis

### Optimization through command line analysis

Out of all of the versions 01 to 09 which were optimized when compiled via command line, I had found that for the given program 01.cpp that version 06 had the fastest run time when run as an application. While version 04 had the smallest memory footprint when compared to all of the other options. It should be noted that both versions 04 and 06 had O3 optimization when compiled, yet version 06 had extra optimizations tacked on top leading to a shorter run time for the application. It is interesting to see how version 06 was the fastest, yet used more memory when compared to version 04. Though this differance in memory usage is only 32kb and has minimal impact on modern operating systems.


