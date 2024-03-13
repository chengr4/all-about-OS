# Scheduler

- Short-term scheduler: selects which process should be executed next and allocates CPU to it. (Ready state => Run state)
- Long-term scheduler: selects which processes should be **loaded into memory** and brought into the ready queue. (New state => Ready state)
- Medium-term scheduler: selects which processes should be **swapped in and out** of memory. (Ready state => Wait state)

Scheduling Criteria:

- CPU utilization: keep the CPU as busy as possible
- Throughput: number of processes that are completed per time unit
- Turnaround time: amount of time to execute a particular process (from submission to completion)
- Waiting time: amount of time a process has been waiting in the ready queue
- Response time: amount of time it takes from when a request was submitted until the first response is produced (first CPU burst cycle)

## Scheduling Algorithms

- First-Come, First-Served (FCFS)
- Shortest-Job-First (SJF)
- Priority Scheduling
- Round Robin (RR)
- Multilevel Queue Scheduling
- Multilevel Feedback Queue Scheduling