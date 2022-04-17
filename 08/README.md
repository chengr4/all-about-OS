## Scheduler

- (頻繁) Short-term scheduler (CPU scheduler) => ready (memory) to run (CPU)
- Long-term scheduler (job scheduler) => new (disk) to ready (memory)
- Medium-term scheduler => ready to wait

### Long-Term scheduler

- Control **degree of multiprogramming** (the number of processes in memory) => should not be to high (crazy swapping) and to low (CPU idle)
- UNIX/NT: no long term scheduler (because current computers usually have enough memory)

### Short-Term scheduler

- Execute quite frequently (e.g. once per 100ms)
- Must be efficient:
  - if 10 ms for picking a job (run algo.), 100 ms for such a pick => overhead (冗余) = 10/110 = 9%

### Medium-Term scheduler

Purpose:

- Improve process mix = improve CPU and I/O
- free up memory

Most mordern OS combine medium-term scheduler with virtual memory