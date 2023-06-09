---
date: 2023-04-14
draft: true
tags:
- inbox
- definition
- CS-tip
sr-due: 2023-05-20
sr-interval: 3
sr-ease: 266
---

# Set (abstract data type)

> Abstract data type that can store unique values, without any particular order.
> It is a computer implementation of the mathematical concept of a finite set.
> Unlike most other collection types, rather than retrieving a specific element
> from a set, one typically tests a value for membership in a set. --
> [Wikipedia](<https://en.wikipedia.org/wiki/Set_(abstract_data_type)>)

So main set feature is that it can store ==only unique values==.

Set seems so similar (especially array-based set) to the
[[array (computer science)|array]] but operations performed on the set are
different, mainly on **insert operation**. It has different efficiency, because
we have non-duplicating constraint. But it perfectly replaces array, when you
need unique data.

Sets can be suitable for any lists of unique data (phone numbers, email
addresses, etc.).

Reading from a set take ==one step==, like array.

Searching a set takes up to ==$N$ steps, where $N$ is a number of items in the
set==, like array.

Deletion from set takes ==$N$ steps, delete and move data to the left to close
gap==, like array.

**Insertion** is different. You need to ensure that you don't have duplicate
data and this means every insertion into a set
==first requires a search operation==.

In best case insertion into set takes:
?
Insert into end of set. $N + 1$ steps. $N$ steps → search, 1 step to insert into
end.

In worst case insertion into set takes:
?
Insert into beginning of set is worst case scenario. In contrast to insertion
into the begging of a regular array ($N+1), insertion can take $2N + 1$ steps.
Formula: (search $N$ steps) + (shift $N$ steps) + (insert 1 step). In other
words we add search operation to insert value into set.
