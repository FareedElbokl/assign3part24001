# Teaching Assistant Marking System

## Overview

This program simulates five Teaching Assistants (TAs) marking student exams concurrently. Each TA accesses a shared database (via shared memory) and marks students while following a semaphore-based protocol to prevent deadlock and livelock. The goal is to ensure that only two TAs access the database at the same time.

Each TA writes their marks to their own file (`TA1.txt`, `TA2.txt`, ..., `TA5.txt`). The program ends when all TAs have marked all students three times.

---

## Prerequisites

To compile and run the program, ensure you have:

- A Unix/Linux system.
- GCC (GNU Compiler Collection) installed.
- Basic familiarity with terminal commands.

---

## Compilation Instructions

To compile the program:

1. Open a terminal.
2. Navigate to the directory containing the source code file (e.g., `program.c`).
3. Use the following command to compile:
   ```bash
   gcc -o TA_MarkingSystem program.c
   ./TA_MarkingSystem
   ```
