# CN Assignment 1:
Tejas Lohia - 23110335
Umang Shikarvar - 23110301

## Overview
This repository contains the implementation and report for **CN Assignment 1**.  
Two folders:

- **Task 1** – Code and files for **Part A** of the assignment  
- **Task 2** – Code and images for **Part B**

A report (`report.pdf`) for the assignment is included.  
The `report/` folder contains the LaTeX source (`.tex`) and the generated PDF.

---

## Directory Structure
```
.
├── Task1/           # Client and server implementation for Part A
├── Task2/           # Code and images for Task 2
├── report/          # LaTeX source files and compiled report
└── report.pdf       # Final assignment report
```

---

## Task 1: Running the Code

### Prerequisites
- **C compiler** (e.g., `gcc`)
- **Python 3.x**
- **pcap6 file** (download separately)
- Python virtual environment (`venv`)

### Setup & Execution

1. **Download the pcap6 file** and place it in the `Task1/` folder.

2. **Navigate to Task1**:
   ```bash
   cd Task1
   ```

3. **Create and activate a virtual environment**:
   ```bash
   python3 -m venv assign1
   source assign1/bin/activate
   ```

4. **Install required package**:
   ```bash
   pip install socket
   ```

5. **Run the server**:
   ```bash
   python dnsserver.py
   ```

6. **Compile and run the client**:
   ```bash
   gcc -o test pcapclient.c
   ./test
   ```

---

## Output
After running the client, two files are generated:

- **`dnsReport.txt`** – Final DNS query results with resolved IP addresses  
- **`dns.txt`** – Raw DNS packet data

---

## Implementation Notes
- **Client:** Implemented in **C** to explore low-level sockets, system calls, and system design.  
- **Server:** Implemented in **Python** for ease of handling and testing.

---

## Report
The final report is available as **`report.pdf`**, with LaTeX sources in the `report/` directory.
