---
title: FAT File System
subtitle: Today we will talk about the FAT file system
# Link this post with a project
projects: []

# Date published
date: '2022-05-25T00:00:00Z'

# Date updated
lastmod: '2022-05-25T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: []()'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - 5 week

categories:
  - post 5

---
A file system is a tool that allows the operating system and programs to access and work with the necessary files. In this case, the programs operate only with the name of the file, its size and the date of creation. All other functions for finding the necessary file in the storage and working with it are taken over by the file system of the drive







## **What is the file system?**



The abbreviated abbreviation "FAT" stands for "file allocation table". This is a simple classical file system architecture, originally designed for small disks and simple folder structures. In other words, the "FAT" file system is a group method of organization in which the file allocation table is allocated to a separate logical area and is located at the beginning of the volume. To avoid unintentional or accidental errors that may affect the correct display of the table, the system, for security purposes, stores a copy of the array of index pointers. The FAT file system is used by MS DOS and Windows OS to organize and manage files.



Developed by Bill Gates and Mark McDonald in 1976-1977. It was used as the main file system in the operating systems of the MS-DOS and Windows 9x families.





## **What are FAT file systems?**

There are several versions of the FAT file system, among which the FAT 16 and FAT 32 file systems have found the greatest use. The difference between these file systems is the bitness of the numbers used in the file placement tables.



However, I mention two more file systems: FAT12 and FAT64 or its other name exFAT. Next, we will analyze their differences.



## **FAT12 File System**



A file system widely used on flexible magnetic disks. It is the first popular file system on IBM PC -compatible computers.



The most recent storage device that used the FAT12 file system was a 3.5-inch diameter floppy disk with a capacity of 1.44 MB. There were also floppy disks with a size of 2.88, but they did not get much distribution.



The entire FAT12 file system space is divided into blocks that are multiples of the floppy disk sector size (512 bytes). When applied to floppy disks, the cluster size is usually chosen to be equal to one sector. Each non-empty file occupies at least 1 cluster. Therefore, if there are a lot of small files on the floppy disk, then a lot of space will be wasted. The maximum cluster size for the FAT12 file system is 8192 bytes.



Its advantages are that it takes up little disk space, requires little RAM to cache it. The disadvantage is that when used on partitions larger than 64 MB, the cluster size becomes the maximum, which leads to the inevitable loss of free disk space in the final cluster of each file.



## **FAT16 File System**



The FAT 16 file system is supported by MS DOS, Windows 95, Windows 98, Windows 2000, as well as some versions of UNIX OS.The number 16 in the file system name indicates the number of bits (binary bits) required

to store information about the cluster numbers used by a file, i.e. no more than 65536 entries can be placed in the file allocation table, the Operating system uses the File Allocation Table to search for a file and determine the clusters that this file occupies on the hard disk. In addition, information about free and defective clusters is recorded in the Table. To make it easier to comprehend the FAT16 file system, imagine

imagine the table of contents of the book and how you work with this table of contents, that's exactly how the operating system works with FAT 16.



The maximum size of partitions or disks in FAT16 is 4.2 gigabytes.



However, nowadays FAT 16 usage is inefficient. But it fully met the requirements of old computers.



Modern NVMDS have a memory capacity of several tens of gigabytes, so the use of the FAT16 file system is inefficient for them.



The second disadvantage is that the FAT system uses only 1 byte to store all file attributes. Therefore, it is simply not possible to store data about access rights to the file, its owner, etc.



## **FAT32 File System**



The FAT32 file system is an extended version of the FAT16 file system, support for which was first implemented in Windows 95B. The FAT32 file system is also supported by Windows 98, Windows 2000 and Windows XP.



The main difference between the FAT32 file system and FAT16 is that in the FAT file allocation table, you can place not 65,536 records about cluster numbers, but 268,435,445.



One of the main reasons for creating FAT32 was the need to use disk space more efficiently. In this file system, smaller clusters are used for drives whose capacity does not exceed 8 GB (the cluster size is 4 KB), which allows for 10-15% more efficient use of the drive's disk space compared to the drive in the FAT16 file system. In addition, the maximum size of the disk volume (partition) increases in the FAT32 file system.



## **FAT64 or exFAT file system**



"exFAT" is an abbreviation of the full English name "Extended File Allocation Table" ("extended file Allocation Table"). The standard is an updated version of the "FAT32" file system created by Microsoft Corporation.The exFAT system is extremely similar to FAT32. But the main difference is the elimination of restrictions present in the FAT32 file system, which allows users to store files much larger than four gigabytes.



Also, in the exFAT file system, the number of overwrites of sectors responsible for direct storage of information has been significantly reduced, which is especially important for flash drives, due to irreversible wear of cells after a certain number of write operations, and the mechanism for allocating free space has been improved.



## **Advantages and Disadvantages of the FAT file system**



Of course, the FAT file system is already outdated and is being used more and more in flash cards than in operating systems. However, it also has its advantages:

- The FAT file system works best for disks and/or partitions of about 200 MB, since FAT starts with very little overhead.

- Supported by most devices.



But there are also disadvantages of FAT:

- It is desirable that when using disks or partitions over 200 MB, the FAT file system should not be used. This is because as the volume size increases, performance with FAT decreases rapidly.

- Low stability with mild failures;

- "Lost Clusters“

- There are no access control mechanisms

- It is not possible to set permissions on files that are FAT partitions.















