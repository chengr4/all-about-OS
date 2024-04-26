# Disk Management

- IDE disk, SCSI disk

## Disk Formatting

Not only file system do formatting but also disk (low-level formatting).

- Divide disks into sectors that disk controller can read and write

## Boot Block

- Bootstrap prgram: init CPU, registers, device controllers, memory

## Bad Blocks

## Swap-Space Management

Two ways to manage:

1. part of a normal file system (e.g. NT)
2. Separate disk partition (raw partition)

## RAID

Redundant Array of Independent Disks

- provide reliability via redundancy
- improve performance via parallelism

- Striping: data is interleaved across multiple disks
- Mirror (Replication): data is duplicated on two disks
- ECC (Error-Correcting Code): parity bits are stored with data