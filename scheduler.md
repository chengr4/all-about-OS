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
- Round Robin (RR): 輪流分配 CPU 時間
- Multilevel Queue Scheduling: evey queue can have its own scheduling algorithm
- Multilevel Feedback Queue Scheduling

如何評估 scheduling algorithm?

1. 定義一個 metric (wait time, response time, turnaround time, throughput, CPU utilization) ...
2. Deterministic modeling: 模擬提供的 scheduling algorithm
3. Queuing models: 用數學模型來模擬 (Queuing theory)
4. 真實模擬
5. 實作: 與真實情況調整