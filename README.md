# Operating-System

## First Paper: 

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
    +--------> |  Exit  |
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
Windows Server M icrosoft ka banaya hua hai, paid hota hai, aur mostly companies ke IT system me use hota hai. Isme GUI hota hai jo beginners ke liye easy hota hai.

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

### 17. what is deadlock? give an appropriate example. Explain the four necessary conditions for deadlock to occur?
A deadlock is a situation where two or more processes are waiting for each other to release resources, and none of them can continue.

####  Example:
1. Process A holds Resource 1 and needs Resource 2 to continue.
2. Process B holds Resource 2 and needs Resource 1.
3. Both are waiting for each other → this causes deadlock.

####  Real-Life Example (Simple):
Two people are in a narrow hallway, each blocking the other. Neither moves back, so both are stuck — that’s a deadlock.

#### Four Necessary Conditions for Deadlock:
##### Mutual Exclusion
Only one process can use a resource at a time.

##### Hold and Wait
A process is holding at least one resource and waiting for others.

##### No Preemption
Resources cannot be forcibly taken from a process.

##### Circular Wait
A set of processes are waiting on each other in a circular chain.

#### Conclusion:
If all four conditions are true at the same time, a deadlock can occur. OS must use methods to prevent or handle it.

### 18. what is the need for page replacement? explain LRU page replacement algorithms with the help of an example.
Page Replacement is needed when a program needs a page that is not in memory (called a page fault), and the memory is already full. So, the system must decide which old page to remove to bring the new one in.

#### Why Page Replacement is Needed?
1. RAM has limited space.
2. When all frames are full and a new page is needed, we must replace an old one.
3. This helps in efficient memory use and allows programs to run smoothly.

#### LRU (Least Recently Used) Algorithm:
LRU removes the page that has not been used for the longest time. It assumes that pages used recently will likely be used again soon.

#### Explanation:
Page replacement ki jarurat tab padti hai jab system ki memory full ho aur koi nayi page memory me laani ho. LRU algorithm us page ko hataata hai jo sabse pehle use hua tha – yani jo sabse kam recent tha. Example me, jab 4th page aayi (2), aur memory full thi, to system ne 7 ko hata diya kyunki wo sabse purana tha. Is tareeke se memory efficiently manage hoti hai.

### 19. Explain any two file allocation methods.
File allocation methods define how files are stored in memory blocks on a disk. Two common methods are:

#### 1. Contiguous Allocation 
##### Definition:
In this method, entire file is stored in a single continuous block of memory.
##### Advantages:
1. Simple to implement.
2. Fast access (direct access possible).

##### Disadvantages:
1. Causes external fragmentation.
2. Difficult to grow files if space isn’t available after current block.

#### Example:
If a file needs 4 blocks, it will be stored in blocks 10 to 13 continuously.

#### Explanation:
Is method me file ko ek saath continuous jagah milti hai disk me. Jaise file ko 4 blocks chahiye, to wo block 5, 6, 7, 8 me save hogi. Simple hai, lekin agar uske baad space na ho to file ko bada karna mushkil hota hai.

#### 2. Linked Allocation

##### Definition:
In this method, file blocks are scattered anywhere on disk, but each block has a pointer to the next block.

##### Advantages:
1. No external fragmentation.
2. Easy to grow file size.

##### Disadvantages:
1. Slower access (no direct access).
2. Pointer takes extra space.

#### Example:
File stored in blocks 5 → 11 → 2 → 8 (each pointing to next).

#### Explanation:
Is method me file ke blocks kisi bhi jagah ho sakte hain, lekin har block ke andar agle block ka address hota hai. Jaise ek train ke bogie me agle bogie ka number likha ho. Isse space ka achha use hota hai, lekin access thoda slow ho jata hai.


### 20. What are the functions of device management? Explain memory mapped I/O.
#### Functions of Device Management:
Device management is a part of the operating system that handles all input/output (I/O) devices like keyboard, mouse, printer, etc.

#### Main Functions:
##### Device Communication:
OS manages communication between devices and the CPU.

##### Device Allocation:
Assigns devices to processes when needed.

##### Device Monitoring:
Keeps track of which device is busy or free.

##### Error Detection:
Detects and handles errors in device operations.

##### Driver Interface:
Uses device drivers to help OS interact with hardware.

#### Memory-Mapped I/O:
##### Definition:
In memory-mapped I/O, input/output devices are treated like memory locations. Each device is assigned a memory address.

##### How it works:

The CPU reads/writes to I/O devices using normal memory instructions. No separate I/O instructions are needed.

#### Example:
Suppose a printer is mapped to address 0x8000. To send data, CPU just writes to that address like it would write to RAM.

####  Explanation:
Device management ka kaam hai sabhi devices ko manage karna – kab kis process ko kaunsa device mile, kaunsa device free hai, aur agar device fail ho jaye to OS usse handle kare.<br/> <br/>
Memory-mapped I/O me devices ko memory ke address ki tarah treat kiya jata hai. Jaise aap RAM me value store karte ho, waise hi printer ya display ko bhi ek address assign karke usme data bhej dete ho. Isse CPU ko alag I/O instruction chalane ki zarurat nahi padti – simple memory access se kaam ho jata hai.

### 21. Discuss the features of Linux OS which make it a popular operating system.
Linux is a popular operating system used worldwide due to its powerful features and flexibility. Some key features are:

#### 1. Open Source:
Linux is free to use and its source code is open for anyone to view, modify, or improve.

#### 2. Security:
Linux provides strong user permissions, file security, and fewer chances of getting viruses.

#### 3. Stability and Performance:
It can run for years without crashing or needing a reboot. It uses system resources efficiently.

#### 4. Multitasking:
Linux can run many processes at the same time without slowing down the system.

#### 5. Portability:
Linux runs on almost all hardware platforms — from smartphones to supercomputers.

#### 6. Community Support:
Millions of developers support Linux, providing updates, fixes, and tutorials.

#### 7. Customizable:
Users can change the desktop, features, and even the kernel according to their needs.

#### Conclusion:
Due to its security, speed, free availability, and flexibility, Linux is a favorite among developers, students, and companies.

### 22. explain the file system available in linux.
A file system defines how data is stored, organized, and accessed on a disk. Linux supports many file systems for different purposes.<br/><br/>

Here are some commonly used file systems in Linux:
 #### 1. ext2 (Second Extended File System):
   - Oldest Linux file system.
   - Does not support journaling.
   - Still used in USB drives and memory cards.

#### Explaination:
ext2 simple file system hai, lekin isme crash ke baad data recovery mushkil hoti hai kyunki journaling nahi hoti.

####  2. ext3 (Third Extended File System):
  - ext2 ka improved version.
  - Supports journaling (keeps logs of changes for recovery).
  - More stable and secure.

#### Explaination: 
ext3 me agar system crash ho jaye to data recover ho sakta hai kyunki ye changes ka record rakhta hai.

#### 3. ext4 (Fourth Extended File System):
  - Most commonly used Linux file system today.
  - Faster, supports large files, and very reliable.
  - Backward compatible with ext3 and ext2.

#### Explaination:
ext4 sabse advanced aur fast file system hai jo Linux me mostly use hota hai. Ye bade size ke files handle kar sakta hai easily.

#### 4. XFS:
  - High-performance file system.
  - Best for handling large files and high-speed data transfer.
  - Often used in servers and enterprise systems.

#### Explaination: 
XFS large data aur fast operations ke liye design kiya gaya hai — jaise video editing, database servers me use hota hai.

#### 5. Btrfs (B-tree File System):
  - Advanced features like snapshots, compression, and error detection.
  - Still under development but powerful.

#### Explaination: 
Btrfs ek modern file system hai jo data ko auto-repair, compress aur snapshot ke saath manage karta hai. Future me zyada use ho sakta hai.

#### 6. Swap File System:
  - Used for virtual memory (acts as extra RAM).
  - Not used for storing files, but helps in performance.

#### Explaination: 
Swap space system me RAM kam padne par kaam aata hai — jaise memory full ho to ye temporary RAM ki tarah kaam karta hai.

#### Conclusion:
Linux offers multiple file systems for different needs — ext4 for general use, XFS for large files, and Btrfs for advanced features.


## Second Paper:

### 1. what do you mean by operating systme?
An Operating System (OS) is system software that manages computer hardware and allows users to run applications.

#### Explanation:
Operating system ek software hota hai jo computer ko chalata hai — jaise Windows, Linux. Ye user aur hardware ke beech bridge ka kaam karta hai.

### 2. Discuss the goal of 'Authentication'?
The goal of authentication is to verify the identity of a user or system before giving access to data or resources.

#### Explanation:
Authentication ka main goal hota hai ye confirm karna ki user wahi hai jo woh claim kar raha hai — jaise username-password se login karke system ko dikhana ki aap authorized user ho.

### 3. What is Multiprogramming system?
A multiprogramming system allows multiple programs to be loaded into memory and executed one by one by the CPU.

#### Explanation:
Is system me ek time par kai programs memory me hote hain, aur CPU unhe ek ek karke execute karta hai. Jab ek program wait karta hai (jaise input ka), tab doosra program CPU use karta hai — isse CPU idle nahi rehta.

### 4. Enlist the various services provided by the operating systme.
The main services provided by an operating system are:

1. Program execution
2. File management
3. Memory management
4. Device management
5. Error detection
6. Security
7. User interface

#### Explaination: 
OS user ke programs chalata hai, files aur memory manage karta hai, devices control karta hai, errors detect karta hai, aur security provide karta hai.

### 5. What is System Call?
A system call is a way for a program to request a service from the operating system, like reading a file or printing data.

#### Explaination: 
System call ek method hai jisse program OS se help maangta hai — jaise file open karni ho, ya data print karwana ho. Ye OS aur program ke beech communication ka zariya hai.

### 6. write a definition of process.
A process is a program in execution. It includes the program code, current activity, and resources.

#### Explanation:
Process ka matlab hota hai ek program jo run ho raha ho. Isme program ka code, uski current state (jaise kaunsa instruction chal raha hai) aur jitne bhi resources use ho rahe hain (jaise memory, files) sab included hote hain.

### 7. Enlist the various states of process.
The various states of a process are:

1. New
2. Ready
3. Running
4. Waiting
5. Terminated

#### Explaination: 
1. New – Jab process abhi create hua hai.
2. Ready – Process execution ke liye ready hai, CPU ka wait kar raha hai.
3. Running – Process ko CPU mil gaya hai aur wo execute ho raha hai.
4. Waiting – Process kisi I/O ya resource ke liye wait kar raha hai.
5. Terminated – Process ka kaam complete ho gaya hai, ab band ho gaya hai.

### 8. What is Thread?
A thread is the smallest unit of execution in a process. Multiple threads can run within a single process.

### Explaination: 
Explanation:
Thread ek chhota part hota hai process ka, jo independently kaam kar sakta hai. Agar ek process me multiple threads ho, to wo sab alag-alag kaam parallel me kar sakte hain. Jaise ek browser me ek thread webpage load karta hai aur doosra video play karta hai.

### 9. What do you mean by Logical address?
A logical address is the address generated by the CPU during a program’s execution. It is also called a virtual address.

#### Explanation:
Logical address wo hoti hai jo CPU create karta hai jab program run ho raha hota hai.
Yeh directly RAM (physical memory) ka address nahi hota — balki ek virtual location hoti hai, jo baad me memory management unit (MMU) ke through physical address me convert hoti hai.
Isse programs ko ek clean aur safe memory space milta hai.

### 10. Differentiate between  'File' and 'Directory'?
File is a collection of data or information, such as a document, image, or program.<br/>

Directory is a container that holds multiple files or other directories to organize data.

#### Explaination:
File ek data ka piece hota hai, jaise koi photo, document, ya program.<br/>
Directory ek folder hota hai jo kai files ya sub-directories ko store karta hai, taki data ko achhe se arrange kiya ja sake.

### 10. Discuss various criteria for measuring the performance of scheduling mechanism.
There are several criteria to measure the performance of a CPU scheduling mechanism:

1. CPU Utilization
2. Throughput
3. Turnaround Time
4. Waiting Time
5. Response Time

#### 1. CPU Utilization – 
CPU kitna time idle na rahkar kaam karta hai, jitna zyada utilization, utni achhi performance.

#### 2. Throughput –
Ek specific time duration me kitne processes complete hue, zyada throughput matlab better efficiency.

#### 3. Turnaround Time –
Process submit hone se leke complete hone tak ka total time, jitna kam ho, utna accha.

#### 4. Waiting Time –
Process ko ready queue me wait karna padta hai CPU milne ke liye, ye time kam hona chahiye.

#### 5. Response Time – 
Pehli baar process ko CPU milne me kitna time laga, interactive systems ke liye important hai.

### 11. Write the method of recovery from deadlock.
Deadlock recovery means removing the deadlock situation from the system. The main methods for recovery are:

1. Process Termination – Stop one or more processes to break the deadlock.
2. Resource Preemption – Take resources from some processes and give them to others.
3. Rollback – Move one or more processes back to a safe earlier state and restart them.

#### Explaination: 
Deadlock recovery ka matlab hai jab system deadlock me chala jata hai, to us situation ko hataana ya system ko wapas normal condition me lana.

#### Process Termination
Ek ya zyada processes ko forcibly band kar dete hain. Kabhi-kabhi sabhi deadlocked processes ko terminate kar dete hain, ya ek ek karke terminate karte hain jab tak deadlock khatam na ho jaaye.

#### Resource Preemption
Kisi process se resource wapas le kar kisi doosre process ko de dete hain jise urgently chahiye. Isse system temporarily slow ho sakta hai, lekin deadlock break ho jaata hai.

#### Rollback
Process ko ek safe point (checkpoint) tak wapas le jaakar wahan se dobara start kiya jaata hai. Isse system wapas stable state me aata hai.


### 12. Explain 'Demand Paging' in brief?
Demand Paging is a memory management technique where pages are loaded into memory only when they are needed, not in advance. If a program tries to access a page that is not in memory, a page fault occurs, and the required page is brought from disk to memory.

#### Explaination:
Demand Paging ek technique hai jisme kisi program ke pages tabhi memory me laaye jaate hain jab unki zarurat padti hai. Jaise hi koi program kisi aise page ko access karta hai jo abhi memory me nahi hai, to system ek page fault detect karta hai. Phir wo page hard disk se memory me load kiya jaata hai. Isse memory ka efficient use hota hai, kyunki sirf zarurat ke pages hi memory me rehte hain.

### 13. What do you mean by Encryption? Discuss.
Encryption is the process of converting plain (readable) data into a secret code (called ciphertext) to protect it from unauthorized access. Only those with the correct key can decrypt it back to readable form. It is widely used in emails, websites, and digital payments to ensure privacy and security.

#### Explaination:
Encryption ka matlab hota hai data ko aise code me badalna jise sirf authorized user hi samajh sake. Jab aap koi message bhejte ho (jaise WhatsApp ya online payment), to wo data encrypt ho jata hai — yaani readable text ko ek secret code me convert kar diya jata hai. Agar kisi hacker ne data chura bhi liya, to bina decryption key ke wo us encrypted message ko samajh nahi paayega. Isse data secure aur private rehta hai.

### 14. Discuss 'Process Control Back (PCB)' with the help of proper  illustration. Also, Explain various types of Schedulers.
#### 1. Process Control Block (PCB):
PCB is a data structure used by the operating system to store all information about a process. It acts like an identity card for a process.

#### 2. Types of Schedulers:
Schedulers are OS components that decide which process to run. There are three main types:
  - Long-term Scheduler – decides which new processes enter the system.
  - Short-term Scheduler – decides which ready process runs on the CPU.
  - Medium-term Scheduler – decides which processes should be paused or resumed.

#### Explaination: 
##### 1. PCB (Process Control Block) kya hota hai?
PCB ek special data structure hota hai jo har ek process ke baare mein complete information store karta hai. Jab bhi ek process create hoti hai, to OS uske liye ek PCB banata hai.

##### Isme kya kya hota hai?

  - Process ID (PID): Har process ka ek unique ID.
  - Process State: Jaise Running, Waiting, Ready, etc.
  - Program Counter: Batata hai ki process next kaunsa instruction run karegi.
  - CPU Registers: CPU ke andar ke data save rehte hain.
  - Memory Information: Kitni memory use kar raha hai.
  - I/O Status: Konsi I/O devices use kar raha hai.

##### 2. Types of Schedulers – Scheduler ke prakaar
Schedulers ka kaam hota hai ki kaunsi process CPU pe chalegi, aur system me process ka flow manage karna.
  - (a) Long-term Scheduler: Iska kaam hota hai ki kaunsi new process ko system me allow karna hai. Ye process creation rate ko control karta hai.
  - (b) Short-term Scheduler (CPU Scheduler): Ye sabse active hota hai. Ye har baar tab kaam karta hai jab CPU free hota hai aur decide karta hai ki kaunsi process CPU use karegi.
  - (c) Medium-term Scheduler: Agar system overload ho jaye to ye kuch processes ko memory se nikal kar suspend kar deta hai. Jab system free ho jata hai to inhe resume karta hai.

### 15. Explain various preemptive scheduling mechanisms in detail.
#### What is Preemptive Scheduling?
Preemptive Scheduling is a CPU scheduling method in which the currently running process can be interrupted and the CPU can be allocated to another higher priority process. It is based on priority, time, or remaining execution time. This makes the system more responsive and efficient, especially for real-time or interactive environments.

#### Types of Preemptive Scheduling Algorithms:

##### 1. Round Robin (RR) -
Time Quantum: Each process gets a fixed time to execute (like 2ms or 4ms). If a process doesn’t finish in its quantum, it is preempted and moved to the back of the queue. The next process is then scheduled.

### 16. How can a deadlock situation ne avoided? Discuss.
Deadlock can be avoided by making sure that at least one of the four necessary conditions of deadlock does not occur. We can use methods like Banker's Algorithm or Resource Allocation Graph to avoid deadlock.

#### Explaination:
Deadlock ek aisi situation hoti hai jisme multiple processes ek dusre ke resources ka wait karte hue ruk jaate hain, aur koi bhi process aage nahi badh pata. Isse avoid karne ke liye hume deadlock ke 4 conditions me se kam se kam ek ko break karna padta hai:

##### 1. Mutual Exclusion:
Sabhi resources ko exclusive access dena zaroori nahi. Kuch resources ko shareable banakar is condition ko tod sakte hain.

##### 2. Hold and Wait:
Process ek resource hold kar raha ho aur dusre ka wait kar raha ho — isse avoid karne ke liye, process ko sabhi resources ek hi baar allocate karo ya kuch bhi na do jab tak sab ready na ho.

##### 3. No Preemption:
Resource forcibly kisi aur process se le lo jab zarurat ho, toh deadlock avoid ho sakta hai.

##### 4. Circular Wait:
Ek circular chain jisme har process ek dusre ka resource hold kar raha ho — agar hum sabhi resources ko ek fixed order me allocate karein, toh ye condition break ho jaati hai.

#### Algorithms:
##### Banker's Algorithm:
Pehle check karta hai ki agar resource diya jaaye toh system safe state me rahega ya nahi.

##### Resource Allocation Graph:
Resource-process graph me cycle detect karke hum deadlock avoid kar sakte hain.

### 17. How to detect a 'Deadlock'? Explain.
A deadlock can be detected by checking if there is a circular wait among the processes. We use Resource Allocation Graph (RAG) or Deadlock Detection Algorithm to find if a deadlock has occurred.

#### Explaination:
Deadlock detect karne ka matlab hai check karna ki system me koi aisi situation hai ya nahi jahan processes ek dusre ke resources ka wait kar rahe hain aur koi bhi process aage nahi badh paa raha. Iske liye kuch popular methods hain:

### 18. Discuss 'Single Program Partition', 'Fixed-Sized Partitioning' and 'Variable Sized Partition' memory allocation techniques  in brief.

#### Single Program Partition:
  - In this technique, the entire memory is allocated to a single program.
  - No other program can be loaded until the current one finishes.
  - It is simple but wasteful, as it doesn’t allow multitasking.

#### Fixed-Sized Partitioning:
  - Memory is divided into equal-sized fixed partitions.
  - Each partition can hold only one program at a time.
  - If the program is smaller than the partition, memory is wasted (called internal fragmentation).
  - Easy to manage, but not flexible for different program sizes.

#### Variable-Sized Partitioning:
  - Memory is divided into partitions of different sizes depending on the program's requirement.
  - More efficient use of memory.
  - It may lead to external fragmentation (free space between allocated partitions).
  - Requires compaction to handle fragmentation.

#### Explaination:
1. Single Program Partition – Poori memory sirf ek hi program ke liye hoti hai. Jab tak ek program complete nahi hota, doosra run nahi ho sakta. Bohot simple hai lekin memory ka waste hota hai.
2. Fixed-Sized Partitioning – Memory ko barabar hisson me baant diya jaata hai (fixed size). Har partition me ek hi program aa sakta hai. Agar program chhota ho to bachi hui memory waste ho jaati hai (internal fragmentation).
3. Variable-Sized Partitioning – Memory ko alag-alag size ke parts me divide kiya jaata hai jaisa program ka requirement ho. Ye zyada efficient hai, lekin kabhi-kabhi memory ke beech me khaali space bach jaata hai (external fragmentation), jise remove karne ke liye compaction ki zarurat padti hai.

### 19. Explain Various 'Page Replacement Algorithms' in brief with the help of suitable example of each.
####  What is a Page Replacement Algorithm?
When a page fault occurs (i.e., the required page is not in memory), the operating system needs to bring that page into memory. If memory is full, it must replace an existing page — this is where Page Replacement Algorithms come in.

##### 1. FIFO (First-In-First-Out)
Concept: Replace the page that has been in memory the longest.

##### 2. LRU (Least Recently Used)
Concept: Replace the page that was least recently used.

##### 3. Optimal (OPT)
Concept: Replace the page that won’t be used for the longest time in future.

##### 4. Clock (Second Chance)
Concept: Like FIFO, but gives each page a second chance using a reference bit.

### 20. Explain the various types of directories systems with the help of suitable examples of each.
Operating systems organize files in directories to manage and access them efficiently. There are several types of directory systems:

#### 1. Single-Level Directory:
All files are stored in one single directory. Suitable for small systems with one user.

#### 2. Two-Level Directory:
There is a separate directory for each user. Users cannot access others’ files directly.

#### 3. Tree-Structured Directory:
Allows users to create subdirectories inside directories. It forms a hierarchical (tree) structure.

#### 4. Acyclic Graph Directory:
Files and directories can be shared among users. Implemented using links or shortcuts.

#### 5. General Graph Directory:
Similar to acyclic graph but cycles are allowed. May require garbage collection to manage deleted files.

### 21. How a file can be protected? Discuss various protection mechanism used for protecting files.
#### How a file can be protected?
A file can be protected by controlling how users access it. Protection ensures that only authorized users can read, write, or execute a file. File protection prevents accidental or malicious modifications or deletions.

#### Various Protection Mechanisms:
##### 1. Access Control (Permission-based):
  - Every file has permissions (read, write, execute) for three types of users:
  - Owner (User)
  - Group
  - Others
  - Example in Linux: rwxr--r-- → Owner can read/write/execute, group and others can only read.

##### 2. Password Protection:
Files are locked with passwords. Only users who know the password can access the file. This is a basic level of security and not very scalable.

##### 3. Encryption:
File contents are encoded using encryption algorithms. Only authorized users with the correct decryption key can access the data. Very secure, especially for sensitive information.

##### 4. User Authentication:
Operating system ensures that only authenticated (logged-in) users can access certain files. This is tied with user accounts and access levels.

##### 5. File Attributes (Read-Only, Hidden, System):
Files can be marked as read-only to prevent modifications. Hidden files are not visible to casual users. System files are protected from changes to maintain OS stability.


##### 6. Backup and Versioning:
Files are periodically backed up. Versioning allows rollback to a previous safe state if tampered or corrupted.

##### 7. Audit and Monitoring:
Tracks access and changes to files. Helps detect unauthorized access and take necessary action.

#### Conclusion:
By combining multiple protection mechanisms like permissions, encryption, authentication, and monitoring, file security is ensured against unauthorized access and corruption.
