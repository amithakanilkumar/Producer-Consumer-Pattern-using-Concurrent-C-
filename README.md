# Producer-Consumer-Pattern-using-Concurrent-C-

**Introduction:**  
This project demonstrates the classic **Producer–Consumer Problem** implemented using **Concurrent C++** features such as threads, mutexes, and condition variables.  
It showcases how multiple **producer threads** generate data and multiple **consumer threads** retrieve and process it safely using a **thread-safe queue**.  
The main goal is to ensure **synchronized access** to shared data without race conditions or data loss.

---

## Installation Instructions

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

command to compile (with threading support):
g++ -std=c++20 -pthread main.cpp -o producer_consumer

### Step 5 — Run the Program

execute the program
./producer_consumer

### Step 6 — Optional (Clean Up / Re-run)

If you modify your code and want to recompile:
rm producer_consumer
g++ -std=c++20 -pthread main.cpp -o producer_consumer
./producer_consumer

### Step 7 — Verify Threading Support (Optional Check)

Check whether your system supports threads:
lscpu | grep -i "core"

### Usage
The program demonstrates a classic Producer–Consumer system implemented using Concurrent C++.
It uses multiple producer threads to generate data and consumer threads to process it concurrently.
A thread-safe queue ensures synchronized access between producers and consumers using mutex and condition variables.

###  How_to_run:
  
    - Step 1: Open the Linux terminal in your project folder.
    - Step 2: Compile the program using:
        command: g++ -std=c++20 -pthread main.cpp -o producer_consumer
    - Step 3: Run the executable:
        command: ./producer_consumer
    - Step 4: Observe producers generating data and consumers processing it concurrently.

  
### Expected_output:

    Producer 1 produced 101
    Producer 2 produced 201
        Consumer 1 consumed 101
        Consumer 2 consumed 201
    Producer 1 produced 102
        Consumer 1 consumed 102
    Main thread exiting...

### Features:

  - Multi-threaded producer–consumer model using C++ threads.
  - Thread-safe queue implemented with std::mutex and std::condition_variable.
  - Safe and synchronized communication between threads.
  - Efficient waiting and notification without busy-waiting.
  - Scalable design — supports multiple producers and consumers.
  - Demonstrates real-world concurrency principles.



