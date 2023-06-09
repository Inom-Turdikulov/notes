---
date: 2023-04-13
draft: true
tags:
- inbox
- definition
- CS-tip
sr-due: 2023-05-20
sr-interval: 3
sr-ease: 269
---

# Computer memory

Memory can be viewed as a giant collection of cells. Each cell is a single byte
of data and has own address, where one number greater than the previous cell's
address.

|     | 0    | 1    | 2    | 3    | 4    |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 0   | 1000 | 1001 | 1002 | 1003 | 1004 |
| 1   | 1005 | 1006 | 1007 | 1008 | 1009 |
| 2   | 1010 | 1011 | 1012 | 1013 | 1014 |
| ... | ...  | ...  | ...  | ...  | ...  |

## Facts about computer memory

A computer can jump to any memory address ==in one== step.
<!--SR:!2023-11-30,179,270-->

When computer allocate an array, it also store arrays
==address, at which memory addresses the array begins==.
