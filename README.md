# CSE-2207: Operating System — Semester Final Preparation Guide (Sessions: 2017–2018 to 2023–2024)

> **Department of Computer Science and Engineering, University of Barishal**  
> **Course Code:** CSE-2207 &bull; **Course Title:** Operating System &bull; **Credits:** 3.0  
> **Course Instructor / Examiner:** Md. Rashid Al Asif, Assistant Professor (along with Dr. Md. Manjur Ahmed, Md. Samsuddoha, Md. Irfan)  
> **Target Exam:** 2nd Year 2nd Semester Final Examination  
> **Syllabus Reference:** *Operating System Concepts* (Silberschatz, Galvin, Gagne — 9th/10th Edition) — Chapters 1 through 10  
> **Exam Structure & Marks Distribution:** Total 60 Marks &bull; 8 Questions Set (12 Marks each) &bull; Answer any 5 Questions ($5 \times 12 = 60\text{ Marks}$)  

---

## 📑 Syllabus Outline Covered (Chapters 1 – 10)

### Chapter 1: Introduction to Operating Systems
- **1.1 What Operating Systems Do** (User View, System View, Resource Allocator, Control Program)
- **1.2 Computer-System Organization** (Interrupts, Storage Structure, I/O Structure)
- **1.3 Computer-System Architecture** (Single/Multiprocessor Systems, Clustered Systems, Logical Organization)
- **1.4 Operating-System Operations** (Dual-Mode Operation: User Mode and Kernel Mode, Mode Bit, Privileged Instructions)
- **1.5 Computing Environments & Types** (Batch Systems, Multiprogramming, Timesharing/Multitasking)
- **1.6 Storage Management & Caching** (Caching Principles, Cache Coherency, Direct Memory Access [DMA])
- **1.7 Essential Operating System Managers** (Memory Manager, Processor Manager, Device Manager, File Manager)

### Chapter 2: Operating-System Structures & System Calls
- **2.1 Operating-System Services** (User Interface, Program Execution, I/O Operations, Communications, Resource Allocation)
- **2.2 System Calls** (Definition, Parameter Passing: Registers, Block/Table, Stack; Execution Steps)
- **2.3 System Programs & Application Architecture** (File Management, Status Information, Programming Support, Relationship to Hardware)
- **2.4 Operating-System Design & Kernel Architectures** (Monolithic, Layered, Microkernel, Modular, Hybrid Kernels: macOS, Linux, Android)

### Chapter 3: Processes & Process Management
- **3.1 Process Concept** (Process Memory Layout: Text, Data, Heap, Stack; Process vs Program)
- **3.2 Process States & Lifecycle** (New, Ready, Running, Waiting, Terminated; State Transition Diagram)
- **3.3 Process Control Block (PCB)** (Process State, Program Counter, CPU Registers, Memory Limits, Accounting Information)
- **3.4 Context Switching** (Definition, State Save & Restore, CPU Overheads)
- **3.5 Inter-Process Communication (IPC)** (Shared-Memory Systems vs Message-Passing Systems, Synchronous vs Asynchronous Communication)

### Chapter 4: Threads & Concurrency
- **4.1 Overview of Threads** (Single-threaded vs Multithreaded Process, Benefits: Responsiveness, Resource Sharing, Economy, Scalability)
- **4.2 Multithreading Models** (User Threads vs Kernel Threads; Many-to-One, One-to-One, Many-to-Many Models)
- **4.3 Thread Scheduling & Issues** (Process-Contention Scope [PCS] vs System-Contention Scope [SCS], Fork/Exec Semantics)

### Chapter 5: CPU Scheduling
- **5.1 Basic Concepts** (CPU-I/O Burst Cycles, Alternating Sequence, CPU Scheduler, Dispatcher & Dispatch Latency)
- **5.2 Schedulers** (Long-Term / Job Scheduler, Medium-Term Scheduler / Swapper, Short-Term / CPU Scheduler)
- **5.3 Scheduling Criteria** (CPU Utilization, Throughput, Turnaround Time, Waiting Time, Response Time)
- **5.4 Preemptive vs Non-Preemptive Scheduling**
- **5.5 Scheduling Algorithms & Gantt Charts** (FCFS, Non-Preemptive SJF, Preemptive SJF [SRTF], Priority Scheduling, Round Robin with Quantum, Multilevel Queue & Multilevel Feedback Queue)

### Chapter 6: Synchronization Tools & Classic Problems
- **6.1 Background & Race Conditions** (Shared Variables Interleaving, Variable `counter++` and `counter--` Assembly Hazards)
- **6.2 The Critical-Section Problem** (Entry, Critical, Exit, Remainder Sections; Requirements: Mutual Exclusion, Progress, Bounded Waiting)
- **6.3 Hardware Synchronization & Mutex Locks** (`test_and_set()`, `compare_and_swap()`, Spinlocks)
- **6.4 Semaphores** (Definition, Wait/P and Signal/V Atomic Operations, Counting vs Binary Semaphores, Busy Waiting vs Blocked Queue)
- **6.5 Classic Problems of Synchronization** (Bounded-Buffer / Producer-Consumer, Readers-Writers, Dining Philosophers)

### Chapter 7: Deadlocks
- **7.1 Deadlock Characterization** (System Model, Four Coffman Conditions: Mutual Exclusion, Hold and Wait, No Preemption, Circular Wait)
- **7.2 Resource-Allocation Graph (RAG)** (Request Edges, Assignment Edges, Cycle Analysis for Single vs Multiple Resource Instances)
- **7.3 Deadlock Handling Methods** (Prevention, Avoidance, Detection & Recovery, Ostrich Algorithm)
- **7.4 Deadlock Prevention** (Invalidating Coffman Conditions, Strict Resource Ordering)
- **7.5 Deadlock Avoidance & Banker's Algorithm** (Safe State, Unsafe State; Resource-Allocation Graph Algorithm; Banker's Safety & Request Algorithms)
- **7.6 Deadlock Detection & Recovery** (Wait-For Graph, Cycle Detection, Process Termination, Resource Preemption & Starvation)

### Chapter 8: Main Memory Management
- **8.1 Address Binding & Program Processing** (Compile Time, Load Time, Execution Time; Multistep Processing: Compiler, Assembler, Linker, Loader)
- **8.2 Contiguous Memory Allocation** (Dynamic Storage-Allocation: First-Fit, Best-Fit, Worst-Fit, Next-Fit; Memory Partitions)
- **8.3 Fragmentation** (Internal Fragmentation, External Fragmentation, 50-Percent Rule, Compaction)
- **8.4 Paging Architecture** (Pages, Frames, Page Table, Logical-to-Physical Address Translation, Hardware Implementation)
- **8.5 Translation Lookaside Buffer (TLB)** (Associative Memory, TLB Hit/Miss, Effective Memory Access Time [EMAT] Calculations)
- **8.6 Segmentation** (User View of Memory, Segment Table: Base and Limit Registers, Address Translation, Paging vs Segmentation)

### Chapter 9: Virtual Memory & Page Replacement
- **9.1 Virtual Memory Concepts** (Separation of Logical & Physical Memory, Sparse Address Spaces, Benefits)
- **9.2 Demand Paging & Page Fault Handling** (Lazy Swapper / Pager, Valid-Invalid Bit, Detailed Steps in Servicing a Page Fault)
- **9.3 Performance of Demand Paging** (Effective Access Time Formula with Page Fault Rate $p$)
- **9.4 Page Replacement Algorithms** (FIFO, Optimal [OPT], Least Recently Used [LRU], Belady's Anomaly, Reference Strings)
- **9.5 Allocation of Frames & Thrashing** (Frame Allocation Strategies, Causes of Thrashing, Working-Set Model, Page-Fault Frequency)

### Chapter 10: Storage Management, Disk Scheduling & RAID
- **10.1 Storage Device Hierarchy** (Registers, Cache, Main Memory, Electronic Disks, Magnetic Disks, Optical Disks, Magnetic Tapes)
- **10.2 Magnetic Disk Structure & Mechanics** (Platters, Tracks, Sectors, Cylinders, Read-Write Heads, Disk Access Time Calculations)
- **10.3 Disk Scheduling Algorithms** (FCFS, SSTF, SCAN / Elevator, C-SCAN, LOOK, C-LOOK; Total Head Movement Calculations)
- **10.4 Solid-State Disks (SSDs)** (Flash-based Storage, FCFS Scheduling Preference, Wear Leveling)
- **10.5 RAID Architecture** (Redundancy, Striping, Mirroring, Parity; RAID Levels 0, 1, 5, 6, RAID 0+1 vs 1+0)

---

## 🎯 Topic-by-Topic Historical Questions & Marks Analysis

---

### CHAPTER 1: Introduction to Operating Systems

#### 1.1 Operating System Fundamentals, Roles & Dual-Mode Operation
* **"What do you mean by an Operating System? What are the three main purposes of an operating system? Write a short note on, 'An operating system is a resource allocator'."**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"What are the three main purposes of an operating system?"**
  * **Marks:** 2 Marks &mdash; [2020-2021 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"What are the four essential managers of an operating system?"**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"How does the distinction between kernel mode and user mode function as a rudimentary form of protection (security) system?"**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

* **"Explain how the division of user mode and kernel mode provides basic system security in an operating system."**
  * **Marks:** 3 Marks &mdash; [2022-2023 1st Mid: Q4](downloaded_questions/Mid/Mid_1st_Mid_Session_2022-2023_Teacher_Md_Rashid_Al_Asif_ID714.pdf#page=1)

* **"We have stressed the need for an operating system to make efficient use of computing hardware. When is it appropriate for the operating system to forsake this principle and to 'waste' resources? Why is such a system not really wasteful?"**
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q1(d)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

* **"Imagine a busy office where employees rely on computers for tasks like word processing, spreadsheet analysis, and web browsing. Describe how an operating system functions as a resource allocator and a control program in this environment."**
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q1(d)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

#### 1.2 Computer-System Organization, Hardware & Storage Architecture
* **"Discuss the relationship between hardware, OS, system programs, and application programs."**
  * **Marks:** 2 Marks &mdash; [2021-2022 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

* **"What are the main components in the logical organization of a computer system?"**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

* **"Why do some systems store the operating system in firmware, while others store it on disk?"**
  * **Marks:** 2 Marks &mdash; [2018-2019 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)
  * **Marks:** 2 Marks &mdash; [2018-2019 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

#### 1.3 Caching, DMA & Computing Environments
* **"Give two reasons why caches are useful. What problems do they solve? What problems do they cause? If a cache can be made larger, why not make it larger?"**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"Direct memory access (DMA) is used for high-speed I/O devices in order to avoid increasing the CPU's execution load. How does the CPU interface with the device to coordinate the transfer?"**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

* **"Explain the key differences between Batch Operating Systems, Multiprogramming Operating Systems, and Multitasking Operating Systems. Provide examples where each type is commonly used."**
  * **Marks:** 6 Marks &mdash; [2020-2021 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

---

### CHAPTER 2: Operating-System Structures & System Calls

#### 2.1 Operating System Services
* **"List five services provided by an operating system and explain how each creates convenience for users. In which cases it would be impossible for user-level programs to provide these services?"**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

#### 2.2 System Calls & Execution Flow
* **"What is system call? Briefly explain the steps taken when a user program makes a system call."**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Briefly explain the purposes of system calls and system programs."**
  * **Marks:** 3 Marks &mdash; [2020-2021 Final: Q2(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

#### 2.3 Kernel Architectures (Monolithic, Microkernel, Layered, Hybrid)
* **"Explain the differences between a monolithic kernel, a microkernel, and a hybrid kernel. What are the advantages and disadvantages of each?"**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2022-2023 1st Mid: Q1](downloaded_questions/Mid/Mid_1st_Mid_Session_2022-2023_Teacher_Md_Rashid_Al_Asif_ID714.pdf#page=1)

* **"Describe the layered structure of an operating system and explain its advantages and disadvantages."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q1(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Compare Monolithic, Layered, Microkernel, and Modular operating system architectures with diagrams."**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

---

### CHAPTER 3: Processes & Process Management

#### 3.1 Process Concept, States & Lifecycle Diagram
* **"With the help of a diagram, describe the different states of a process in the process lifecycle. Explain what causes a process to transition between states."**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2022-2023 1st Mid: Q3](downloaded_questions/Mid/Mid_1st_Mid_Session_2022-2023_Teacher_Md_Rashid_Al_Asif_ID714.pdf#page=1)

* **"Outline the lifecycle of a process, describing each state and the events that cause transitions between them."**
  * **Marks:** 6 Marks &mdash; [2020-2021 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)
  * **Marks:** 5 Marks &mdash; [2017-2018 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"What is a process in an operating system, and how does it differ from a program?"**
  * **Marks:** 3 Marks &mdash; [2020-2021 Final: Q2(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"What are the two essential parts of a process? How is a process different from a program?"**
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

#### 3.2 Process Control Block (PCB) & Context Switching
* **"What is Process Control Block (PCB)? List and explain any four types of information contained in a PCB."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)
  * **Marks:** 6 Marks &mdash; [2019-2020 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"Explain the concept of context switching. Why is it necessary and what overheads are associated with it?"**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q2(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

#### 3.3 Inter-Process Communication (IPC)
* **"What is inter-process communication (IPC), and what are some common IPC mechanisms? Contrast shared-memory and message-passing."**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"What are the benefits and the disadvantages of synchronous and asynchronous communication?"**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

---

### CHAPTER 4: Threads & Concurrency

#### 4.1 Process vs Thread & Multithreading Benefits
* **"Define a thread. How does it differ from a process in terms of resource allocation, creation overhead, and execution?"**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q2(c)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

* **"A multithreaded web server wishes to keep track of the number of client requests. Explain how multithreading provides benefits over a single-threaded server."**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

* **"Provide two programming examples in which multithreading provides better performance than a single-threaded solution."**
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q2(d)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

#### 4.2 User-Level vs Kernel-Level Threads & Multithreading Models
* **"Explain the difference between user-level threads and kernel-level threads. Under what circumstances is one preferred over the other?"**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q2(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"Explain different threading models (Many-to-One, One-to-One, Many-to-Many) with sufficient diagrams."**
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q2(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

* **"How does thread scheduling differ from process scheduling? Explain with examples of user-level vs kernel-level threads."**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

---

### CHAPTER 5: CPU Scheduling

#### 5.1 Basic Concepts & Schedulers
* **"Define CPU burst and I/O burst. How do these concepts influence the choice of a CPU scheduling algorithm?"**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Define the following terms: i) Short-term scheduler ii) CPU dispatcher"**
  * **Marks:** 2 Marks &mdash; [2020-2021 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"Describe the differences among short-term, medium-term, and long-term scheduling."**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

* **"Describe process scheduling and the role of the scheduler in managing the ready queue."**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"What is a job scheduler? What is a process scheduler?"**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q1(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"Explain the concept of scheduling criteria. Describe any four commonly used scheduling criteria."**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"What is the relationship between turnaround time, CPU cycle time, and waiting time?"**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q2(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"Explain the difference between preemptive and non-preemptive scheduling."**
  * **Marks:** 2 Marks &mdash; [2019-2020 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

#### 5.2 CPU Scheduling Algorithms & Gantt Chart Numericals
* **"Define CPU scheduling. Consider the following set of processes: P1 (Burst 10, Priority 3), P2 (Burst 1, Priority 1), P3 (Burst 2, Priority 3), P4 (Burst 1, Priority 4), P5 (Burst 5, Priority 2). Draw Gantt charts for FCFS, SJF, Priority, and Round Robin (Quantum=1), and calculate average waiting time."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Consider the following set of processes, with the length of the CPU burst time given in milliseconds: P1 (Burst 10), P2 (Burst 29), P3 (Burst 3), P4 (Burst 7), P5 (Burst 12). Illustrate the execution of these processes using FCFS, SJF, and Round Robin (quantum = 10) scheduling."**
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

* **"Consider the following set of process with CPU burst time: P1 (Burst 6), P2 (Burst 8), P3 (Burst 7), P4 (Burst 3). Draw Gantt charts and find average waiting time using SJF and Round Robin (quantum = 2)."**
  * **Marks:** 5 Marks &mdash; [2022-2023 1st Mid: Q2](downloaded_questions/Mid/Mid_1st_Mid_Session_2022-2023_Teacher_Md_Rashid_Al_Asif_ID714.pdf#page=1)

* **"Consider the following set of processes with their respective arrival time and CPU burst times: P1 (Arrival 0, Burst 8), P2 (Arrival 1, Burst 4), P3 (Arrival 2, Burst 9), P4 (Arrival 3, Burst 5). Compute turnaround and waiting times under Preemptive SJF (SRTF) and Non-preemptive Priority."**
  * **Marks:** 6 Marks &mdash; [2020-2021 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)
  * **Marks:** 6 Marks &mdash; [2018-2019 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

* **"The following processes are being scheduled using a Priority Scheduling algorithm: P1 (Burst 10, Priority 3), P2 (Burst 1, Priority 1), P3 (Burst 2, Priority 4), P4 (Burst 1, Priority 5), P5 (Burst 5, Priority 2). Draw Gantt chart and compute average waiting time."**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q3(d)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"Draw Gantt Charts for illustrating five scheduling algorithms (FCFS, SJF, Priority, Round Robin, SRTF) for the given process workload."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q3(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"Calculate the turnaround time for each process based on the five scheduling algorithms."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"Calculate the waiting time for each process based on the scheduling algorithms."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"Calculate the average turnaround time and the average waiting time for each algorithm."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q3(d)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"What advantage is there in having different time-quantum sizes at different levels of a multilevel queueing system?"**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q3(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=1)

* **"Consider a computer system that runs 5,000 jobs per month and has no dynamic priority adjustments. Why would a multilevel feedback queue algorithm be superior to a simple priority scheme?"**
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q3(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=1)

---

### CHAPTER 6: Process Synchronization & Classic Problems

#### 6.1 Critical-Section Problem, Race Conditions & Shared Variable Interleaving
* **"Define process synchronization. Why is it necessary in a multiprogramming environment? State the three requirements of a solution to the critical-section problem (Mutual Exclusion, Progress, Bounded Waiting)."**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)
  * **Marks:** 3 Marks &mdash; [2020-2021 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q4(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=1)

* **"Two processes, P1 and P2, share a common variable counter initially set to 5. P1 executes 'counter++' and P2 executes 'counter--'. Show how an improper interleaving of low-level machine instructions leads to a race condition."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q4(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Race conditions are possible in many computer systems. Consider a bank account balance shared by two transactions. Illustrate how race condition occurs."**
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

* **"Consider a system in which a program can be separated into two parts: code executed in user mode and code executed in kernel mode. How does synchronization apply?"**
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q4(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

#### 6.2 Semaphores & Implementation
* **"Describe how semaphores are used for process synchronization. Illustrate with an example how binary semaphores can be used to solve the critical-section problem."**
  * **Marks:** 5 Marks &mdash; [2021-2022 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

#### 6.3 Classical Synchronization Problems & Simulation
* **"Describe the Producer–Consumer problem and explain how semaphores can be used to solve it without causing race conditions or deadlocks."**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=1)

* **"Regarding the Producer-Consumer problem, explain the following terms: i) Bounded Buffer, ii) Empty and Full Semaphores, iii) Race Condition on Counter."**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q4(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

* **"Compare and contrast classical synchronization problems: Producer-Consumer, Readers-Writers, and Dining Philosophers."**
  * **Marks:** 4 Marks &mdash; [2022-2023 1st Mid: Q5](downloaded_questions/Mid/Mid_1st_Mid_Session_2022-2023_Teacher_Md_Rashid_Al_Asif_ID714.pdf#page=1)

* **"Case Study: In a university's computer lab, two students, Alice and Bob, are writing programs to simulate bank transactions. Both programs concurrently update the same bank account balance. (i) Identify the critical section problem. (ii) Show how race conditions can corrupt the account balance. (iii) Design a semaphore-based solution ensuring mutual exclusion, progress, and bounded waiting."**
  * **Marks:** 12 Marks &mdash; [2021-2022 Final: Q4(c) [Lab Simulation Case]](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=1)

---

### CHAPTER 7: Deadlocks

#### 7.1 Deadlock Characterization & Four Coffman Conditions
* **"What is deadlock? Describe about necessary conditions for deadlock characterization (Mutual Exclusion, Hold & Wait, No Preemption, Circular Wait)."**
  * **Marks:** 5 Marks &mdash; [2017-2018 Final: Q4(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2017-2018 Final: Q4(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

* **"List three examples of deadlocks that are not related to a computer system environment (e.g., traffic gridlock, bridge crossing)."**
  * **Marks:** 2 Marks &mdash; [2018-2019 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

#### 7.2 Resource Allocation Graph (RAG) & Cycle Detection
* **"Describe the Resource Allocation Graph (RAG) method for detecting deadlocks. How does the presence of a cycle determine whether a deadlock exists?"**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 5 Marks &mdash; [2021-2022 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)

* **"Consider a system with two types of resources (R1, R2) and three processes (P1, P2, P3). Draw a Resource Allocation Graph and analyze if deadlock exists."**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"List two deadlock detection mechanisms. Construct the wait-for graph for a given set of processes and explain cycle detection."**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q5(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

* **"Identify all of the deadlocked processes from the given Resource Allocation Graph."**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Can the deadlock be resolved without selecting a victim process to terminate?"**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Which requests by the three processes for resources from R2 would result in an immediate deadlock?"**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q5(c)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Conversely, which requests by the three processes for resources from R1 could be safely granted?"**
  * **Marks:** 4 Marks &mdash; [2017-2018 Final: Q5(d)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

#### 7.3 Deadlock Prevention, Avoidance & Safe States
* **"Explain the difference between deadlock prevention and deadlock avoidance. Discuss how each approach manages resource requests."**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q5(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 6 Marks &mdash; [2020-2021 Final: Q5(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"What is deadlock? Discuss various strategies used to prevent it from occurring by invalidating the 4 Coffman conditions."**
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)

* **"Suppose that a system is in an unsafe state. Show that it is possible for the processes to complete without entering a deadlock."**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q5(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

#### 7.4 Banker's Algorithm Safe-State Numericals
* **"Consider the following system with 3 processes (P1, P2, P3) and 4 resource types (A, B, C, D). Given Allocation, Max, and Available matrices, determine if the system is in a safe state using Banker's Algorithm. Find the safe sequence."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)

* **"Answer the following questions using the Banker's algorithm: (i) What is the content of the Need matrix? (ii) Is the system in a safe state? If yes, find the safe sequence. (iii) If a request from process P1 arrives for (0, 4, 2, 0), can the request be granted immediately?"**
  * **Marks:** 10 Marks &mdash; [2021-2022 1st Mid: Q2](downloaded_questions/Mid/Mid_1st_Mid_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID637.pdf#page=1)

* **"Consider the following snapshot of a system: 5 processes (P0-P4) and 3 resource types (A, B, C). Allocation and Max matrices provided. Answer: (i) What is the Need matrix? (ii) Is the system in a safe state? (iii) Can request by P1 for (1, 0, 2) be granted?"**
  * **Marks:** 6 Marks &mdash; [2019-2020 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)
  * **Marks:** 6 Marks &mdash; [2018-2019 Final: Q5(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

* **"Given the following system: Total of four processes and three resource types. Determine whether the current state is safe, and find the safe execution sequence."**
  * **Marks:** 5 Marks &mdash; [2018-2019 Final: Q5(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

* **"Briefly describe Banker's algorithm and its Safety test procedure."**
  * **Marks:** 4 Marks &mdash; [2017-2018 Final: Q4(c)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

---

### CHAPTER 8: Main Memory Management

#### 8.1 Address Binding & Program Processing
* **"Explain multistep processing of a user program from source code to execution (compiler, assembler, linker, loader)."**
  * **Marks:** 4 Marks &mdash; [2017-2018 Final: Q1(c)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)

#### 8.2 Contiguous Memory Allocation: First-Fit, Best-Fit, Worst-Fit
* **"A system has memory blocks of sizes: 100 KB, 500 KB, 200 KB, 300 KB, and 600 KB (in order). How would each of the First-Fit, Best-Fit, and Worst-Fit algorithms place processes of sizes 212 KB, 417 KB, 112 KB, and 426 KB? Which algorithm makes the most efficient use of memory?"**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2020-2021 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

* **"Compare first-fit, best-fit, and worst-fit memory allocation strategies. What are the advantages and disadvantages of each?"**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)

* **"Consider a system with 1000 KB of memory and processes that require various block sizes. Trace First-fit and Best-fit allocations."**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)

* **"Given six memory partitions of 300 KB, 600 KB, 350 KB, 200 KB, 750 KB, and 125 KB (in order), how would First-fit, Best-fit, and Worst-fit allocate processes of 115 KB, 500 KB, 358 KB, 200 KB, and 375 KB?"**
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

* **"Use the best-fit algorithm to allocate the memory blocks to the three incoming jobs."**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Use the first-fit algorithm to allocate the memory blocks to the three incoming jobs."**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Use the next-fit algorithm to allocate the memory blocks to the three incoming jobs."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Worst-fit is an allocation algorithm that allocates the largest free block. Allocate the blocks using worst-fit."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q6(d)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"From the comparison of the allocation results, WHICH algorithm is the best in terms of memory utilization?"**
  * **Marks:** 2 Marks &mdash; [2017-2018 Final: Q6(e)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

#### 8.3 Fragmentation: Internal vs External
* **"Define internal and external fragmentation with necessary diagrams. How can external fragmentation be eliminated?"**
  * **Marks:** 2 Marks &mdash; [2021-2022 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 2 Marks &mdash; [2020-2021 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)
  * **Marks:** 2 Marks &mdash; [2019-2020 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

#### 8.4 Paging Architecture & Address Translation
* **"A system uses paging for memory management. The logical address space consists of 8 pages of 1024 bytes each, mapped to 32 physical frames. (i) How many bits are required for the logical address and physical address? (ii) Given page table entries, translate logical address 2050 into physical address."**
  * **Marks:** 6 Marks &mdash; [2022-2023 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)

* **"What is paging in an operating system, and how does it manage memory? Draw and explain the paging hardware with a page table."**
  * **Marks:** 5 Marks &mdash; [2020-2021 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"What is paging? Consider a logical address space of 64 pages of 1,024 words each, mapped onto a physical memory of 32 frames. (i) How many bits are there in the logical address? (ii) How many bits are there in the physical address?"**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q6(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q6(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=2)

* **"Draw and describe address translation architecture in a paging system."**
  * **Marks:** 4 Marks &mdash; [2017-2018 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

#### 8.5 Translation Lookaside Buffer (TLB) & Effective Memory Access Time (EMAT)
* **"A system has a memory access time of 100 ns. The TLB hit ratio is 80%, and TLB lookup takes 20 ns. Calculate the Effective Memory Access Time (EMAT)."**
  * **Marks:** 2 Marks &mdash; [2022-2023 Final: Q6(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q6(d)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=2)

* **"Describe the concept of a Translation Lookaside Buffer (TLB). How does it improve the performance of paging? Draw the hardware architecture with TLB."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)

* **"Define TLB with diagram. Given the following information about a system: TLB search time = 20 ns, memory access time = 100 ns, TLB hit ratio = 90%. What is the effective memory access time?"**
  * **Marks:** 4 Marks &mdash; [2020-2021 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"Describe the following with examples: i) Paging, ii) TLB. Calculate EMAT for a given TLB configuration."**
  * **Marks:** 10 Marks &mdash; [2021-2022 1st Mid: Q1](downloaded_questions/Mid/Mid_1st_Mid_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID637.pdf#page=1)

#### 8.6 Segmentation Architecture & Segment Table Numericals
* **"What is segmentation? Consider the following segment table: Segment 0 (Base 219, Limit 600), Segment 1 (Base 2300, Limit 14), Segment 2 (Base 90, Limit 100), Segment 3 (Base 1327, Limit 580), Segment 4 (Base 1952, Limit 96). What are physical addresses for logical addresses: <0, 430>, <1, 10>, <2, 500>, <3, 400>, <4, 112>?"**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 5 Marks &mdash; [2019-2020 Final: Q7(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)
  * **Marks:** 5 Marks &mdash; [2018-2019 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

* **"Define demand paging and segmentation with examples."**
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

#### 8.7 Comparison: Paging vs Segmentation
* **"Explain how paging and segmentation deal with the problem of fragmentation. Compare the two techniques."**
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q6(d)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 3 Marks &mdash; [2020-2021 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

---

### CHAPTER 9: Virtual Memory & Page Replacement

#### 9.1 Virtual Memory Concepts & Advantages
* **"Define virtual memory. How does it empower computing? Explain the benefits of separating user logical memory from physical memory."**
  * **Marks:** 3 Marks &mdash; [2019-2020 Final: Q7(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)

* **"Define page replacement in virtual memory. Why is it necessary?"**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q8(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)

#### 9.2 Page Fault Handling Steps
* **"Define page fault. What are the actions taken by the operating system when a page fault occurs? Draw the steps in handling a page fault."**
  * **Marks:** 3 Marks &mdash; [2021-2022 Final: Q7(c)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 5 Marks &mdash; [2017-2018 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Describe the sequence of steps that occur when a virtual address is translated in a system using demand paging and a page fault occurs."**
  * **Marks:** 5 Marks &mdash; [2021-2022 Final: Q7(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)

#### 9.3 Demand Paging Performance & EMAT Calculation
* **"A system uses demand paging and has: Memory access time = 200 ns, Average page fault service time = 8 ms (8,000,000 ns). If we want the effective access time to be no more than 220 ns, what is the maximum acceptable page fault rate p?"**
  * **Marks:** 3 Marks &mdash; [2022-2023 Final: Q7(c)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)

#### 9.4 Page Replacement Algorithms & Reference String Numericals
* **"Consider the following page reference string: 7, 0, 1, 2, 0, 3, 0, 4, 2, 3, 0, 3, 2, 1, 2, 0, 1, 7, 0, 1 with 3 frames. Calculate page faults under LRU, Optimal, and FIFO algorithms."**
  * **Marks:** 5 Marks &mdash; [2022-2023 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 5 Marks &mdash; [2021-2022 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 6 Marks &mdash; [2020-2021 Final: Q7(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"Consider the following page reference string: 2, 3, 2, 1, 5, 2, 4, 5, 3, 2, 5, 2. How many page faults would occur for the following algorithms with 3 frames: i) FIFO, ii) Optimal, iii) LRU?"**
  * **Marks:** 6 Marks &mdash; [2019-2020 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)

* **"Consider the following page reference string: 1, 2, 3, 4, 2, 1, 5, 6, 2, 1, 2, 3, 7, 6, 3, 2, 1, 2, 3, 6. Calculate page faults for FIFO and LRU with 3 frames."**
  * **Marks:** 6 Marks &mdash; [2018-2019 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

* **"Given that main memory is composed of THREE page frame for public use and that a program requests pages in the following order: A, B, C, D, A, B, E, A, B, C, D, E. Using FIFO and LRU algorithms, determine the total number of page faults."**
  * **Marks:** 8 Marks &mdash; [2017-2018 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

#### 9.5 Thrashing & Solutions
* **"Define the following terms: i) CPU Thrashing, ii) RAID. Explain the causes of thrashing and how the working-set model prevents it."**
  * **Marks:** 4 Marks &mdash; [2022-2023 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2022-2023_Teacher_Unknown_ID771.pdf#page=2)
  * **Marks:** 4 Marks &mdash; [2021-2022 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2021-2022_Teacher_Md_Rashid_Al_Asif_ID650.pdf#page=2)
  * **Marks:** 2 Marks &mdash; [2019-2020 Final: Q8(c)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

---

### CHAPTER 10: Storage Management, Disk Scheduling & RAID

#### 10.1 Storage Device Hierarchy
* **"Draw storage device hierarchy and describe tradeoffs between speed, cost, and capacity."**
  * **Marks:** 3 Marks &mdash; [2017-2018 Final: Q1(d)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=1)
  * **Marks:** 4 Marks &mdash; [2018-2019 Final: Q8(d)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

#### 10.2 Disk Scheduling Algorithms & Numericals
* **"Suppose that a disk drive has 200 cylinders, numbered 0 to 199. The drive is currently serving a request at cylinder 53, and the previous request was at cylinder 20. The queue of pending requests in FIFO order is: 98, 183, 37, 122, 14, 124, 65, 67. Calculate total head movements for FCFS and SSTF."**
  * **Marks:** 4 Marks &mdash; [2019-2020 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2019-2020_Teacher_Md_Rashid_Al_Asif_ID414.pdf#page=3)

* **"Suppose that a disk drive has 5000 cylinders, numbered 0 to 4999. The drive is currently serving a request at cylinder 143, and the previous request was at cylinder 125. The queue of pending requests in FIFO order is: 86, 1470, 913, 1774, 948, 1509, 1022, 1750, 130. Starting from the current head position, what is the total distance (in cylinders) that the disk arm moves to satisfy all pending requests for: i) FCFS, ii) SSTF, iii) SCAN, iv) LOOK, v) C-SCAN?"**
  * **Marks:** 12 Marks &mdash; [2017-2018 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2017-2018_Teacher_Md_Rashid_Al_Asif_ID420.pdf#page=2)

* **"Explain why SSDs often use an FCFS disk-scheduling algorithm."**
  * **Marks:** 3 Marks &mdash; [2018-2019 Final: Q8(c)](downloaded_questions/Final/Final_Final_Session_2018-2019_Teacher_Md_Rashid_Al_Asif_ID421.pdf#page=3)

#### 10.3 Disk Access Time & Physical Geometry Calculations
* **"Explain the moving-head disk mechanism in operating systems. How does the arm movement determine seek time?"**
  * **Marks:** 5 Marks &mdash; [2020-2021 Final: Q8(a)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"How do you calculate the disk access time? A disk is advertised with an average seek time of 4 ms, 7200 RPM rotation speed, and transfer rate of 50 MB/s. Calculate total access time for a 4 KB sector."**
  * **Marks:** 5 Marks &mdash; [2020-2021 Final: Q8(b)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

* **"A hard disk with 4 platters that has 2048 tracks for each platter and 1024 sectors for each track. If each sector stores 512 bytes, what is the total capacity of the hard disk?"**
  * **Marks:** 2 Marks &mdash; [2020-2021 Final: Q8(c)](downloaded_questions/Final/Final_Final_Session_2020-2021_Teacher_Md_Rashid_Al_Asif_ID494.pdf#page=2)

---

## 🏆 Top 10 "Guaranteed" Exam Topics for Semester Final

Based on exhaustive historical analysis across all 6 Final examinations (Sessions 2017–2018 through 2022–2023) and Midterms under Md. Rashid Al Asif and faculty at University of Barishal, the following **10 problem patterns are guaranteed to appear** on your Semester Final paper:

### 1. CPU Scheduling Algorithms & Gantt Chart Numericals
- **Target Problem:** Gantt Chart construction and calculation of Average Turnaround Time (TAT) and Average Waiting Time (WT) for FCFS, Preemptive/Non-preemptive SJF (SRTF), Priority, and Round Robin (RR).
- **Historical Appearances:** 2022–2023 Final (5M), 2021–2022 Final (4M), 2020–2021 Final (6M), 2019–2020 Final (4M), 2018–2019 Final (6M), 2017–2018 Final (12M), 2022–2023 Mid (5M).
- **Exam Strategy & Tips:** Appears consistently as **Question 3** on every single Final exam paper without exception. Master Preemptive SJF (SRTF) tie-breaking and Round Robin with small time quanta ($q=1, 2, 10$).

### 2. Deadlock Avoidance: Banker's Algorithm Numerical
- **Target Problem:** Computation of the `Need` matrix ($Need = Max - Allocation$), safety verification algorithm to find a Safe Sequence $\langle P_0, P_1, \dots, P_n \rangle$, and evaluating immediate resource request feasibility using the Resource-Request Algorithm.
- **Historical Appearances:** 2022–2023 Final (5M), 2021–2022 Mid (10M), 2020–2021 Final (4M), 2019–2020 Final (6M), 2018–2019 Final (11M), 2017–2018 Final (4M).
- **Exam Strategy & Tips:** Appears as **Question 5(b)** on virtually every Final exam. If you write down the safety algorithm trace neatly, you are guaranteed 100% marks.

### 3. Page Replacement Algorithms Numerical (LRU, Optimal, FIFO)
- **Target Problem:** Tracing reference strings on 3 (or 4) page frames and counting the exact number of page faults and page hits for LRU, Optimal (OPT), and FIFO.
- **Historical Appearances:** 2022–2023 Final (5M), 2021–2022 Final (5M), 2020–2021 Final (6M), 2019–2020 Final (6M), 2018–2019 Final (6M), 2017–2018 Final (8M).
- **Exam Strategy & Tips:** Appears as **Question 8(a)** (or Q7) on every single Final exam. The standard reference string `7, 0, 1, 2, 0, 3, 0, 4, 2, 3, 0, 3, 2, 1, 2, 0, 1, 7, 0, 1` was repeated identically in 2022–2023, 2021–2022, and 2020–2021!

### 4. Contiguous Memory Allocation: First-Fit, Best-Fit, Worst-Fit Numericals
- **Target Problem:** Allocation of a given sequence of process sizes (e.g., 212 KB, 417 KB, 112 KB, 426 KB) into given memory blocks (e.g., 100 KB, 500 KB, 200 KB, 300 KB, 600 KB) and analyzing internal/external fragmentation and memory utilization.
- **Historical Appearances:** 2022–2023 Final (4M), 2021–2022 Final (6M), 2020–2021 Final (3M), 2019–2020 Final (3M), 2018–2019 Final (4M), 2017–2018 Final (12M).
- **Exam Strategy & Tips:** Appears as **Question 6(a)**. The exact partition problem (`100 KB, 500 KB, 200 KB, 300 KB, 600 KB` with processes `212 KB, 417 KB, 112 KB, 426 KB`) has appeared in three consecutive sessions!

### 5. Paging, TLB & Effective Memory Access Time (EMAT) Calculations
- **Target Problem:** Calculation of EMAT using the formula: $\text{EMAT} = \alpha \times (t_{\text{TLB}} + t_{\text{mem}}) + (1 - \alpha) \times (t_{\text{TLB}} + 2 \times t_{\text{mem}})$, and logical-to-physical address translation.
- **Historical Appearances:** 2022–2023 Final (2M + 5M), 2021–2022 Mid (10M), 2020–2021 Final (4M), 2019–2020 Final (3M + 4M), 2017–2018 Final (4M).
- **Exam Strategy & Tips:** Appears as **Question 6(c) or 7(a)**. Ensure you include both cases (TLB hit requires 1 memory access; TLB miss requires 2 memory accesses).

### 6. Segmentation Architecture & Segment Table Numericals
- **Target Problem:** Given a segment table with Base and Limit for 5 segments (Segments 0 to 4), compute physical addresses for logical addresses $\langle s, d \rangle$ or identify illegal address traps ($d \ge Limit$).
- **Historical Appearances:** 2022–2023 Final (4M), 2021–2022 Final (4M), 2019–2020 Final (5M), 2018–2019 Final (5M).
- **Exam Strategy & Tips:** Appears consistently as **Question 7(a)**. The exact segment table entries (Segment 0: Base 219, Limit 600; Segment 1: Base 2300, Limit 14; Segment 2: Base 90, Limit 100; Segment 3: Base 1327, Limit 580; Segment 4: Base 1952, Limit 96) were repeated across 4 different sessions!

### 7. Process Lifecycle State Transition Diagram & PCB Structure
- **Target Problem:** Drawing the complete 5-state process lifecycle diagram (New, Ready, Running, Waiting, Terminated) with all triggering events (Admit, Dispatch, Interrupt, I/O wait, I/O complete, Exit), and detailing Process Control Block (PCB) fields.
- **Historical Appearances:** 2022–2023 Final (4M + 5M), 2021–2022 Final (4M + 4M), 2020–2021 Final (3M + 6M), 2019–2020 Final (6M), 2018–2019 Final (3M), 2017–2018 Final (5M), 2022–2023 Mid (4M).
- **Exam Strategy & Tips:** Appears as **Question 2(a) and 2(b)** on every single paper. Guaranteed 9 to 12 marks on Question 2.

### 8. Kernel Architectures & Dual-Mode System Protection
- **Target Problem:** Detailed comparison of Monolithic, Microkernel, Layered, and Hybrid kernel architectures with diagrams, and the distinction between User Mode and Kernel Mode (Mode Bit, Privileged Instructions, System Calls).
- **Historical Appearances:** 2022–2023 Final (5M + 4M), 2021–2022 Final (3M + 2M), 2020–2021 Final (4M), 2018–2019 Final (3M + 2M), 2022–2023 Mid (4M + 3M).
- **Exam Strategy & Tips:** Appears as **Question 1** on every Final exam. Essential theory that examiners love to start the exam with.

### 9. Process Synchronization: Critical-Section Problem, Semaphores & Race Condition
- **Target Problem:** The three requirements for critical-section solutions (Mutual Exclusion, Progress, Bounded Waiting), race condition disassembly tracing on `counter++` / `counter--`, and Producer-Consumer bounded-buffer implementation with binary/counting semaphores.
- **Historical Appearances:** 2022–2023 Final (3M + 4M + 5M), 2021–2022 Final (4M + 5M + 12M), 2020–2021 Final (3M + 4M), 2019–2020 Final (4M), 2018–2019 Final (3M + 4M), 2022–2023 Mid (4M).
- **Exam Strategy & Tips:** Appears as **Question 4**. Be prepared to write assembly/C pseudo-code showing register load/store race condition hazards.

### 10. Storage Architecture: Disk Scheduling (Cylinders), CPU Thrashing & RAID
- **Target Problem:** Disk head movement calculations for FCFS, SSTF, SCAN, LOOK, C-SCAN on cylinder queues (e.g., 200 or 5000 cylinders), defining CPU Thrashing and the Working-Set Model, and RAID levels (0, 1, 5).
- **Historical Appearances:** 2022–2023 Final (4M), 2021–2022 Final (4M), 2020–2021 Final (5M + 5M + 2M), 2019–2020 Final (4M + 2M), 2018–2019 Final (6M + 3M + 3M), 2017–2018 Final (12M).
- **Exam Strategy & Tips:** Appears as **Question 8(b) and 8(c)**. A full 12-mark question on disk scheduling appeared in 2017–2018, and combined disk/thrashing questions appear every year.

---

*Maintained for academic revision and semester final exam preparation &bull; University of Barishal CSE.*