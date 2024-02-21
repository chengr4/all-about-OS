# All About OS

- [I/O](#io)

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

## I/O

### Zero-copy 

In Linux, There are two ways to implement zero-copy: `mmap + write` and `sendfile`

> `mmap` returns addresses instead of copy data from kernal memory

- by Java: `Java NIO - transferTo()`

## References

- [事件驅動伺服器：原理和實例](https://hackmd.io/@sysprog/event-driven-server)
- https://github.com/cccriscv/mini-riscv-os
- [Understanding the bin, sbin, usr/bin, usr/sbin split](http://lists.busybox.net/pipermail/busybox/2010-December/074114.html)
