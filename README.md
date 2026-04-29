# HEALTH-QUEUE---Greedy-Algorithm
🏥 Patient Appointment Scheduling using Greedy Algorithm

This project implements a Greedy Algorithm approach in C to efficiently allocate limited doctor consultation time among multiple patients based on their emergency priority.

🚀 Overview

In real-world healthcare scenarios, doctors often have limited time while patients have varying levels of urgency. This program prioritizes patients with higher emergency percentages and allocates available consultation time accordingly.

The algorithm ensures that:

Patients with higher emergency levels are served first
Available time is utilized optimally
Partial allocation is allowed if time runs out
⚙️ Features
Sorts patients based on emergency priority (descending)
Allocates consultation time using a greedy strategy
Supports:
Interactive mode (user input via terminal)
Machine mode (--machine or -m) for automated input/output (JSON format)
Handles invalid inputs and memory allocation errors safely
🧠 Algorithm Used

This program uses a Greedy Algorithm, where:

Patients are sorted by highest emergency percentage
Time is allocated sequentially:
If full time is available → assign completely
If not → assign remaining time (fractional allocation)

This approach is similar to the Fractional Knapsack Problem.

📥 Input Format
Interactive Mode:
Number of patients
Patient details:
Name
Emergency percentage
Required consultation time
Total available doctor time
Machine Mode:
n
name1 emergency1 req_time1
name2 emergency2 req_time2
...
totalSlots
📤 Output
Displays a priority-based appointment schedule
Shows:
Patient Name
Emergency %
Required Time
Allocated Time
In machine mode, outputs structured JSON
🛠️ Compilation & Usage
gcc scheduler.c -o scheduler
./scheduler

Machine mode:

./scheduler --machine < input.txt
📌 Use Cases
Hospital appointment systems
Emergency resource allocation
Task scheduling with priority constraints

📄 License
This project is open-source and free to use for educational purposes.
