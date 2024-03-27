# Synchronization

- Peterson's Solution (for 2 processes)
- Critical Section 越小越好
- mutex, condition variable
- Hareware Support: 因為 Hardware 有提供 atomic operation (`TestAndSet(), Swap()`), 所以可以用來實作 synchronization

## Race condition

Race condition means the situation where several processes 

1. acess and manipulate **shared data** concurrently. The final value of the shared data 
2. depends upon which process **finishes last**.

## Algorithms

- Bakery algorithm (`N` processes)

## Condition Variables

Condition variables represent some **condition** that a thread can:
  1. Wait on, until the condition occurs
  2. Notify other waiting threads that the condition has occurred

- Can make thread pool

## Thread Pool

- Avoid creating and destroying threads frequently

## Semaphores

- A **tool** to generalize the synchronization problem
- A record of **how many units** of a paritcular resource are available
    - if #record = 1 => binary semaphore, mutex
    - if #record > 1 => counting semaphore
- Two atomic operations: `wait()` and `signal()`
- Implementation: Spinlock