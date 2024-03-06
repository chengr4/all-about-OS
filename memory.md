# Memory

- fixed partition and variable partition
- We create virual memory to enhance the utilization rate of physical memory
- Demand paging: A page rather than the entire process is brought into meomory only when it isi needed

## Page Table

- Page table is kept in memory
- Contains protection bit (E.g. read, write, execute, valid-invalid bit)
- Can share pure code's pages among processes

## Translation Lookaside Buffer (TLB)

- Target: resolve 2 memory reads (one for the page table, one for the physical memory)
- cache for page table
- stored in MMU (hardware)
- associative memory => parallel search
- TLB must be flushed after a context switch

## Segmentation

> variable-size partitioning

- Has a segmentation table

## Page Replacement

> Conditions: no free frame

1. frame-allocation algorithm: Determines how many frames to allocate to a process
2. page-replacement algorithm: Determines which page to replace
    - FIFO
    - Optimal (Belday) Algorithm (need future knowledge)
    - LRU (Least Recently Used, looking backward)

## Frame

- Each process needs min number of frames

## References

- [What Every Programmer Should Know About Memory](https://sysprog21.github.io/cpumemory-zhtw/)
