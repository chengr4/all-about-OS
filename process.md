# Process

- 對作業系統來說， process 是資源分配的最小單位，並且同時是個「操作單位
- IPC (InterProcess Communication): send data between a process and a process

## Process Creation

- Two possibilities of execution: concurrent or parent wait for child to finish.

In Unix/Linux:

- `fork` system call: create a new process, with **duplicate address spcace**, **concurrent**
- `execlp` system call: Load a new binary file into memory - destroying the old code
- `wait` system call: actively lets parent wait for child to finish

## Thread

> aka. lightweight process

- All threads belonging to the same process share (Global variable): 
    1. code section
    2. data section
    3. OS resources (eg open files and signals)
- Each thread has its own thread control block: thread ID, program counter, register set, and a stack

### User vs. Kernel Threads

- many-to-one, one-to-one (common), many-to-many

| User Thread | Kernel Thread |
| --- | --- |
| Thread library provides | kernel performs |
| POSIX Pthreads, Win32 threads, Java threads | Window 2000 (NT), solaris, Linux, Tru Unix |
| fast to create | slower |

### Thread Pools

- Create a number of threads in a pool where they await work
- pros: faster, size of pool can be bounded