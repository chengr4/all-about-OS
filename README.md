# All About OS

## Technical Terms

| Term | Description |
| ---- | ----------- |
| Batch | 批次，one time a job |
| idle |  閒置 |
| volatile | 斷電即遺失 |
| userprog | user program |
| overhead | 浪費 |
| cascading | 瀑布般的 |

## Important concepts

- Two Interrupt types: System call (software trigger), Signal (Hareware trigger)

## Memory
- Memory related: [Prof. Jerry Chou 04](./10510prof-jerry-chou-OS/04/README.md)
- https://sysprog21.github.io/cpumemory-zhtw/

## Thread vs Process

- 對作業系統來說， process 是資源分配的最小單位，並且同時是個「操作單位」

| Thread | Process |
| ------ | ------- |

### Thread

> lightweight process

- All threads belonging to the same process share 1. code section, 2. data section, 3. OS resources (eg open files and signals)

> == Global variable

## Topics to Read

1. [Understanding the bin, sbin, usr/bin , usr/sbin split](http://lists.busybox.net/pipermail/busybox/2010-December/074114.html)
