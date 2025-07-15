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

### 13. what are device drivers? what is it uses?
A device driver is a software that helps the operating system communicate with hardware devices.

#### Uses:

1. It controls how hardware devices work.
2. It helps the OS to detect and use the device.
3. It acts as a link between OS and hardware.
4. It supports plug-and-play, so devices work easily when connected.

#### Explanation:
Device driver ek chhoti software hoti hai jo OS aur hardware ke beech connection banata hai. Jaise jab aap mouse ya printer lagate ho, to driver batata hai OS ko ki usse kaise handle karna hai. Agar driver nahi ho, to hardware properly kaam nahi karega. Isse OS ko device ko samajhne aur control karne me aasani hoti hai.

### 14. how linux is diffrent from windows server?
1. Linux is open-source and free, while Windows Server is paid and closed-source.
2. Linux mostly uses command-line, while Windows Server has graphical interface by default.
3. Linux is popular for web servers and development, Windows Server is used in corporate networks.
4. Linux supports many distributions (like Ubuntu, CentOS), Windows Server has limited versions from Microsoft.

#### Explanation:
Linux ek free aur open-source system hai jahan user code ko modify kar sakta hai. Isme jyadatar kaam terminal (command line) se hota hai. Web hosting aur programming ke liye use hota hai.
Windows Server Microsoft ka banaya hua hai, paid hota hai, aur mostly companies ke IT system me use hota hai. Isme GUI hota hai jo beginners ke liye easy hota hai.

### 14. describe the essential properties of the following types of operating system:
a. Batch <br/> 
b. time sharing <br/> 
c. real time 

#### a. Batch Operating System (4 Marks)
In Batch OS, similar jobs are grouped together and processed without user interaction. The system runs them one after another in a batch.

#### Key Properties:

1. Jobs are collected and executed in batches.
2. No user interaction during execution.
3. Suitable for long and repetitive tasks.
4. Less costly than manual execution.

#### Explanation:
Batch OS me user directly interact nahi karta. Sabhi similar jobs ko ek sath batch me daal diya jata hai aur wo system automatically run karta hai. Jaise salary process karna, billing reports banana – ek hi type ka kaam ek sath complete hota hai.

#### b. Time-Sharing Operating System (4 Marks)
In Time-Sharing OS, multiple users can use the computer at the same time. CPU gives each user a small amount of time to run their task.

#### Key Properties:

1. Multiple users work together using time slices.
2. CPU time is shared among users.
3. Response time is fast.
4. Used in systems where many users work together.

#### Explanation:
Is system me ek hi computer par kai users apna kaam ek sath kar sakte hain. CPU har user ko thoda-thoda time deta hai, isse lagta hai ki sabhi ka kaam ek sath ho raha hai. Jaise ek computer lab me sabhi students same computer system se connected hote hain.

#### c. Real-Time Operating System (RTOS) (4 Marks)
RTOS is used where tasks must be done within a fixed time. It gives fast and predictable responses to inputs.

#### Key Properties:

1. Works within strict time limits.
2. Fast and accurate response.
3. Used in medical, robotics, or aircraft systems.
4. Supports critical and time-sensitive operations.

#### Explanation:
RTOS un jagahon par use hota hai jahan delay allowed nahi hota – jaise rocket launch, pacemaker, ya automatic car brakes. Har task ko time ke andar complete karna hota hai, warna system fail ho sakta hai. Isme timing sabse important hoti hai.

### 15. explain different services provided by an operating system and how each provides convenience to the users.
An operating system provides several key services that help users interact with the computer easily and efficiently. These services include:

#### 1. User Interface (UI):
What it does: Allows users to interact with the system (CLI or GUI).
Convenience: GUI makes it easy to click icons and run apps without commands.

#### explanation:
User Interface help karta hai user ko system ke saath interact karne me. GUI me user easily mouse se kaam kar sakta hai — commands yaad karne ki zarurat nahi hoti.

#### 2. Program Execution:
What it does: Loads programs into memory and runs them.
Convenience: Users can easily start apps like browsers, games, etc.

#### explanation:
Jab bhi user koi program open karta hai, OS usse memory me load karke chalata hai. Ye process user ke liye automatic aur simple bana deta hai.

#### 3. File Management:
What it does: Manages files on disk (creation, reading, writing, deletion).
Convenience: Users can organize data into folders and access it easily.

#### explanation:
OS user ke liye data ko file aur folders me manage karta hai. Jaise Documents, Photos alag-alag folders me save kar sakte ho.

#### 4. Memory Management:
What it does: Manages RAM by allocating space to programs.
Convenience: Ensures smooth multitasking without crashes.

#### explanation:
Jab multiple programs chal rahe hote hain, OS decide karta hai kisko kitni memory mile. Isse system slow nahi hota aur saare programs smoothly chalte hain.

#### 5. Device Management:
What it does: Controls hardware like printers, keyboards, etc.
Convenience: User can plug and play devices without any complex setup.

#### explanation:
Jab aap USB ya printer lagate ho, OS usse detect karke use ready karta hai. User ko kuch manually install nahi karna padta.

#### 6. Security and Protection:
What it does: Protects system from unauthorized access.
Convenience: Login system, password protection keeps user data safe.

#### explanation:
OS user ka data secure karta hai passwords, login systems ke through. Kisi aur ko system access nahi milta bina permission ke.

#### 7. Error Detection and Handling:
What it does: Finds and fixes system errors.
Convenience: Shows messages when issues occur and helps solve them.

#### explanation:
Agar system me koi error hota hai, OS usse detect karta hai aur user ko notify karta hai, jaise “Not Responding” ya “Low Memory” messages.

#### Conclusion:
These OS services make computers user-friendly, manage resources efficiently, and keep systems secure and responsive.

### 16. explain process synchronization with the help of suitable examples 
Process synchronization means managing processes so they can run together without interfering with each other, especially when they share resources like files, memory, or printers.

It helps avoid problems like race conditions, where two processes access shared data at the same time and give incorrect results.

####  Why Synchronization is Needed:
When multiple processes access the same resource, we must make sure only one uses it at a time.

#### Example:
<b>Bank Account System: <b></br>

Suppose two processes are trying to update the same bank account balance. One is adding ₹500, the other is withdrawing ₹300. Without synchronization, both may read the old balance at the same time, and the final balance may be incorrect.

####  With Synchronization (Using Lock):
First process locks the account, adds ₹500, unlocks it. Then second process locks, subtracts ₹300, and unlocks. Now the final balance is correct.

#### Common Synchronization Tools:
1. Semaphore: Used to control access to shared resources.
2. Mutex (Mutual Exclusion): Only one process enters critical section at a time.
3. Monitor: High-level structure to handle synchronization easily.

#### explaination
Process synchronization ka matlab hai – jab 2 ya zyada process ek hi resource (jaise memory, file, account balance) use kar rahe ho, to unko aapas me coordinate karna taaki data kharab na ho.

Agar dono process ek sath balance update kare bina control ke, to result galat aayega. Isliye synchronization tools jaise mutex ya semaphore use hote hain jisse ek process ek time pe kaam kare, doosra wait kare.
