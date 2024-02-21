# Memory

## Page Table

- Page table is kept in memory

## Translation Lookaside Buffer (TLB)

- Target: resolve 2 memory reads (one for the page table, one for the physical memory)
- cache for page table
- stored in MMU (hardware)
- associative memory => parallel search
- TLB must be flushed after a context switch

## References

- [What Every Programmer Should Know About Memory](https://sysprog21.github.io/cpumemory-zhtw/)
