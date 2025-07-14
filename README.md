# Operating-System
Questions for main exams 

### 1. what is the main reason of designing an operating system?
#### Definition:
The main reason for designing an operating system is to manage hardware and provide a platform for software.

#### Explanation:
OS hardware (CPU, memory, etc.) ko control karta hai aur users ko ek simple interface deta hai programs run karne ke liye.

### 2. what are  system calls?
#### Definition:
System calls are the way through which a program requests services from the operating system.

#### Explanation:
Jab koi program OS se kuchh kaam karwana chahta hai (jaise file read/write), to wo system call ke through OS se baat karta hai.

### 3. what is priority scheduling?

#### Definition:
Priority scheduling is a CPU scheduling algorithm that executes processes based on their priority.

#### Explanation:
Jis process ki priority zyada hoti hai, usse pehle CPU milta hai. Agar 2 processes ki priority same ho, to wo order of arrival se decide hota hai.

### 4. what is context switching?
#### Definition:
Context switching is the process of saving the state of one process and loading the state of another.

#### Explanation:
Jab CPU ek process se dusre par switch karta hai, to pehle current process ka data save karta hai aur naye process ka data load karta hai—isse hi context switching kehte hain.

### 5. What is page fault?
Definition:
A page fault occurs when a program tries to access a page that is not currently in main memory.

Explanation:
Jab required data RAM me nahi hota aur hard disk se lana padta hai, to us situation ko page fault kehte hain.

### 6. what is thrashing?
#### Definition:
Thrashing is a condition where the system spends most of its time swapping pages instead of executing processes.

#### Explanation:
Jab RAM me jagah kam hoti hai aur bar-bar pages load/unload hote hain, to CPU useful kaam kam aur swapping zyada karta hai—isse system slow ho jata hai.

### 7. what are various file operations?
#### Definition:
File operations are actions performed on files to manage data.

#### Explanation:
Main file operations hain:<br/>
Create – nayi file banana<br/>
Open – file ko access ke liye kholna<br/>
Read – file se data lena<br/>
Write – file me data dalna<br/>
Close – kaam ke baad file band karna<br/>
Delete – file ko remove karna

### 8. Name various file attributes ?
#### Definition:
File attributes are properties that define a file’s characteristics and behavior.

#### Explanation:
Kuch common file attributes hain:<br/>
Name – file ka naam<br/>
Type – file ka format (e.g., .txt, .jpg)<br/>
Size – file ki memory size<br/>
Location – file ka storage path<br/>
Creation Time – kab file bani<br/>
Access Rights – kaun read/write kar sakta hai<br/>
Modified Time – last time file me change कब हुआ

### 9. what is kernel?
#### Definition:
Kernel is the core part of an operating system that controls all system operations.

#### Explanation:
Kernel hardware (CPU, memory, devices) aur software ke beech bridge ka kaam karta hai. Ye hi decide karta hai ki kaun sa process kab chalega aur resources kaise use honge.

### 10. list any four shells available in linux
#### Definition:
Shell is a command-line interface that allows users to interact with the operating system.

#### Explanation:
Linux me commonly used 4 shells hain:<br/>
Bash (Bourne Again Shell)<br/>
Sh (Bourne Shell)<br/>
Csh (C Shell)<br/>
Ksh (Korn Shell)<br/>

### 11. explain the three most important functions of operating system?
#### Process Management:
OS handles the creation, scheduling, and termination of processes.
It ensures each process gets enough CPU time and manages multitasking.

#### Memory Management:
OS keeps track of each byte in memory and manages allocation/deallocation.
It ensures that one process doesn’t interfere with another’s memory.

#### File Management:
OS manages files on storage devices – creation, reading, writing, and deletion.
It maintains file hierarchy (directories) and access permissions.

### 12 explain all the states of a process with the help of neat labelled diiagram?
#### Process States:
New: Process is being created.<br/>
Ready: Process is waiting to be assigned to the CPU.<br/>
Running: Process is currently being executed by the CPU.<br/>
Waiting (or Blocked): Process is waiting for some event (like I/O) to occur.<br/>
Terminated: Process has finished execution.

               +--------+
               |  New   |
               +--------+
                   |
                   v
               +--------+        I/O Wait
    +<-------- | Ready  | <----------------+
    |          +--------+                 |
    |               |                     |
    |               v                     |
    |          +--------+                 |
    |          | Running| --------------> +--------+
    |          +--------+     I/O         |Waiting |
    |               |                    +--------+
    |               v                        |
    |          +--------+ <-----------------+
    +--------> | Exit   |
               +--------+

### 13. what are the limitations of contiguous memory allocation?
#### Contiguous Memory Allocation:
In this method, each process is allocated a single continuous block of memory.

