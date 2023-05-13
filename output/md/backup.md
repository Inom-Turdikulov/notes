---
date: 2023-03-05
draft: true
sr-due: 2023-08-10
sr-ease: 230
sr-interval: 1
tags:
- defenition
- inbox
---

# Backup

Copy of some data. This copy precious if when the original data is lost or
damaged (changed).

I lose some data in my life and some of it was important.

Additionally, you can use backup to migrate data, do data versioning, and it
will be your disaster recovery plan.

I use [borg](./borg.md) and [btrfs](./btrfs.md), with
[my disaster recovery plan](./my%20backup%20plan.md).

Borg provide solution for incremental/full backup, encryption, compression, and
de-duplication. It's also having data validation and integrity check.

Btrfs can be used to snapshot the whole system, and it's also having data
validation and integrity check.

I'm also trying to follow 3-2-1 backup rule. It's means having at least three
copies of your data, two local (on-site) but on different media (read: devices),
I use 2 hard disk drives and 2 solid-state drive (RAID-1), and at least one copy
off-site (I use encrypted `borg backup`).