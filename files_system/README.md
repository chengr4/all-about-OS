# File System

## Open file Attributes

- File types
  - .exe, .com, .obj, .cc
  - Hint for OS to operate file in a resonable way

## Access Methods

### Sequential access

- Continuously
- faster than random access
- read/write next block + rewind/skip + reset

### Direct access

> aka. random access

- Advanced => Index Access

## Directory Structure

- Partition: no file system, e.g. database, UNIX swap space
- Volume: Formatted partition with file system
- Directory: Tree 

### Acyclic-Graph Directory

- symbolic link (`ln -s`): a file that points to another file
- A file can have multiple absolute paths
- How to delete a file? reference count = 0

### General-Graph Directory

- **May contain cycles**
- Use **Garbage Collection** to resolve cycles
  - First pass traverses the entire graph and marks accessible files or dir
  - Second pass collect and free everything that is unmarked

## File System Mounting

A file system must be mounted before it can be accessed.

- Mount timing
  - Boot time
  - automatically at runtime
  - manually at runtime (early)
- OS will maintain a mount table

> `mount -t`

## File Sharing on Multiusers

- Each user has a unique user ID and group ID
- Each file has owner, group and others
- Acess Control List (ACL)

## File Protection

- physical damage => RAID
- improper access => password

---

## File System Structure

- I/O transfers between memory and disk are performed in units of blocks (one or more sectors, one sactor is usually 512 bytes)
- One OS can supprot multiple file systems (NTFS, FAT32)

