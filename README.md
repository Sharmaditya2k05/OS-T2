# Operating Systems (24B11CS312) — Syllabus T2: Week-wise Notes

> **How these notes are built:** every topic and its order come only from the weekly syllabus and the lecture PPTs (Week 5, Week 6_1 / 6_2 / 6_3, Week 7, Week 8). Nothing outside the PPTs has been added. Where a PPT slide is only a figure, the notes describe what the figure shows. Simple "how it works" explanations are added only to make a PPT point easy to understand.

## Weekly syllabus followed

| Week | Dates | Topics | Lectures |
| --- | --- | --- | --- |
| **Week 5** | 25-Aug to 29-Aug | Threads: Processes vs. Threads, User vs. Kernel Threads, Multithreading Models, Threading Issues, Pthreads, Linux Threads, Windows XP Threads | 3 |
| **Week 6** | 09-Sep to 16-Sep | Inter Process Communication: Background, The Critical-Section Problem, Peterson's Solution, Synchronization Hardware, Semaphores, Classic Problems of Synchronization, Monitors, Synchronization Examples, Atomic Transactions | 4 |
| **Week 7** | 17-Sep to 24-Sep | Deadlocks: Deadlock Characterization, Methods for Handling Deadlocks, Deadlock Prevention, Deadlock Avoidance, Deadlock Detection, Recovery from Deadlock | 3 |
| **Week 8** | 25-Sep to 02-Oct | Memory Management: Background, Swapping, Contiguous Memory Allocation, Paging, Structure of Page Table, Types of Paging | 4 |

---

## Contents (full list of topics and subtopics)

### Week 5 — Threads
- **5.1 Processes vs. Threads** — 5.1.1 The 4-CPU scenario · 5.1.2 Method 1: four processes · 5.1.3 Method 2: four threads · 5.1.4 Process vs thread (comparison) · 5.1.5 What is a thread · 5.1.6 Single-threaded and multithreaded processes · 5.1.7 Merits of using threads · 5.1.8 Thread scheduling · 5.1.9 Threads: pros and cons
- **5.2 User vs. Kernel Threads** — 5.2.1 Types of threads · 5.2.2 Thread management · 5.2.3 ULT states and process states · 5.2.4 Merits and demerits of ULT (Jacketing) · 5.2.5 Merits and demerits of KLT · 5.2.6 ULT vs KLT table
- **5.3 Multithreading Models** — 5.3.1 Many-to-One · 5.3.2 One-to-One · 5.3.3 Many-to-Many · 5.3.4 Comparison
- **5.4 Threading Issues** — 5.4.1 fork(), exec(), exit() · 5.4.2 Signal handling · 5.4.3 Thread pools · 5.4.4 Thread safety · 5.4.5 How to ensure thread safety · 5.4.6 Thread-specific data
- **5.5 Pthreads** — 5.5.1 Thread libraries · 5.5.2 POSIX Pthreads · 5.5.3 The pthread library calls · 5.5.4 Example program · 5.5.5 Terminating a thread · 5.5.6 Thread cancellation
- **5.6 Linux Threads**
- **5.7 Windows XP Threads**

### Week 6 — Inter Process Communication
- **6.1 Background** — 6.1.1 Why synchronization is needed · 6.1.2 Producer–consumer · 6.1.3 Race condition
- **6.2 The Critical-Section Problem** — 6.2.1 Definition · 6.2.2 General structure · 6.2.3 A simple lock picture and the `turn` algorithm · 6.2.4 Three requirements · 6.2.5 Critical-section handling in the OS
- **6.3 Peterson's Solution**
- **6.4 Synchronization Hardware** — 6.4.1 Locks · 6.4.2 test_and_set · 6.4.3 compare_and_swap · 6.4.4 Bounded-waiting mutual exclusion with test_and_set
- **6.5 Semaphores** — 6.5.1 Definition · 6.5.2 Usage · 6.5.3 Implementation and busy waiting · 6.5.4 Implementation with no busy waiting · 6.5.5 Deadlock, starvation, priority inversion
- **6.6 Classic Problems of Synchronization** — 6.6.1 Bounded-buffer · 6.6.2 Readers–writers · 6.6.3 Dining philosophers
- **6.7 Monitors** — 6.7.1 Problems with semaphores · 6.7.2 Monitor · 6.7.3 Condition variables · 6.7.4 Condition-variable choices · 6.7.5 Dining philosophers using a monitor · 6.7.6 Monitor implementation using semaphores · 6.7.7 Resuming processes within a monitor · 6.7.8 Single-resource allocation
- **6.8 Synchronization Examples**
- **6.9 Atomic Transactions**

### Week 7 — Deadlocks
- **7.1 Resources and the Deadlock Problem** — 7.1.1 Resources · 7.1.2 The deadlock problem · 7.1.3 When do deadlocks happen · 7.1.4 Formal definition · 7.1.5 Deadlock with semaphores
- **7.2 Deadlock Characterization** — 7.2.1 Four conditions · 7.2.2 Resource-allocation graph · 7.2.3 Basic facts
- **7.3 Methods for Handling Deadlocks**
- **7.4 Deadlock Prevention**
- **7.5 Deadlock Avoidance** — 7.5.1 Safe state · 7.5.2 Avoidance algorithms · 7.5.3 Modified resource-allocation graph · 7.5.4 Banker's algorithm · 7.5.5 Banker's example · 7.5.6 Safe and unsafe state examples
- **7.6 Deadlock Detection** — 7.6.1 Single instance (wait-for graph) · 7.6.2 Several instances · 7.6.3 Example · 7.6.4 Detection-algorithm usage · 7.6.5 Question
- **7.7 Recovery from Deadlock** — 7.7.1 Process termination · 7.7.2 Resource preemption
- **7.8 Advantages and Disadvantages of the Approaches**

### Week 8 — Memory Management
- **8.1 Background** — 8.1.1 Basics · 8.1.2 Base and limit registers · 8.1.3 Address binding · 8.1.4 Logical, relative, physical addresses · 8.1.5 MMU and dynamic relocation · 8.1.6 Dynamic loading · 8.1.7 Dynamic linking
- **8.2 Swapping**
- **8.3 Contiguous Memory Allocation** — 8.3.1 Fixed partitioning · 8.3.2 Dynamic partitioning · 8.3.3 Placement algorithms · 8.3.4 Buddy system
- **8.4 Paging** — 8.4.1 Concept · 8.4.2 Internal fragmentation · 8.4.3 Address translation scheme · 8.4.4 Paging hardware and model · 8.4.5 Paging example · 8.4.6 Free frames
- **8.5 Structure of Page Table** — 8.5.1 Page table · 8.5.2 Implementation (PTBR, PTLR, TLB) · 8.5.3 Effective memory access time · 8.5.4 Valid/invalid bit · 8.5.5 Shared pages
- **8.6 Types of Paging** — 8.6.1 Hierarchical page tables · 8.6.2 Hashed page tables · 8.6.3 Inverted page table

---
---

# WEEK 5 — THREADS

## 5.1 Processes vs. Threads

### 5.1.1 The 4-CPU scenario

- The system has **4 CPUs**.
- A program adds the numbers up to 10 million using one function `addall()`, and the whole process runs on **one CPU**.
- **Problem:** the other three CPUs are not used at all, and the single process takes a long time to finish.

### 5.1.2 Method 1: four processes

- Create **4 processes**, each adding **2.5 million** numbers.
- This needs **4 `fork()` calls**.
- Each process can run on its own CPU, so the computation time goes down.

**But there are problems:**
- Each process has its **own instructions, data, heap and stack**.
- A large part of these 4 processes is **the same**, so there is a lot of **duplication** of instructions and data.
- **Process management and IPC** (inter-process communication) are required.

### 5.1.3 Method 2: four threads

- Create **4 threads under 1 process** using **Pthreads**.
- Each thread runs on a **separate CPU**.
- The threads **share** the common instructions, parameters, heap, etc.
- But **each thread has its own stack**.
- Each thread adds **2.5 million** numbers.
- **Threads are lighter than processes.**
- **Very few or no system calls** are needed to create threads.

### 5.1.4 Process vs thread (comparison from the slides)

| Point | 4 Processes | 4 Threads in 1 Process |
| --- | --- | --- |
| What is copied/kept | Each has its own instructions, data, heap, stack | Instructions, parameters, heap shared; only the **stack is separate** |
| Creation | 4 `fork()` calls | Very few or no system calls |
| Communication | Process management and IPC required | Threads share data, so no IPC needed |
| Weight | Heavyweight | **Lighter** than processes |

### 5.1.5 What is a thread

- A **thread** is a **separate stream of execution within a single process**.
- Threads of one process are **not isolated** from each other (they share the process's memory).
- The state of a thread is stored in the **Thread Control Block (TCB)**, which contains its **registers and stack**.
- Threads give a way to perform **multiple tasks concurrently**.
- Each thread has: **Thread ID**, **Program counter**, **Register set**, **Stack**.

### 5.1.6 Single-threaded and multithreaded processes

- **Single-threaded process:** one set of code, data, files, registers and stack — one flow of control. It is called a **heavyweight process**.
- **Multithreaded process:** code, data and files are **shared**, but each thread has its **own registers and stack**. It is called a **lightweight process**.

```
Single-threaded (heavyweight)        Multithreaded (lightweight)
┌──────────────────────────┐         ┌──────────────────────────────────────┐
│ code | data | files      │         │ code | data | files   (shared)       │
│ registers | stack        │         │ regs | regs | regs    (one per thread)│
│ one thread               │         │ stack| stack| stack   (one per thread)│
└──────────────────────────┘         └──────────────────────────────────────┘
```

### 5.1.7 Merits of using threads

- Threads can be **created and destroyed quickly** compared with processes.
- Applications can use threads to run some functions **in the background**.
- Threads can **share the same address space**.
- **Switching between threads takes less time**, because the state record to save is smaller.

### 5.1.8 Thread scheduling

- Threads are scheduled on the CPU **independently**.
- The state of each executing thread is kept **separately**.
- If a process is **suspended**, **all its threads are suspended**.
- If a process is **terminated**, **all its threads are terminated**.
- A thread also has states like **ready, running, waiting (blocked)**.

### 5.1.9 Threads: pros and cons

| Advantages of multithreading | Disadvantages of multithreading |
| --- | --- |
| Easy to share resources | Threads compete for acquiring memory |
| Faster to create | Thread safety must be ensured |
| | An error in one thread can disturb the other threads because resources are shared |

**Considerations for future design:** handling signals is tricky; all threads must run the same program.

---

## 5.2 User vs. Kernel Threads

### 5.2.1 Types of threads

There are two types: **User-Level Threads (ULT)** and **Kernel-Level Threads (KLT)**.

> **Note (from the slide):** this is about threads for *user processes*. Both ULTs and KLTs execute in user mode. An OS may have its own threads, but that is not being discussed here.

### 5.2.2 Thread management

| User-Level Threads (ULTs) | Kernel-Level Threads (KLTs) |
| --- | --- |
| Managed by **applications and a user-level thread library** | **Created and managed by the kernel** |
| The **kernel is not aware** of these threads | Also called **lightweight processes** |

### 5.2.3 Relationship between ULT states and process states

With ULTs, the kernel only sees the **process**; the thread library decides which **thread** runs. So a thread's state and the process state can look different. The slide shows Process B with Thread 1 and Thread 2 in four situations:

| Case | Thread 1 | Thread 2 | Process B | What it means |
| --- | --- | --- | --- | --- |
| (a) | Ready | **Running** | **Running** | Normal case: thread 2 is running inside the running process |
| (b) | Ready | Running (library's view) | **Blocked** | Thread 2 made a blocking system call (like I/O). The kernel blocks the **whole process**. The library still shows thread 2 as "running" |
| (c) | Ready | Running (library's view) | **Ready** | Time slice of the process ended (clock interrupt). The process goes to Ready; thread 2 is still "running" in the library's view |
| (d) | **Running** | **Blocked** | **Running** | Thread 2 must wait for thread 1, so the library blocks thread 2 and runs thread 1. The kernel sees no change; the process keeps running |

**Key idea:** a ULT shown as "Running" is really executing only when its process is also "Running".

### 5.2.4 Merits and demerits of ULT

**Merits (+)**
- Can be implemented in an OS that **does not support threading**.
- **Fast creation and switching.**
- **Does not need a system call.**

**Demerits (−)**
- A process with many threads still **competes like one single-threaded process**.
- Scheduling decisions **cannot favour** processes with a larger number of threads.
- If **one thread makes a system call, all other threads get blocked**.

**Solution — Jacketing:** it **converts a blocking system call into a non-blocking system call**.

*(The slide figure shows two processes in user space, each with its own **run-time system** and **thread table**; the kernel has only the **process table**. That is why the kernel does not know about the threads.)*

### 5.2.5 Merits and demerits of KLT

**Merits (+)**
- The **thread table is stored in kernel space**, so the kernel knows how many threads a process has.
- The OS can give **more time quantum** to a process with a large number of threads.
- Better for applications that **frequently block**.
- **One thread making a system call does not block the others.**

**Demerits (−)**
- **Slow.**
- **Larger overhead** because of kernel-level management.
- Moving control from one thread to another in the same process needs a **mode switch to the kernel**.

### 5.2.6 ULT vs KLT

| Point | User-Level Threads | Kernel-Level Threads |
| --- | --- | --- |
| Managed by | Application + user-level thread library | Kernel |
| Kernel aware? | No | Yes (thread table in kernel space) |
| Creation / switching | Fast, no system call | Slow, needs mode switch to kernel |
| One thread makes a system call | All threads block | Other threads are not blocked |
| Scheduling | Cannot favour processes with more threads | Can give more time quantum to such processes |
| OS support needed | Works even on an OS without thread support | OS must support threads |
| Main weakness / fix | Blocking calls — fix is **Jacketing** | Slow, larger overhead |

---

## 5.3 Multithreading Models

A model shows **how user threads are connected to kernel threads**. The three models are **One-to-One, Many-to-One, Many-to-Many**.

### 5.3.1 Many-to-One
- **Many user-level threads are mapped to a single kernel thread.**

```
user  user  user  user
  \    |    |    /
     kernel thread
```

### 5.3.2 One-to-One
- **Each user-level thread maps to one kernel thread.**
- Examples: **Windows NT/XP/2000**, **Linux**.

```
user   user   user   user
 |      |      |      |
kernel kernel kernel kernel
```

### 5.3.3 Many-to-Many
- **Many user-level threads are mapped to many kernel threads.**
- It allows the OS to **create a sufficient number of kernel threads**.
- Example: **Windows NT/2000**.

```
user  user  user  user
   \    |    |    /
  kernel  kernel  kernel
```

### 5.3.4 Comparison

| Model | Mapping | Example (from slides) |
| --- | --- | --- |
| Many-to-One | many user : 1 kernel | — |
| One-to-One | 1 user : 1 kernel | Windows NT/XP/2000, Linux |
| Many-to-Many | many user : many kernel | Windows NT/2000 |

---

## 5.4 Threading Issues

The slide lists five issues: **(1) use of fork() and exec(), (2) signal handling, (3) thread pools, (4) thread safety, (5) thread-specific data.**

### 5.4.1 Use of fork(), exec(), exit()
- **Question:** does `fork()` duplicate **only the calling thread** or **all threads**?
- A few UNIX systems keep **two versions of `fork()`** so that both options are available.
- **`exec()`:** the program given in the parameter of `exec()` **replaces the entire process, including all threads**.
- **Recommendation:** in a process with multiple threads, use `fork()` only together with `exec()` (the slide says "use fork() only after exec()").

### 5.4.2 Signal handling
- **Signals** are used to **tell a process about an event**.
- A **signal handler** processes signals in three steps:
  1. A signal is **generated** by a particular event.
  2. The signal is **delivered** to a process.
  3. The signal is **handled**.
- **Signal delivery options** in a multithreaded process:
  - to the **intended thread**,
  - to **every thread** in the intended process,
  - to **certain threads** in the process,
  - **assign one specific thread** to receive all signals for the process.

### 5.4.3 Thread pools
- **Create and keep** a number of threads in a **pool**.
- **Give work** to the threads as needed.
- It is a **faster** way to handle a request: use an **existing thread** instead of creating a new one.
- It **limits the number of threads** in the application(s) to the size of the pool.

### 5.4.4 Thread safety
A function is **thread-safe** when it can be called by **many threads at the same time without causing any disturbance**.

Example of a function that is **not** thread-safe:

```c
static int glob = 0;

static void Incr(int loops) {
    int loc, j;
    for (j = 0; j < loops; j++) {
        loc = glob;      // read the shared value
        loc++;           // change the local copy
        glob = loc;      // write it back
    }
}
```

It uses **global or static values that are shared by all threads**. Two threads can read the same `glob`, both add one, and write back the same value — so one update is lost.

### 5.4.5 How to ensure thread safety
1. **Serialize the function** — keep the critical section **locked** so only one thread uses it at a time and the others stay out.
2. Use only **thread-safe system functions**.
3. **Avoid global and static variables.**

### 5.4.6 Thread-specific data
- Makes existing functions **thread-safe**.
  - May be slightly **less efficient than being reentrant**.
- Lets **each thread have its own copy of data** — **per-thread storage** for a function.
- Useful when you **do not control how threads are created** (for example, when using a **thread pool**).

---

## 5.5 Pthreads

### 5.5.1 Thread libraries
- A thread library gives the programmer an **API for creating and managing threads**.
- Two main ways to implement it: a library **entirely in user space**, or a **kernel-level library** supported by the OS.
- Three main thread libraries in use today: **POSIX Pthreads, Win32, Java**.

### 5.5.2 POSIX Pthreads
- Can be used on **Linux** systems.
- A program using the Pthreads API must be compiled with **`-pthread`** or **`-lpthread`**.

```c
#include <pthread.h>
pthread_t pthread_self();   // returns the ID of the current (this) thread
```

### 5.5.3 The pthread library calls

| Purpose | Call | Meaning of parameters |
| --- | --- | --- |
| **Create** a thread in a process | `int pthread_create(pthread_t *thread, const pthread_attr_t *attr, void *(*start_routine)(void *), void *arg);` | `thread` = thread identifier (TID); `attr` = attributes; `start_routine` = pointer to the function that starts running in the new thread; `arg` = argument to that function |
| **Destroy** (end) a thread | `void pthread_exit(void *retval);` | `retval` = value returned |
| **Join** — wait for a specific thread to complete | `int pthread_join(pthread_t thread, void **retval);` | `thread` = TID of the thread to wait for; `retval` = exit status of that thread |

### 5.5.4 Example program: four-thread sum
This is the program for the 4-CPU scenario in 5.1.

```c
#include <pthread.h>
#include <stdio.h>

unsigned long sum[4];

void *thread_fn(void *arg) {
    long id = (long) arg;
    int start = id * 2500000;
    int i = 0;
    while (i < 2500000) {
        sum[id] += (i + start);
        i++;
    }
    return NULL;
}

int main() {
    pthread_t t1, t2, t3, t4;

    pthread_create(&t1, NULL, thread_fn, (void *)0);
    pthread_create(&t2, NULL, thread_fn, (void *)1);
    pthread_create(&t3, NULL, thread_fn, (void *)2);
    pthread_create(&t4, NULL, thread_fn, (void *)3);

    pthread_join(t1, NULL);
    pthread_join(t2, NULL);
    pthread_join(t3, NULL);
    pthread_join(t4, NULL);

    printf("%lu\n", sum[0] + sum[1] + sum[2] + sum[3]);
    return 0;
}
```

**Note (from the slide):** you need to **link the pthread library**:
```
$ gcc threads.c -lpthread
$ ./a.out
```

**How it works (simple):**
- `sum[4]` is global, so all threads can see it, and each thread writes only to **its own slot** `sum[id]`.
- The number `0–3` passed as `arg` tells each thread which quarter of the numbers to add.
- `main` **joins** all four threads first, and only then adds the four partial sums.

### 5.5.5 Terminating a thread
```c
#include <pthread.h>
void pthread_exit(return_value);
```
A thread terminates in one of these cases:
1. It **completes its function** and returns a value.
2. A **`pthread_cancel()` request** is received by the thread.
3. The **thread itself starts termination** (`pthread_exit`).
4. The **process of the threads terminates**.

### 5.5.6 Thread cancellation
- **`pthread_cancel()`** terminates a thread **before it has completed its execution**.
- Whether the thread is cancelled depends on its **state** and **type**.

**States**

| State | Meaning |
| --- | --- |
| `PTHREAD_CANCEL_DISABLE` | Thread **cannot** be cancelled |
| `PTHREAD_CANCEL_ENABLE` | **Default state.** Thread **can** be cancelled |

**Two types of cancellation**

| Type | Meaning | Constant |
| --- | --- | --- |
| **Asynchronous cancellation** | Terminates the target thread **immediately** | `PTHREAD_CANCEL_ASYNCHRONOUS` |
| **Deferred cancellation** | The target thread **periodically checks** whether it should be cancelled; it is cancelled when it reaches a **cancellation point** | `PTHREAD_CANCEL_DEFERRED` |

---

## 5.6 Linux Threads

- In Linux, threads are called **tasks**.
- Tasks are created using the **`clone()` system call**.
- `clone()` lets a child task **share the address space of the parent task (process)**.

---

## 5.7 Windows XP Threads

- Windows XP uses a **one-to-one mapping** of threads with kernel-level threads.
- Each thread contains:
  - a **unique thread ID**,
  - a **set of registers**,
  - **separate user and kernel stacks**,
  - a **private data storage area**.
- These together are called the **context of the thread**.
- The primary data structures of a thread are **ETHREAD** (executive thread block), **KTHREAD** (kernel thread block) and **TEB** (thread environment block).

**What the slide figure shows:**

| Structure | Where | Contents shown in the figure |
| --- | --- | --- |
| **ETHREAD** | Kernel space | Thread start address, pointer to parent process, pointer to KTHREAD |
| **KTHREAD** | Kernel space | Scheduling and synchronization information, kernel stack, pointer to TEB |
| **TEB** | User space | Thread identifier, user stack, thread-local storage |

---
---

# WEEK 6 — INTER PROCESS COMMUNICATION

## 6.1 Background

### 6.1.1 Why synchronization is needed
- Processes can execute **concurrently**.
- A process can be **interrupted at any moment**, even when it has only partly finished.
- **Concurrent access to shared data may cause data inconsistency.**
- A **mechanism is needed** to keep data consistent so that cooperating processes run in an orderly way.

### 6.1.2 Producer–consumer
- There is a **buffer of n slots**; each slot holds one unit of data.
- Two processes work on it: **Producer** and **Consumer**.
  - The producer tries to put data into an **empty** slot.
  - The consumer tries to take data from a **filled** slot.
  - The producer must **not insert when the buffer is full**.
  - The consumer must **not remove when the buffer is empty**.
  - They should **not insert and remove at the same time**.

A shared variable `count` keeps the number of filled slots (starts at 0).

```c
// Producer
int count = 0;
void producer(void) {
    int itemP;
    while (1) {
        Produce_item(itemP);
        while (count == n);        // buffer full: wait
        buffer[in] = itemP;
        in = (in + 1) % n;
        count = count + 1;
    }
}

// Consumer
void consumer(void) {
    int itemC;
    while (1) {
        while (count == 0);        // buffer empty: wait
        itemC = buffer[out];
        out = (out + 1) % n;
        count = count - 1;
    }
}
```

`count = count + 1` is really **three machine steps**: `Load Rp, m[count]` → `Increment Rp` → `Store m[count], Rp`. In the same way, `count = count - 1` is `Load Rc` → `Decrement Rc` → `Store`.

### 6.1.3 Race condition
`counter++` is done as `register1 = counter; register1 = register1 + 1; counter = register1`, and `counter--` as `register2 = counter; register2 = register2 - 1; counter = register2`.

Take `count = 5` at the start and this interleaving:

| Step | Who | Action | Value |
| --- | --- | --- | --- |
| S0 | producer | `register1 = counter` | register1 = 5 |
| S1 | producer | `register1 = register1 + 1` | register1 = 6 |
| S2 | consumer | `register2 = counter` | register2 = 5 |
| S3 | consumer | `register2 = register2 - 1` | register2 = 4 |
| S4 | producer | `counter = register1` | counter = 6 |
| S5 | consumer | `counter = register2` | **counter = 4** |

One item was produced and one consumed, so the right answer is **5**, but we got **4**. This is a **race condition**: the result depends on the **order** in which the processes run their steps.

---

## 6.2 The Critical-Section Problem

### 6.2.1 Definition
- Assume **n processes** `{p0, p1, …, pn-1}`.
- Each process has a **critical section**, a part of code where it may change common variables, update a table, write into a file, etc.
- **When one process is in its critical section, no other process may enter its critical section.**
- The **critical-section problem** is to design an algorithm so that the processes can cooperate.
- Each process must **take permission** to enter its critical section.

### 6.2.2 General structure of process Pi

```c
do {
    entry section        // ask permission
        critical section
    exit section         // announce leaving
        remainder section
} while (true);
```

### 6.2.3 A simple lock picture and the `turn` algorithm

The slide shows the idea with a variable `S` (`S = 1` means the critical section is free):

| State | P1 | P2 | S |
| --- | --- | --- | --- |
| 1 | In non-critical section | In non-critical section | 1 |
| 2 | **Enters** critical section, sets `S = 0` | In non-critical section | 0 |
| 3 | Executing in critical section | Wants to enter but **cannot**, as `S = 0` | 0 |
| 4 | Leaves critical section, sets `S = 1` | Enters critical section (as `S = 1`) and sets `S = 0` | 1 → 0 |

**Algorithm for process Pi (shared variable `turn`):**

```c
do {
    while (turn == j);      // wait while it is the other's turn
        critical section
    turn = j;               // give the turn to the other process
        remainder section
} while (true);
```

*Easy reading:* Pi waits as long as it is Pj's turn; after its critical section Pi gives the turn to Pj. This keeps both from entering together, but the processes are forced to take turns one after the other. (This weakness is what Peterson's solution fixes.)

### 6.2.4 Three requirements of a solution

1. **Mutual exclusion** — if process Pi is executing in its critical section, no other process can be executing in its critical section.
2. **Progress** — if no process is in its critical section and some processes want to enter, only those **not in their remainder sections** can take part in deciding who enters next, and this decision **cannot be postponed forever**.
3. **Bounded waiting** — there is a **limit** on how many times other processes may enter their critical sections **after** a process has made a request and **before** that request is granted.

### 6.2.5 Critical-section handling in the OS
Two approaches, depending on the kernel:

| Kernel | Meaning |
| --- | --- |
| **Preemptive** | Allows a process to be preempted (taken off the CPU) while running in kernel mode |
| **Non-preemptive** | A process runs until it exits kernel mode |

---

## 6.3 Peterson's Solution

- A **good solution for two processes**; a classic **software-based** solution.
- It **may not work correctly on modern computer architectures**, but it gives a good algorithmic description of how to meet **mutual exclusion, progress and bounded waiting**.
- Restricted to **two processes**, Pi and Pj, that take turns between their critical and remainder sections.
- **Assumption:** the `load` and `store` machine instructions are **atomic** (cannot be interrupted).

**Two shared variables:**

| Variable | Meaning |
| --- | --- |
| `int turn;` | Whose **turn** it is to enter the critical section |
| `boolean flag[2];` | Shows whether a process is **ready** to enter. `flag[i] = true` means Pi is ready |

```c
// Process Pi                              // Process Pj
do {                                       do {
    flag[i] = true;                            flag[j] = true;
    turn = j;                                  turn = i;
    while (flag[j] && turn == j);              while (flag[i] && turn == i);
        critical section                           critical section
    flag[i] = false;                           flag[j] = false;
        remainder section                          remainder section
} while (true);                            } while (true);
```

**Easy reading:** "I am ready (`flag[i] = true`), but I politely give you the turn (`turn = j`). I wait only if you are also ready **and** it is your turn." If the other process is not interested, `flag[j]` is false and Pi walks in directly. If both want to enter, whichever wrote `turn` last waits, so only one enters.

---

## 6.4 Synchronization Hardware

- Many systems give **hardware support** for critical-section code.
- All solutions are based on **locking** — protecting critical regions with locks.
- **Uniprocessors** — can **disable interrupts**, so the running code runs **without preemption**. This is generally **too inefficient on multiprocessor systems**, and OSs using it are **not broadly scalable**.
- Modern machines provide special **atomic hardware instructions** (**atomic = non-interruptible**) that either
  - **test a memory word and set its value**, or
  - **swap the contents of two memory words**.

### 6.4.1 Solution using locks
```c
do {
    acquire lock
        critical section
    release lock
        remainder section
} while (TRUE);
```

### 6.4.2 test_and_set instruction
```c
boolean test_and_set(boolean *target) {
    boolean rv = *target;     // remember old value
    *target = TRUE;           // set to TRUE
    return rv;                // return old value
}
```
1. Executed **atomically**.
2. **Returns the original value** of the passed parameter.
3. **Sets the new value** of the parameter to **TRUE**.

**Solution** (shared boolean `lock`, initially FALSE):
```c
do {
    while (test_and_set(&lock));    // do nothing
        /* critical section */
    lock = false;
        /* remainder section */
} while (true);
```
*Easy reading:* if `lock` was FALSE, the call returns FALSE (loop ends, you enter) and sets it TRUE at the same moment. Others now get TRUE and keep waiting until you set `lock = false`.

### 6.4.3 compare_and_swap instruction
```c
int compare_and_swap(int *value, int expected, int new_value) {
    int temp = *value;
    if (*value == expected)
        *value = new_value;
    return temp;
}
```
1. Executed **atomically**.
2. **Returns the original value** of `value`.

**Solution** (shared integer `lock`, initially 0):
```c
do {
    while (compare_and_swap(&lock, 0, 1) != 0);   // do nothing
        /* critical section */
    lock = 0;
        /* remainder section */
} while (true);
```

### 6.4.4 Bounded-waiting mutual exclusion with test_and_set
```c
do {
    waiting[i] = true;
    key = true;
    while (waiting[i] && key)
        key = test_and_set(&lock);
    waiting[i] = false;

        /* critical section */

    j = (i + 1) % n;
    while ((j != i) && !waiting[j])
        j = (j + 1) % n;
    if (j == i)
        lock = false;
    else
        waiting[j] = false;

        /* remainder section */
} while (true);
```
*Easy reading:* when a process leaves, it looks at the other processes **in circular order** (i+1, i+2, …). If someone is waiting, it hands the critical section directly to that process (`waiting[j] = false`); if nobody waits, it releases the lock. This way no process waits forever, so **bounded waiting** is met.

---

## 6.5 Semaphores

### 6.5.1 Definition
- A **semaphore** is a **robust synchronization tool** used by processes to synchronize their activities.
- Semaphore **S** is an **integer variable**.
- It can be accessed only through two **indivisible (atomic)** operations: **`wait()`** and **`signal()`** (originally called **P()** and **V()**).

```c
wait(S) {
    while (S <= 0);    // busy wait
    S--;
}

signal(S) {
    S++;
}
```

### 6.5.2 Semaphore usage
- **Counting semaphore** — integer value can range over an **unrestricted domain**.
- **Binary semaphore** — value can be only **0 or 1**; the same as a **mutex lock**.
- Semaphores can solve various synchronization problems.
- A **counting semaphore S can be implemented as a binary semaphore**.

**Example — P1 and P2 where S1 must happen before S2.** Create a semaphore `synch` initialized to **0**:

```c
// P1                   // P2
S1;                     wait(synch);
signal(synch);          S2;
```
P2 cannot pass `wait(synch)` until P1 has finished S1 and called `signal(synch)`.

### 6.5.3 Semaphore implementation and the busy-waiting problem
- It must be ensured that **no two processes execute `wait()` and `signal()` on the same semaphore at the same time**.
- So the implementation itself becomes a **critical-section problem**, with the wait and signal code placed inside a critical section.
- This can bring **busy waiting** into the implementation. But the implementation code is **short**, and there is **little busy waiting if the critical section is rarely occupied**.

**What is the busy-waiting problem?**
- The main disadvantage of the semaphore definition above is that it **requires busy waiting**.
- While one process is in its critical section, any other process that tries to enter **must loop continuously in the entry code** (wasting CPU time).

### 6.5.4 Implementation with no busy waiting
**How to overcome busy waiting:**
- Change the definition of `wait()` and `signal()`.
- When a process executes `wait()` and finds the semaphore value **not positive**, it must wait — but instead of busy waiting, the process **blocks itself**.
- The **block** operation puts the process into a **waiting queue attached to the semaphore** and changes its state to **waiting**. Control goes to the **CPU scheduler**, which picks another process.
- A blocked process is **restarted** when some other process executes `signal()`. The **wakeup()** operation changes it from the **waiting state to the ready state**.

Each semaphore has a waiting queue; each entry has two items: **value** (integer) and a **pointer to the next record** in the list. Two operations: **block** and **wakeup**.

```c
typedef struct {
    int value;
    struct process *list;
} semaphore;

wait(semaphore *S) {
    S->value--;
    if (S->value < 0) {
        add this process to S->list;
        block();
    }
}

signal(semaphore *S) {
    S->value++;
    if (S->value <= 0) {
        remove a process P from S->list;
        wakeup(P);
    }
}
```

### 6.5.5 Deadlock, starvation, priority inversion

**Deadlock** — two or more processes wait **indefinitely** for an event that can be caused only by one of the waiting processes.

Let S and Q be two semaphores initialized to 1:

```c
// P0                 // P1
wait(S);              wait(Q);
wait(Q);              wait(S);
...                   ...
signal(S);            signal(Q);
signal(Q);            signal(S);
```
If P0 runs `wait(S)` and P1 runs `wait(Q)`, then P0 waits for Q (held by P1) and P1 waits for S (held by P0) — neither can go on.

**Starvation** — **indefinite blocking**. A process may **never be removed from the semaphore queue** in which it is waiting.

**Priority inversion** — a scheduling problem when a **lower-priority process holds a lock needed by a higher-priority process**. It is solved by the **priority-inheritance protocol**.

---

## 6.6 Classic Problems of Synchronization

These problems are used to **test newly proposed synchronization schemes**: **Bounded-Buffer, Readers–Writers, Dining-Philosophers.**

### 6.6.1 Bounded-buffer problem
- **n buffers**, each can hold one item.

| Semaphore | Initial value | Purpose |
| --- | --- | --- |
| `mutex` | 1 | Only one process touches the buffer at a time |
| `full` | 0 | Number of filled slots |
| `empty` | n | Number of empty slots |

```c
// Producer
do {
    wait(empty);     // wait until empty > 0, then decrement empty
    wait(mutex);     // acquire lock
    /* add data to buffer */
    signal(mutex);   // release lock
    signal(full);    // increment full
} while (TRUE);

// Consumer
do {
    wait(full);      // wait until full > 0, then decrement full
    wait(mutex);     // acquire lock
    /* remove data from buffer */
    signal(mutex);   // release lock
    signal(empty);   // increment empty
} while (TRUE);
```

### 6.6.2 Readers–writers problem
- A **database is shared** among several concurrent processes.
- Some processes only **read** (**readers**); others **update — read and write** (**writers**).
- If **two readers** access the shared data together, **no problem** occurs.
- If a **writer and any other process** (reader or writer) access it together, **chaos may result**.
- So **writers must have exclusive access** to the shared database.

**Solution using semaphores** — two semaphores and one integer:
1. `mutex` — semaphore (initial **1**); gives mutual exclusion when **`readcount`** is updated, i.e. when a reader enters or leaves.
2. `wrt` — semaphore (initial **1**); **common to readers and writers**.
3. `readcount` — integer (initial **0**); **how many processes are reading** right now.

```c
// Writer
do {
    wait(wrt);            // writer requests the critical section
    /* writing is performed */
    signal(wrt);          // leaves the critical section
} while (true);

// Reader
do {
    wait(mutex);
    readcnt++;            // one more reader
    if (readcnt == 1)
        wait(wrt);        // first reader blocks writers
    signal(mutex);        // other readers can enter now

    /* reading is performed */

    wait(mutex);
    readcnt--;            // a reader leaves
    if (readcnt == 0)
        signal(wrt);      // last reader lets writers in
    signal(mutex);
} while (true);
```

**Variations of the problem**
- **First variation** — no reader is kept waiting unless a writer already has permission to use the shared object.
- **Second variation** — once a writer is ready, it does its write **as soon as possible**.
- **Both may cause starvation**, which leads to even more variations.
- On some systems the problem is solved by the **kernel providing reader–writer locks**.

### 6.6.3 Dining-philosophers problem
- Philosophers can only **think and eat, alternately**.
- They **don't interact with neighbours**; sometimes they try to pick up **2 chopsticks (one at a time)** to eat from the bowl.
- They need **both** chopsticks to eat, and **release both** when finished.
- For **5 philosophers**, the shared data is: a **bowl of rice** (data set) and **semaphore `chopstick[5]`** initialized to **1**.

**Structure of philosopher i:**
```c
do {
    wait(chopstick[i]);
    wait(chopstick[(i + 1) % 5]);
    // eat
    signal(chopstick[i]);
    signal(chopstick[(i + 1) % 5]);
    // think
} while (TRUE);
```

**What is the problem with this algorithm?**
- It guarantees that **no two neighbours eat at the same time**, but it **could still create a deadlock**.
- Suppose **all five philosophers become hungry together and each picks up the left chopstick**. All elements of `chopstick` become **0**.
- When each tries to pick up the right chopstick, he is **delayed forever**.

**Possible remedies to avoid deadlock**
1. Allow **at most four** philosophers to sit at the table at the same time.
2. Allow a philosopher to pick up chopsticks **only if both are available** (he must pick them up in a critical section).
3. Use an **asymmetric solution**: an **odd** philosopher picks up the **left** chopstick first and then the right; an **even** philosopher picks up the **right** first and then the left.

---

## 6.7 Monitors

### 6.7.1 Problems with semaphores
Incorrect use of semaphore operations:
- `signal(mutex) … wait(mutex)` (wrong order)
- `wait(mutex) … wait(mutex)`
- **Omitting** `wait(mutex)` or `signal(mutex)` (or both)

Also, **deadlock and starvation are possible**. These mistakes are the reason for monitors.

### 6.7.2 Monitor
- A **convenient and effective mechanism for process synchronization**.
- **Only one process may be active within the monitor at a time.**
- On its own it **lacks the power to model some synchronization schemes** (so condition variables are added).

```
monitor monitor-name
{
    // shared variable declarations
    procedure P1 (…) { …. }
    ...
    procedure Pn (…) { …… }
    initialization code (…) { … }
}
```

**Schematic view:** the monitor has **shared data**, a set of **operations** and **initialization code**; processes wanting to use it wait in an **entry queue**.

```
 entry queue ──►┌──────────────────────────┐
 (waiting       │ shared data              │
  processes)    │ operations (P1 … Pn)     │
                │ initialization code      │
                └──────────────────────────┘
```

### 6.7.3 Condition variables
```c
condition x, y;
```
Two operations are allowed on a condition variable:
- **`x.wait()`** — the process that calls it is **suspended** until another process calls `x.signal()`.
- **`x.signal()`** — **resumes one** of the processes (if any) that called `x.wait()`. If **no process is waiting** on `x`, it has **no effect** on the variable.

**Monitor with condition variables:** the figure shows the same monitor, with **a separate queue for each condition** (x and y) inside it, besides the entry queue.

### 6.7.4 Condition-variable choices
If process **P** calls `x.signal()` and process **Q** is suspended in `x.wait()`, what happens next? **P and Q cannot both run in parallel inside the monitor.** If Q is resumed, P must wait.

Options:
- **Signal and wait**
- **Signal and continue**

Both have merits and demerits — the **language implementer can decide**. Monitors in **Concurrent Pascal** use a compromise. Monitors are also implemented in **Mesa, C#, Java** and other languages.

### 6.7.5 Dining philosophers solution using a monitor
- This is a **deadlock-free** solution. It adds the rule that a philosopher may **pick up his chopsticks only if both are available**.
- We need **three states** for a philosopher: `enum { thinking, hungry, eating } state[5];`
- Philosopher i can set `state[i] = eating` only if his two neighbours are not eating: `state[(i+4)%5] != eating` and `state[(i+1)%5] != eating`.
- We also declare **`condition self[5];`** — philosopher i can **delay himself** when he is hungry but cannot get the chopsticks he needs.

```c
monitor DiningPhilosophers
{
    enum { THINKING, HUNGRY, EATING } state[5];
    condition self[5];

    void pickup(int i) {
        state[i] = HUNGRY;
        test(i);
        if (state[i] != EATING)
            self[i].wait();
    }

    void putdown(int i) {
        state[i] = THINKING;
        // test left and right neighbours
        test((i + 4) % 5);
        test((i + 1) % 5);
    }

    void test(int i) {
        if ((state[(i + 4) % 5] != EATING) &&
            (state[i] == HUNGRY) &&
            (state[(i + 1) % 5] != EATING)) {
            state[i] = EATING;
            self[i].signal();
        }
    }

    initialization_code() {
        for (int i = 0; i < 5; i++)
            state[i] = THINKING;
    }
}
```

Each philosopher i uses the operations in this order:
```c
DiningPhilosophers.pickup(i);
EAT
DiningPhilosophers.putdown(i);
```
**Result: no deadlock, but starvation is possible.**

### 6.7.6 Monitor implementation using semaphores
**Variables**
```c
semaphore mutex;      // (initially = 1)
semaphore next;       // (initially = 0)
int next_count = 0;
```
**Each procedure F** is replaced by:
```c
wait(mutex);
…
body of F;
…
if (next_count > 0)
    signal(next);
else
    signal(mutex);
```
This ensures **mutual exclusion within the monitor**.

**For each condition variable x:**
```c
semaphore x_sem;      // (initially = 0)
int x_count = 0;
```

`x.wait` is implemented as:
```c
x_count++;
if (next_count > 0)
    signal(next);
else
    signal(mutex);
wait(x_sem);
x_count--;
```

`x.signal` is implemented as:
```c
if (x_count > 0) {
    next_count++;
    signal(x_sem);
    wait(next);
    next_count--;
}
```

### 6.7.7 Resuming processes within a monitor
- If **several processes are queued on condition x** and `x.signal()` is executed, **which one should be resumed?**
- **FCFS is frequently not adequate.**
- Use the **conditional-wait** construct **`x.wait(c)`**, where **c is a priority number**.
- The process with the **lowest number (highest priority)** is scheduled next.

### 6.7.8 Single-resource allocation
- A **priority number** is used to allocate a **single resource** among competing processes. It gives the **maximum time** a process plans to use the resource.

```c
R.acquire(t);
...
access the resource;
...
R.release;
```
where **R** is an instance of type `ResourceAllocator`.

```c
monitor ResourceAllocator
{
    boolean busy;
    condition x;

    void acquire(int time) {
        if (busy)
            x.wait(time);
        busy = TRUE;
    }

    void release() {
        busy = FALSE;
        x.signal();
    }

    initialization_code() {
        busy = FALSE;
    }
}
```

---

## 6.8 Synchronization Examples

> **Not covered in the PPTs.** The Week 6_3 overview slide lists "Synchronization Examples", but no slide explains it. Nothing is added here to keep the notes strictly within the PPTs.

## 6.9 Atomic Transactions

> **Not covered in the PPTs.** The Week 6_3 overview slide lists "Atomic transactions", but no slide explains it. Nothing is added here to keep the notes strictly within the PPTs.

---
---

# WEEK 7 — DEADLOCKS

## 7.1 Resources and the Deadlock Problem

### 7.1.1 Resources
- A system consists of **resources**.
- **Resource types** R1, R2, …, Rm — for example **CPU cycles, memory space, I/O devices**.
- Each resource type Ri has **Wi instances**.
- Each process uses a resource in this order: **request → use → release**.
- **Preemptable resources** — can be taken away from a process with **no ill effects**.
- **Non-preemptable resources** — taking them away makes the process **fail**.
- If a request is **denied**, the requesting process must wait: it may be **blocked**, or the request may **fail with an error code**.

### 7.1.2 The deadlock problem
In a computer system, deadlocks arise when members of a group of processes that **hold resources** are **blocked indefinitely** from getting resources **held by other processes in the group**.

### 7.1.3 When do deadlocks happen?
- Process 1 **holds resource A and requests B**.
- Process 2 **holds B and requests A**.
- Both can be blocked, and **neither can proceed** → **DEADLOCK**.

Deadlocks occur when:
- Processes are given **exclusive access** to devices or software constructs (resources), and
- **Each deadlocked process needs a resource held by another deadlocked process.**

### 7.1.4 Formal definition
> *A set of processes is deadlocked if each process in the set is waiting for an event that only another process in the set can cause.*

- Usually the event is the **release of a currently held resource**.
- In a deadlock, none of the processes can **run**, **release resources**, or **be awakened**.

### 7.1.5 Deadlock with semaphores
- Data: semaphore **S1 = 1**, semaphore **S2 = 1**; two processes P1 and P2.

```c
// P1                // P2
wait(S1);            wait(S2);
wait(S2);            wait(S1);
```
If P1 gets S1 and P2 gets S2, then P1 waits for S2 (held by P2) and P2 waits for S1 (held by P1) → deadlock.

---

## 7.2 Deadlock Characterization

### 7.2.1 Four conditions for deadlock
Deadlock can happen **only if all four conditions hold together**:

| Condition | Meaning (from the slides) |
| --- | --- |
| **1. Mutual exclusion** | Each resource is assigned to **only one process** or is available |
| **2. Hold and wait** | A process **holding resources can request additional** ones |
| **3. No preemption** | Previously granted resources **cannot be forcibly taken away** |
| **4. Circular wait** | There is a **circular chain of 2 or more processes**, each waiting for a resource held by the next member of the chain |

### 7.2.2 Resource-allocation graph (RAG)
A set of **vertices V** and a set of **edges E**.
- V has two types:
  - **P = {P1, P2, …, Pn}** — all the **processes**.
  - **R = {R1, R2, …, Rm}** — all the **resource types**.
- **Request edge** — directed edge **Pi → Rj** (Pi requests Rj).
- **Assignment edge** — directed edge **Rj → Pi** (Rj is allocated to Pi).

**Example graph (from the slide):**
- One instance of R1, two instances of R2, one instance of R3, three instances of R4.
- **T1** holds one instance of R2 and is **waiting for an instance of R1**.
- **T2** holds one instance of R1 and one instance of R2, and is **waiting for an instance of R3**.
- **T3** holds one instance of R3.

*Easy reading:* there is **no cycle**, so there is no deadlock. T3 can finish and release R3 → T2 can finish → T1 can finish.

**Resource-allocation graph with a deadlock:** add one more edge — **T3 requests R2**. Now there are cycles:
- T1 → R1 → T2 → R3 → T3 → R2 → T1
- T2 → R3 → T3 → R2 → T2

Both instances of R2 are held by T1 and T2, who are inside the cycles, so **T1, T2, T3 are deadlocked**.

**Graph with a cycle but no deadlock (slide):** R1 and R2 each have two instances. There is a cycle T1 → R1 → T3 → R2 → T1, **but no deadlock**, because T4 (not in the cycle) can release its instance of R2, which can then go to T3 and break the cycle. (T2 can likewise release R1.)

### 7.2.3 Basic facts
- If the graph contains **no cycle** ⇒ **no deadlock**.
- If the graph contains a **cycle**:
  - if there is **only one instance per resource type** ⇒ **deadlock**;
  - if there are **several instances per resource type** ⇒ **possibility of deadlock**.

---

## 7.3 Methods for Handling Deadlocks

Three general approaches (from the slide):

| Approach | Idea |
| --- | --- |
| **Prevent deadlock** | Adopt a policy that **eliminates one of the conditions** |
| **Avoid deadlock** | Make the right **dynamic choices based on the current state of resource allocation** |
| **Detect deadlock** | Try to **detect the presence of deadlock** and take action to **recover** |

---

## 7.4 Deadlock Prevention

**Idea:** make **one of the four necessary conditions impossible.**

1. **Mutual exclusion** — **not required for sharable resources** (for example read-only files); it **must hold for non-sharable resources**.
2. **Hold and wait** — must guarantee that **whenever a process requests a resource, it does not hold any other resources**.
   - Require the process to **request and be allocated all its resources before it begins execution**, **or** allow a process to request resources **only when it has none allocated**.
   - Drawbacks: **low resource utilization; starvation is possible.**
3. **No preemption**
   - If a process holding some resources requests another resource that **cannot be given immediately**, then **all resources it is holding are released**.
   - The preempted resources are added to the **list of resources the process is waiting for**.
   - The process is **restarted only when it can get back its old resources as well as the new ones** it is requesting.
4. **Circular wait** — **impose a total ordering of all resource types**, and require that each process requests resources in an **increasing order of enumeration**.

**Attacking "circular wait" (slide):**
- **Assign an order (number) to the resources.**
- **Always acquire resources in numerical order.** They need not all be acquired at once.
- Circular wait is prevented: a process holding resource **n** cannot wait for resource **m** if **m < n**.
- There is **no way to complete a cycle**: place processes above the highest resource they hold and below any they are requesting — **all arrows point up**.

---

## 7.5 Deadlock Avoidance

Avoidance **requires some additional a priori (advance) information**.
- The simplest and most useful model: each process **declares the maximum number of resources of each type** it may need.
- The avoidance algorithm **dynamically checks the resource-allocation state** to make sure there can **never be a circular-wait condition**.
- The **resource-allocation state** is defined by the number of **available** and **allocated** resources, and the **maximum demands** of the processes.

### 7.5.1 Safe state
- When a process requests an available resource, the system must decide whether **giving it immediately leaves the system in a safe state**.
- The system is in a **safe state** if there is a sequence **<P1, P2, …, Pn>** of **ALL** the processes such that, for each Pi, the resources Pi can still request can be satisfied by **currently available resources + resources held by all Pj with j < i**.

That is:
- If Pi's needs are not immediately available, Pi can **wait until all Pj have finished**.
- When Pj finishes, Pi can get the needed resources, run, **return its resources, and terminate**.
- When Pi terminates, Pi+1 can get its needed resources, and so on.

**Basic facts**
- System in **safe state** ⇒ **no deadlock**.
- System in **unsafe state** ⇒ **possibility of deadlock**.
- **Avoidance** ⇒ make sure the system **never enters an unsafe state**.

*(The slide figure "Safe, Unsafe, Deadlock state" shows: deadlock states are a part of the unsafe states; safe and unsafe states do not overlap.)*

### 7.5.2 Avoidance algorithms
- **Single instance** of a resource type → use a **modified resource-allocation graph**.
- **Multiple instances** of a resource type → use the **Banker's algorithm**.

### 7.5.3 Modified resource-allocation graph scheme (single instance)
- **Claim edge Pi ⇢ Rj** (dashed) — Pi **may request** Rj in the future.
- **Request edge Pi → Rj** — Pi **requests** Rj. A claim edge **converts to a request edge** when the process requests the resource.
- **Assignment edge Rj → Pi** — Rj **was allocated** to Pi. A request edge **converts to an assignment edge** when the resource is allocated.
- When the resource is released, the assignment edge **changes back to a claim edge**.
- Resources must be **claimed a priori** in the system.

**Algorithm:** suppose Pi requests Rj. The request is **granted only if converting the request edge to an assignment edge does not form a cycle** in the graph.

**Slide example:** R1 is assigned to T1, T2 requests R1, and both T1 and T2 have claim edges to R2. If T2 now requests R2, giving R2 to T2 would form a cycle, so it is **not granted** — the slide calls this an **unsafe state**. If T1 then requests R2, a deadlock would occur.

### 7.5.4 Banker's algorithm
- For **multiple instances** of resources.
- Each process must **claim its maximum use in advance**.
- When a process requests a resource, it **may have to wait**.
- When a process gets all its resources, it must **return them in a finite amount of time**.

**Data structures** (n = number of processes, m = number of resource types):

| Structure | Meaning |
| --- | --- |
| **Available** | Vector of length **m**. `Available[j] = k` → k instances of resource type Rj are available |
| **Max** | **n × m** matrix. `Max[i,j] = k` → Pi may request **at most** k instances of Rj |
| **Allocation** | **n × m** matrix. `Allocation[i,j] = k` → Pi is **currently allocated** k instances of Rj |
| **Need** | **n × m** matrix. `Need[i,j] = k` → Pi may **need k more** instances of Rj to finish |

> **Need = Max − Allocation**

**Safety algorithm**
1. Let **Work** and **Finish** be vectors of length m and n. Initialize: `Work = Available`; `Finish[i] = false` for i = 0, 1, …, n−1.
2. Find an i such that both: (a) `Finish[i] = false` and (b) `Need_i ≤ Work`. If no such i exists, go to step 4.
3. `Work = Work + Allocation_i`; `Finish[i] = true`; go to step 2.
4. If `Finish[i] = true` for all i, the system is in a **safe state**.

*Easy reading:* pick any unfinished process whose remaining need fits in what is free; pretend it finishes and gives back everything it holds; repeat. If everyone can finish, the state is safe.

**Resource-request algorithm for process Pi**
`Request_i` = request vector of Pi. If `Request_i[j] = k`, Pi wants k instances of Rj.
1. If `Request_i ≤ Need_i`, go to step 2. Otherwise **raise an error** — the process has exceeded its maximum claim.
2. If `Request_i ≤ Available`, go to step 3. Otherwise **Pi must wait**, since resources are not available.
3. **Pretend** to allocate the requested resources to Pi by changing the state:
   - `Available = Available − Request_i`
   - `Allocation_i = Allocation_i + Request_i`
   - `Need_i = Need_i − Request_i`

   Then run the safety algorithm:
   - If **safe** ⇒ the resources are **allocated** to Pi.
   - If **unsafe** ⇒ **Pi must wait**, and the **old resource-allocation state is restored**.

### 7.5.5 Example of Banker's algorithm
5 processes P0–P4; 3 resource types: **A (10 instances), B (5 instances), C (7 instances)**.

**Snapshot at time T0**

| | Allocation (A B C) | Max (A B C) | Available (A B C) | Need = Max − Allocation (A B C) |
| --- | --- | --- | --- | --- |
| P0 | 0 1 0 | 7 5 3 | **3 3 2** | 7 4 3 |
| P1 | 2 0 0 | 3 2 2 | | 1 2 2 |
| P2 | 3 0 2 | 9 0 2 | | 6 0 0 |
| P3 | 2 1 1 | 2 2 2 | | 0 1 1 |
| P4 | 0 0 2 | 4 3 3 | | 4 3 1 |

**Is the system safe?** Work = (3 3 2).

| Step | Pick | Check Need ≤ Work | Work after adding its Allocation |
| --- | --- | --- | --- |
| 1 | P1 | (1 2 2) ≤ (3 3 2) ✓ | (3 3 2) + (2 0 0) = (5 3 2) |
| 2 | P3 | (0 1 1) ≤ (5 3 2) ✓ | (5 3 2) + (2 1 1) = (7 4 3) |
| 3 | P4 | (4 3 1) ≤ (7 4 3) ✓ | (7 4 3) + (0 0 2) = (7 4 5) |
| 4 | P2 | (6 0 0) ≤ (7 4 5) ✓ | (7 4 5) + (3 0 2) = (10 4 7) |
| 5 | P0 | (7 4 3) ≤ (10 4 7) ✓ | (10 4 7) + (0 1 0) = (10 5 7) |

The system is in a **safe state**; the safe sequence is **<P1, P3, P4, P2, P0>**.

**Now P1 requests (1, 0, 2).**
1. `Request ≤ Need`? (1 0 2) ≤ (1 2 2) ✓
2. `Request ≤ Available`? (1 0 2) ≤ (3 3 2) ✓
3. Pretend to allocate. New state:

| | Allocation | Need | Available |
| --- | --- | --- | --- |
| P0 | 0 1 0 | 7 4 3 | **2 3 0** |
| P1 | **3 0 2** | **0 2 0** | |
| P2 | 3 0 2 | 6 0 0 | |
| P3 | 2 1 1 | 0 1 1 | |
| P4 | 0 0 2 | 4 3 1 | |

Safety check from Work = (2 3 0): P1 (0 2 0) → Work (5 3 2); P3 → (7 4 3); P4 → (7 4 5); P0 → (7 5 5); P2 → (10 5 7). The sequence **<P1, P3, P4, P0, P2>** is safe, so **the request is granted immediately**.

**Questions on the slide (in the state after P1's request was granted):**
- **Can P4's request (3, 3, 0) be granted?** `Request ≤ Need` ✓ ((3 3 0) ≤ (4 3 1)) but `Request ≤ Available`? (3 3 0) ≤ (2 3 0) ✗ — only 2 of A are free. **No — P4 must wait.**
- **Can P0's request (0, 2, 0) be granted?** (0 2 0) ≤ Need (7 4 3) ✓ and ≤ Available (2 3 0) ✓. Pretend: Available = (2 1 0), P0 Allocation = (0 3 0), P0 Need = (7 2 3). Now check: P0 (7 2 3), P1 (0 2 0), P2 (6 0 0), P3 (0 1 1), P4 (4 3 1) — **none** of these fit in Work (2 1 0). The state is **unsafe**, so **the request is not granted**; P0 must wait and the old state is restored.

### 7.5.6 Safe and unsafe state examples (slides)

**Q1. Determination of a safe state**
Here **C** = claim matrix (maximum claim of each process), **A** = allocation matrix, **C − A** = what each process may still need, **R** = total resource vector, **V** = available vector.

Initial state: R = (9 3 6), V = (0 1 1).

| | C (R1 R2 R3) | A | C − A |
| --- | --- | --- | --- |
| P1 | 3 2 2 | 1 0 0 | 2 2 2 |
| P2 | 6 1 3 | 6 1 2 | 0 0 1 |
| P3 | 3 1 4 | 2 1 1 | 1 0 3 |
| P4 | 4 2 2 | 0 0 2 | 4 2 0 |

| Step | Who can run to completion | Reason | New V |
| --- | --- | --- | --- |
| (a) → (b) | **P2** | C−A = (0 0 1) ≤ V = (0 1 1) | (6 2 3) |
| (b) → (c) | **P1** | (2 2 2) ≤ (6 2 3) | (7 2 3) |
| (c) → (d) | **P3** | (1 0 3) ≤ (7 2 3) | (9 3 4) |
| (d) → end | **P4** | (4 2 0) ≤ (9 3 4) | (9 3 6) |

All processes finish, so the state is **safe** (sequence P2, P1, P3, P4).

**Determination of an unsafe state**
Initial state (a): R = (9 3 6), V = (1 1 2). Allocation: P1 (1 0 0), P2 (5 1 1), P3 (2 1 1), P4 (0 0 2). C − A: P1 (2 2 2), P2 (1 0 2), P3 (1 0 3), P4 (4 2 0).

**(b) P1 requests one unit each of R1 and R3.** If granted: P1 Allocation = (2 0 1), V = (0 1 1), P1's C − A = (1 2 1). Now check each process against V = (0 1 1): P1 needs (1 2 1) ✗, P2 needs (1 0 2) ✗, P3 needs (1 0 3) ✗, P4 needs (4 2 0) ✗. **No process can finish → unsafe state**, so this request should not be granted.

**Question on the slide:** a system uses the Banker's algorithm. P0, P1, P2 are processes and R0, R1, R2 are resource types.

| | Maximum need (R0 R1 R2) | Current allocation (R0 R1 R2) | Need = Max − Allocation |
| --- | --- | --- | --- |
| P0 | 4 1 2 | 1 0 2 | 3 1 0 |
| P1 | 1 5 1 | 0 3 1 | 1 2 0 |
| P2 | 1 2 3 | 1 0 2 | 0 2 1 |

Available = (2 2 0).

**(a) Show that the system can be in this state.** The state is safe if some order lets everybody finish. Work = (2 2 0): P1 needs (1 2 0) ≤ (2 2 0) ✓ → Work = (2 5 1); P2 needs (0 2 1) ≤ (2 5 1) ✓ → Work = (3 5 3); P0 needs (3 1 0) ≤ (3 5 3) ✓. The sequence **<P1, P2, P0>** is a safe sequence, so the system can be in this state.

**(b) What will the system do on a request by P0 for one unit of R1?** Request = (0 1 0). It is ≤ Need (3 1 0) and ≤ Available (2 2 0). Pretend: Available = (2 1 0), P0 Allocation = (1 1 2), P0 Need = (3 0 0). Check: P0 (3 0 0) ✗, P1 (1 2 0) ✗ (needs 2 of R1, only 1 free), P2 (0 2 1) ✗. The state is **unsafe**, so the system **will not grant the request; P0 has to wait**.

---

## 7.6 Deadlock Detection

The system is **allowed to enter a deadlock state**; then a **detection algorithm** finds it and a **recovery scheme** fixes it.

### 7.6.1 Single instance of each resource type — wait-for graph
- Maintain a **wait-for graph**:
  - **Nodes are processes.**
  - **Pi → Pj** if Pi is waiting for Pj.
- **Periodically run an algorithm that searches for a cycle** in the graph. If there is a cycle, **there is a deadlock**.
- A cycle-detection algorithm needs about **n² operations**, where n is the number of vertices.
- *(The slide shows a resource-allocation graph and its corresponding wait-for graph: the resource nodes are removed and only the "who waits for whom" arrows between processes remain.)*

### 7.6.2 Several instances of a resource type
Data structures:
- **Available** — vector of length m: number of available resources of each type.
- **Allocation** — **n × m** matrix: resources of each type currently allocated to each process.
- **Request** — **n × m** matrix: the **current request** of each process. If `Request[i][j] = k`, process Pi is requesting **k more instances** of Rj.

**Detection algorithm**
1. Let **Work** and **Finish** be vectors of length m and n. Initialize:
   - (a) `Work = Available`
   - (b) For i = 1, 2, …, n: if `Allocation_i ≠ 0` then `Finish[i] = false`; otherwise `Finish[i] = true`.
2. Find an index i such that both: (a) `Finish[i] == false` and (b) `Request_i ≤ Work`. If no such i exists, go to step 4.
3. `Work = Work + Allocation_i`; `Finish[i] = true`; go to step 2.
4. If `Finish[i] == false` for some i (1 ≤ i ≤ n), the system is in a **deadlock state**. Moreover, if `Finish[i] == false`, then **Pi is deadlocked**.

The algorithm needs about **O(m × n²)** operations to detect whether the system is deadlocked.

*Easy reading:* it is like the safety algorithm, but it uses what the processes are **actually requesting now** (Request) instead of their maximum possible need. A process holding nothing cannot be part of a deadlock, so it starts as finished.

### 7.6.3 Example of the detection algorithm
5 processes P0–P4; 3 resource types **A (7), B (2), C (6)**. Snapshot at T0:

| | Allocation (A B C) | Request (A B C) | Available (A B C) |
| --- | --- | --- | --- |
| P0 | 0 1 0 | 0 0 0 | **0 0 0** |
| P1 | 2 0 0 | 2 0 2 | |
| P2 | 3 0 3 | 0 0 0 | |
| P3 | 2 1 1 | 1 0 0 | |
| P4 | 0 0 2 | 0 0 2 | |

Work = (0 0 0): P0 (0 0 0) ✓ → (0 1 0); P2 (0 0 0) ✓ → (3 1 3); P3 (1 0 0) ✓ → (5 2 4); P1 (2 0 2) ✓ → (7 2 4); P4 (0 0 2) ✓ → (7 2 6). The sequence **<P0, P2, P3, P1, P4>** gives `Finish[i] = true` for all i → **no deadlock**.

**Now P2 requests one more instance of type C.** Request matrix: P0 (0 0 0), P1 (2 0 2), P2 **(0 0 1)**, P3 (1 0 0), P4 (0 0 2).
- State of the system? We can **take back the resources held by P0**, but there are **not enough resources to satisfy the requests of the other processes**.
- **A deadlock exists, consisting of P1, P2, P3 and P4.**

### 7.6.4 Detection-algorithm usage
When and how often to run it depends on:
- **How often a deadlock is likely to occur.**
- **How many processes will need to be rolled back** — one for each disjoint cycle.

If the detection algorithm is run **at arbitrary times**, there may be many cycles in the resource graph, and we **cannot tell which of the many deadlocked processes "caused" the deadlock**.

### 7.6.5 Question: deadlock detection (solve) — slide
5 resource types; Request matrix Q, Allocation matrix A:

| | Q (R1 R2 R3 R4 R5) | A (R1 R2 R3 R4 R5) |
| --- | --- | --- |
| P1 | 0 1 0 0 1 | 1 0 1 1 0 |
| P2 | 0 0 1 0 1 | 1 1 0 0 0 |
| P3 | 0 0 0 0 1 | 0 0 0 1 0 |
| P4 | 1 0 1 0 1 | 0 0 0 0 0 |

Resource vector = (2 1 1 2 1). The slide's last vector (0 0 0 0 1) is the **free resources** (total minus all allocated).

**Solution:** Work = (0 0 0 0 1). P4 holds nothing, so `Finish[P4] = true` at the start. P3's request (0 0 0 0 1) ≤ Work ✓ → P3 finishes and returns (0 0 0 1 0) → Work = (0 0 0 1 1). P1 needs (0 1 0 0 1): R2 is not free ✗. P2 needs (0 0 1 0 1): R3 is not free ✗. So `Finish[P1] = Finish[P2] = false` → **P1 and P2 are deadlocked.**

---

## 7.7 Recovery from Deadlock

### 7.7.1 Process termination
- **Abort all deadlocked processes**, or
- **Abort one process at a time** until the deadlock cycle is removed.
- **In which order should we choose processes to abort?**
  - **Priority** of the process
  - **How long the process has computed**, and how much longer to completion
  - **Resources the process has used**
  - **Resources the process needs** to complete
  - **How many processes will need to be terminated**
  - Is the process **interactive or batch**?

### 7.7.2 Resource preemption
- **Selecting a victim** — choose so that the **cost is minimum**.
- **Rollback** — return to some **safe state** and restart the process from that state.
- **Starvation** — the same process may always be picked as the victim, so include the **number of rollbacks in the cost factor**.

---

## 7.8 Advantages and Disadvantages of the Approaches (slide table)

| Approach | Resource-allocation policy | Different schemes | Major advantages | Major disadvantages |
| --- | --- | --- | --- | --- |
| **Prevention** | Conservative; **undercommits resources** | **Requesting all resources at once** | Works well for processes that do a single burst of activity; no preemption necessary | Inefficient; delays process initiation; future resource requirements must be known by processes |
| | | **Preemption** | Convenient when applied to resources whose state can be saved and restored easily | Preempts more often than necessary |
| | | **Resource ordering** | Feasible to enforce via compile-time checks; needs no run-time computation since the problem is solved in system design | Disallows incremental resource requests |
| **Avoidance** | **Midway** between detection and prevention | Manipulate to **find at least one safe path** | No preemption necessary | Future resource requirements must be known by the OS; processes can be blocked for long periods |
| **Detection** | **Very liberal**; requested resources are granted where possible | **Invoke periodically** to test for deadlock | Never delays process initiation; facilitates online handling | Inherent preemption losses |

---
---

# WEEK 8 — MEMORY MANAGEMENT

## 8.1 Background

### 8.1.1 Basics
- Every instruction must be **fetched from memory** before it can run, and most instructions also **read data from memory or store data in memory** (or both).
- **Multitasking** makes memory management harder, because processes are **swapped in and out of the CPU** at high speed without disturbing other processes.
- **Shared memory, virtual memory, read-only vs read-write memory, and copy-on-write forking** make it even more complex.
- The **CPU can access only its registers and main memory.** It cannot directly use the hard drive, so data on the disk must **first be moved to main memory** before the CPU can work with it.
- **Register access** takes **one CPU clock (or less)**.
- **Main memory** can take **many cycles**, causing a **stall**.
- **Cache** sits between main memory and the CPU registers.
- **Protection of memory** is required for correct operation.

### 8.1.2 Base and limit registers
- User processes must be **restricted to the memory locations that belong to them.**
- A pair of **base and limit registers** defines the **logical address space** of each process.
- **Every memory access** by a process is checked against these two registers; if a user process tries to access memory **outside the valid range**, a **fatal error** is generated.
- **Changing the base and limit registers is a privileged activity**, allowed only to the **OS kernel**.

**Hardware address protection (figure):** the CPU address is compared with `base` (address ≥ base?) and with `base + limit` (address < base + limit?). If both checks say **yes**, the access goes to memory; if either says **no**, there is a **trap to the operating system — addressing error**.

### 8.1.3 Address binding
- Programs on disk waiting to be brought into memory form an **input queue**.
  - Without support, a program must be loaded at address **0000**.
- It is inconvenient if the first user process always has physical address 0000.
- Addresses are written differently at different stages of a program's life:
  - **Source code** addresses are usually **symbolic**.
  - **Compiled code** addresses bind to **relocatable addresses** — e.g. "14 bytes from the beginning of this module".
  - The **linker or loader** binds relocatable addresses to **absolute addresses** — e.g. 74014.
  - **Each binding maps one address space to another.**

**Binding of instructions and data to memory can happen at three stages:**

| Stage | Meaning |
| --- | --- |
| **Compile time** | If it is known at compile time where the program will be in physical memory, the compiler generates **absolute code** with actual physical addresses. If the load address changes later, the program must be **recompiled**. (DOS .COM programs use compile-time binding.) |
| **Load time** | If the load location is not known at compile time, the compiler generates **relocatable code** (addresses relative to the start of the program). If the starting address changes, the program must be **reloaded but not recompiled**. |
| **Execution time** | If the program can be **moved in memory while it runs**, binding is **delayed until execution time**. This needs **special hardware** and is the method used by **most modern OSs**. |

**Multistep processing of a user program (figure):** source program → compiler/assembler → object module → linker (with other object modules and system libraries) → load module → loader → program in memory (with dynamically loaded system library, dynamic linking). Binding can happen at compile time, load time or execution time.

### 8.1.4 Logical, relative and physical addresses
- **Logical address** — a reference to a memory location **independent of the current assignment of data to memory**.
- **Relative address** — an address given as a location **relative to some known point**.
- **Physical (absolute) address** — the **actual location in main memory**.

### 8.1.5 Memory-Management Unit (MMU) and dynamic relocation
- The **MMU** is a hardware device that, **at run time, maps virtual (logical) addresses to physical addresses**.
- Simple scheme: the value in the **relocation register** is **added to every address** generated by a user process when it is sent to memory.
  - The **base register is now called the relocation register.**
  - MS-DOS on Intel 80x86 used **4 relocation registers**.
- The user program deals with **logical addresses**; it **never sees the real physical addresses**.
- **Execution-time binding** happens when a reference is made to a memory location: the logical address is bound to a physical address.

*Example:* if the relocation register holds 14000 and the program generates logical address 346, the memory unit gets 14000 + 346 = **14346**.

### 8.1.6 Dynamic loading
- **Dynamic loading loads each routine only when it is called.**
- **Unused routines are never loaded.**
- This **reduces total memory usage** and gives **faster program start-up**.
- Downside: extra **complexity and overhead** — each call must check whether the routine is already loaded, and load it if not.

### 8.1.7 Dynamic linking
- **Static linking** — system libraries and program code are combined by the loader into the binary program image.
- **Dynamic linking** — linking is **postponed until execution time**.
- A small piece of code, the **stub**, is used to **locate the right memory-resident library routine**.
- The stub **replaces itself with the address of the routine** and runs the routine.
- The OS checks whether the routine is in the process's memory; if not, it is **added to the address space**.
- Dynamic linking is especially useful for **libraries**; the system is also known as **shared libraries**.
- It is useful for **patching system libraries**; **versioning may be needed**.

---

## 8.2 Swapping

- A process can be **swapped temporarily out of memory to a backing store**, and later **brought back** into memory to continue.
  - The **total physical memory space of processes can exceed physical memory.**
- **Backing store** — a **fast disk**, large enough to hold copies of all memory images for all users; it must give **direct access** to these images.
- **Roll out, roll in** — a swapping variant used for **priority-based scheduling**: a **lower-priority process is swapped out** so a **higher-priority process** can be loaded and run.
- **Most of the swap time is transfer time**, and the total transfer time is **directly proportional to the amount of memory swapped**.
- The system keeps a **ready queue** of ready-to-run processes whose memory images are on disk.
- **Does a swapped-out process need to come back to the same physical addresses?** It **depends on the address-binding method**. Also consider **pending I/O** to or from the process's memory space.
- **Modified versions of swapping** are found on many systems (UNIX, Linux, Windows):
  - Swapping is **normally disabled**.
  - It starts if **more than a threshold amount of memory is allocated**.
  - It is **disabled again** once memory demand falls below the threshold.

---

## 8.3 Contiguous Memory Allocation (Memory Management Techniques)

### 8.3.1 Fixed partitioning
- **Equal-size partitions:** any process whose size is **less than or equal to the partition size** can be loaded into an available partition.
- The OS can **swap out** a process if all partitions are full and no process is in the Ready or Running state.
- A program too big for a partition must be designed using **overlays**.

**Disadvantages**
- **Main memory is used inefficiently** — any program, however small, occupies an **entire partition**.
- The **number of partitions** fixed at system-generation time **limits the number of active processes**.
- **Internal fragmentation** — wasted space because the block of data loaded is **smaller than the partition**.

**Unequal-size partitions** help reduce these problems:
- Programs up to **16M** can be accommodated **without overlays**.
- Partitions **smaller than 8M** allow small programs to fit with **less internal fragmentation**.

*(The slide figure "Memory assignment for fixed partitioning" shows two ways: (a) **one process queue per partition**, (b) a **single queue** for all partitions.)*

### 8.3.2 Dynamic partitioning
- Partitions are of **variable length and number**.
- A process is allocated **exactly as much memory as it needs**.
- Used by IBM's mainframe OS, **OS/MVT**.

**Disadvantage — external fragmentation:** memory becomes more and more fragmented and **memory utilization declines**.
- **Compaction** — the technique to overcome external fragmentation: the OS **shifts processes so they are contiguous** and all free memory is together in **one block**.
- Compaction is **time consuming and wastes CPU time**.

### 8.3.3 Placement algorithms
- **Best-fit** — chooses the block **closest in size** to the request.
- **First-fit** — scans memory **from the beginning** and chooses the **first available block that is large enough**.
- **Next-fit** — scans from the **location of the last placement** and chooses the next available block that is large enough.
- **Worst-fit** — allocates the **largest block**; must also search the entire list; **produces the largest leftover hole**.

**Question (slide):** Five memory partitions of **100 KB, 500 KB, 200 KB, 300 KB, 600 KB** (in order). How do first-fit, best-fit and worst-fit place processes of **212 KB, 417 KB, 112 KB, 426 KB** (in order)? Which makes the most efficient use of memory?

| Algorithm | 212 KB | 417 KB | 112 KB | 426 KB |
| --- | --- | --- | --- | --- |
| **First-fit** | 500K partition | 600K partition | 288K partition (leftover of 500K − 212K) | **Must wait** |
| **Best-fit** | 300K partition | 500K partition | 200K partition | 600K partition |
| **Worst-fit** | 600K partition | 500K partition | 388K partition | **Must wait** |

**Answer:** **Best-fit** is the most efficient here — it is the only one that places all four processes.

### 8.3.4 Buddy system
- It combines **fixed and dynamic partitioning** schemes.
- The space available for allocation is treated as **a single block**.
- Memory blocks are available in sizes of **2^K words**, where **L ≤ K ≤ U**:
  - **2^L** = smallest block size that is allocated,
  - **2^U** = largest block size that is allocated (generally the size of the whole memory available for allocation).

**Example of buddy system (slide figure) — a 1 MB block:**

| Event | Memory after the event |
| --- | --- |
| Start | 1M (one free block) |
| Request 100K (A) | A = 128K, 128K free, 256K free, 512K free |
| Request 240K (B) | A = 128K, 128K free, B = 256K, 512K free |
| Request 64K (C) | A = 128K, C = 64K, 64K free, B = 256K, 512K free |
| Request 256K (D) | A = 128K, C = 64K, 64K free, B = 256K, D = 256K, 256K free |
| Release B | B's 256K becomes free |
| Release A | A's 128K becomes free |
| Request 75K (E) | E = 128K (uses the free 128K block), C = 64K, 64K free, 256K free, D = 256K, 256K free |
| Release C | C and its free 64K buddy join into a 128K free block |
| Release E | Free blocks join → a 512K free block, D = 256K, 256K free |
| Release D | Everything joins back into one **1M** block |

*(The slide also shows the **tree representation** of the buddy system: the 1M block splits into 512K blocks, then 256K, 128K and 64K. A leaf is either an allocated block or an unallocated block; the other nodes are split (non-leaf) nodes.)*

---

## 8.4 Paging

### 8.4.1 Concept
- The **physical address space of a process can be non-contiguous**; the process gets physical memory **whenever it is available**.
  - This **avoids external fragmentation**.
  - It **avoids the problem of varying-sized memory chunks**.
- **Physical memory** is divided into **equal fixed-size blocks** that are relatively small — called **frames** (the available blocks of memory).
- The **process is also divided** into small fixed-size blocks of the **same size** — called **pages** (the blocks of a process).
- The system **keeps track of all free frames**.
- To run a program of **N pages**, find **N free frames** and load the program.
- There is **still internal fragmentation**.

### 8.4.2 Internal fragmentation (calculation from the slide)
- Page size = **2,048 bytes**; process size = **72,766 bytes**.
- 72,766 = **35 pages + 1,086 bytes** → the process needs 36 pages.
- Internal fragmentation = 2,048 − 1,086 = **962 bytes**.
- **Worst case** fragmentation = **1 frame − 1 byte**.
- **On average** fragmentation = **1/2 frame size**.
- So are small frame sizes better? **But each page-table entry takes memory to track**, and **page sizes have been growing over time**.

### 8.4.3 Address translation scheme
The address generated by the CPU is divided into two parts:
- **Page number (p)** — used as an **index into the page table**, which holds the **base address of each page in physical memory**.
- **Page offset (d)** — combined with the base address to give the **physical memory address** sent to the memory unit.

For a logical address space of **2^m** and a page size of **2^n**: the **higher m − n bits** are the page number p and the **lower n bits** are the offset d.

| page number (p) | page offset (d) |
| --- | --- |
| m − n bits | n bits |

### 8.4.4 Paging hardware and model
**Paging hardware (figure):** the CPU produces a logical address (p, d). **p** indexes the **page table** to get the **frame number f**. The physical address is **(f, d)**, i.e. frame f followed by the same offset d, and it goes to physical memory.

**Paging model of logical and physical memory (figure):** the pages 0, 1, 2, 3 of logical memory are placed in **any free frames** of physical memory, and the page table records which frame holds each page.

### 8.4.5 Paging example
**n = 2 and m = 4; 32-byte memory and 4-byte pages.**
- Logical memory has 16 bytes (a to p) = 4 pages. Page table: page 0 → frame 5, page 1 → frame 6, page 2 → frame 1, page 3 → frame 2.
- Logical address 0 (`a`): page 0, offset 0 → frame 5 → physical address 5 × 4 + 0 = **20**.
- Logical address 3 (`d`): page 0, offset 3 → 5 × 4 + 3 = **23**.
- Logical address 4 (`e`): page 1, offset 0 → frame 6 → 6 × 4 + 0 = **24**.
- Logical address 13 (`n`): page 3, offset 1 → frame 2 → 2 × 4 + 1 = **9**.

### 8.4.6 Free frames
The slide shows the **free-frame list before allocation and after allocation**: when a new process arrives, the OS takes as many frames from the free-frame list as the process has pages, loads the pages into them, and writes the frame numbers into the process's page table. Those frames are then no longer free.

---

## 8.5 Structure of Page Table

### 8.5.1 Page table
- **Maintained by the OS for each process.**
- It **contains the frame location for each page** of the process (it **translates logical to physical addresses**).
- The **processor must know how to access the page table** of the current process.
- The processor uses it to **produce a physical address**.

**Question (GATE 2015, slide):** byte-addressable memory, **32-bit logical addresses**, **4 KB page size**, **page table entries of 4 bytes**. Size of the page table in MB?
- Number of pages = 2^32 / 2^12 = **2^20** entries.
- Page table size = 2^20 × 4 bytes = 2^22 bytes = **4 MB**.

### 8.5.2 Implementation of page table
- The page table is **kept in main memory**.
- **Page-table base register (PTBR)** — **points to the page table**.
- **Page-table length register (PTLR)** — indicates the **size of the page table**.
- In this scheme **every data/instruction access needs two memory accesses**: one for the page table and one for the data/instruction.
- This **two-memory-access problem** is solved by a special **fast-lookup hardware cache** called **associative memory** or **translation look-aside buffer (TLB)**.

**Associative memory** — **parallel search**. For address translation (p, d):
- If **p is in an associative register**, get the frame number directly — **TLB hit**.
- Otherwise get the frame number **from the page table in memory** — **TLB miss**.

*(Figure "Paging hardware with TLB": the page number is first looked up in the TLB; on a hit the frame number comes straight from it; on a miss it is read from the page table in memory.)*

### 8.5.3 Effective memory access time (EMAT)
- Associative lookup = **ε** time units (can be **< 10%** of the memory access time).
- **Hit ratio = α** — the percentage of times a page number is found in the associative registers; it is related to the number of associative registers.
- **EMAT = TLB hit × (TLB access time + memory access time) + TLB miss × (TLB access time + page table access time + memory access time)**

**Question (GATE 2014, slide):** TLB search takes **10 ms**, physical memory access takes **80 ms**, TLB hit ratio is **0.6**. Find the EMAT.
- Hit: 10 + 80 = 90 ms. Miss: 10 + 80 (page table) + 80 (data) = 170 ms.
- EMAT = 0.6 × 90 + 0.4 × 170 = 54 + 68 = **122 ms** → option **(B)**.

### 8.5.4 Valid (v) / invalid (i) bit in a page table
- Each page-table entry has a **valid–invalid bit** next to the frame number.
- **v** → the page is in the process's logical address space (a legal page).
- **i** → the page is **not** in the process's logical address space.
- *(Slide figure: pages 0–5 have frames 2, 3, 4, 7, 8, 9 and are marked **v**; the entries for pages 6 and 7 are marked **i**.)*

### 8.5.5 Shared pages
- **Shared code**
  - **One copy of read-only (reentrant) code** is shared among processes (e.g. text editors, compilers, window systems).
  - Similar to **multiple threads sharing the same process space**.
  - Also useful for **inter-process communication** if sharing of **read-write pages** is allowed.
- **Private code and data**
  - Each process keeps a **separate copy** of its code and data.
  - The pages for private code and data can appear **anywhere in the logical address space**.
- *(Slide figure "Shared pages example": the page tables of different processes point to the **same frames** for the shared code, and to different frames for each process's private data.)*

---

## 8.6 Types of Paging

### 8.6.1 Hierarchical page tables
- **Break up the logical address space into multiple page tables.**
- A simple technique is a **two-level page table** — **"page the page table"**.
- *(Figure: **two-level page-table scheme** — an **outer page table** points to pages of the page table, and those point to the actual frames in memory.)*

**Question (GATE 2013, slide):** 46-bit virtual address, 32-bit physical address, **three-level** page table. The page-table base register holds the base address of the first-level table **T1**, which occupies **exactly one page**. Each entry of T1 points to a page of **T2**, each entry of T2 points to a page of **T3**, and each entry of T3 is a PTE of **32 bits**. What is the **page size in KB**?

**Solution (as in the slide):** let the page size be **x**.
- Number of pages = 2^46 / x → T3 has that many entries; each entry is 4 bytes, so total T3 size = 2^48 / x bytes.
- Number of T3 pages = 2^48 / x² → T2 needs that many entries; total T2 size = 2^50 / x² bytes.
- Number of T2 pages = 2^50 / x³ → T1 needs that many entries; T1 size = 2^52 / x³ bytes.
- T1 occupies exactly one page, so 2^52 / x³ = x → x⁴ = 2^52 → x = 2^13 bytes = **8 KB**.

### 8.6.2 Hashed page tables
- Common in address spaces **larger than 32 bits**.
- The **virtual page number is hashed** into a page table. Each hash-table location holds a **chain of elements** that hash to the same place.
- Each element contains: **(1) the virtual page number, (2) the value of the mapped page frame, (3) a pointer to the next element**.
- Virtual page numbers are **compared along the chain** to find a match; if found, the **corresponding physical frame is taken**.
- **Variation for 64-bit addresses — clustered page tables:** similar to hashed, but **each entry refers to several pages (such as 16) instead of 1**. Especially useful for **sparse address spaces** (memory references that are non-contiguous and scattered).

### 8.6.3 Inverted page table
- Instead of each process having a page table that tracks all its possible logical pages, **track all physical pages**.
- There is **one entry for each real page (frame) of memory**.
- Each entry holds the **virtual address of the page stored in that real memory location**, with information about the **process that owns the page**.
- It **reduces the memory needed to store page tables**, but **increases the time needed to search the table** on a page reference.
- A **hash table** is used to limit the search to **one or at most a few** page-table entries; the **TLB can speed up access**.
- **How to implement shared memory?** With an inverted table there is **only one mapping** of a virtual address to the shared physical address.
- *(Figure "Inverted page table architecture": the CPU's logical address has (pid, p, d); the table is searched for (pid, p); the index i of the matching entry is the frame number, giving the physical address (i, d).)*

---

*End of notes.*