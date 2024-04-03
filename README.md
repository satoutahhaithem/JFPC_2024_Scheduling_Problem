# Scheduling Problem for Rodef 
This repository contains a Python program designed for scheduling conference sessions for the ROADEF Challenge in [2024,2023,2022]. The program utilizes constraint satisfaction and optimization techniques to efficiently allocate sessions, respecting various constraints like the number of papers, parallel sessions, and working group conflicts.

## Getting Started

### Prerequisites
Before running the program, ensure you have Python 3 and pip installed on your system. The program also relies on several Python packages, including NumPy and PySAT.
### Install Required Packages:
```bash
pip install numpy
pip install python-sat[pblib,aiger]

```
# Running the Program
Replace [year] with the dataset year you wish to process (2022, 2023, or 2024).

For example:

```
python3 Scheduling_Problem.py 2024
```

# Data
The datasets provided correspond to the years 2022, 2023, and 2024. Each dataset contains specific configurations for conference sessions, including session count, time slots, paper ranges, and working groups.

# Program Overview

The script performs the following key operations:

Loads the dataset based on the specified year.
Sets up various constraints like session-slot-paper combinations and working group conflicts.
Utilizes PySAT to solve the scheduling problem.
Outputs the optimal scheduling arrangement.
