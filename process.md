# Process

## Process Creation

- Two possibilities of execution: concurrent or parent wait for child to finish.

In Unix/Linux:

- `fork` system call: create a new process, with **duplicate address spcace**, **concurrent**
- `execlp` system call: Load a new binary file into memory - destroying the old code
- `wait` system call: actively lets parent wait for child to finish

