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



## References

- [What Every Programmer Should Know About Memory](https://sysprog21.github.io/cpumemory-zhtw/)
