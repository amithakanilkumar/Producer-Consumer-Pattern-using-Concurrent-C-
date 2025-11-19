# Producer-Consumer-Pattern-using-Concurrent-C-

**Introduction:**  
This project demonstrates the classic **Producer–Consumer Problem** implemented using **Concurrent C++** features such as threads, mutexes, and condition variables.  
It showcases how multiple **producer threads** generate data and multiple **consumer threads** retrieve and process it safely using a **thread-safe queue**.  
The main goal is to ensure **synchronized access** to shared data without race conditions or data loss.

---

## ⚙️ Installation Instructions

Follow these steps to compile and run the project on a Linux system.

### Step 1 — Check if C++ is Installed

First, check if the GNU C++ compiler ('g++') is installed:

g++ --version

If not, install it using:

sudo apt update
sudo apt install g++


### Step 2 — Add the Source Files

Create the two files inside the folder:
nano thread_safe_queue.h

Then create the main program:
nano main.cpp

### Step 4 — Compile the Program

