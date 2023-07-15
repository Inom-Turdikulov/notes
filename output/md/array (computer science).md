---
date: 2022-12-29
draft: true
sr-due: 2023-11-09
sr-ease: 230
sr-interval: 176
tags:
- definition
- inbox
- CS-tip
---

# Array (computer science)

Array is one of most basic data structure in computer science.

## Array (data structure)

> Array is a [data structure](./data%20structure.md) consisting of a collection of elements (values
> or variables), each identified by at least one array index or key.
>
> -- [Wikipedia](<[https://en.wikipedia.org/wiki/Array_(data_structure)>)](https://en.wikipedia.org/wiki/Array_(data_structure)>))

> An assemblage of items that are randomly accessible by integers, the index.
>
> -- <[https://xlinux.nist.gov/dads/HTML/array.html>](https://xlinux.nist.gov/dads/HTML/array.html>)

Array in memory is a **contiguous** block of memory locations (which allocated
when you create it). Array usually at least has an **address** in memory and
**size** (number of items in array). Each element of array has an index
(location of elements or address), and first index is `0`.

size_of_array = ==last_index + 1==

| 0   | 1   | 2   | 3   | 4   | 5   |
| --- | --- | --- | --- | --- | --- |
|     |     | `9`   |     |     | `1`   |
|     | `5`   |     |     |     |     |
|     |     |     | `10`  |     |     |
|     |     |     |     | `6`   |     |
|     | `7`   |     |     | `11`  |     |
*Graphical representation of array in memory*\
How many total items in this array? Is empty items has address in memory?
?
6*5 = 30
yes, empty items has address in memory

## Array (data type)

> In [computer science](./computer%20science.md), **array** is a [data type](./data%20type.md) that represents a
> collection of _elements_ [values](./value%20%28computer%20science%29.md) or
> [variables](./variable%20%28computer%20science%29.md), each selected by one or more
> indices (identifying keys) that can be computed at
> [runtime](./runtime%20%28program%20lifecycle%20phase%29.md) during program execution. Such a
> collection is usually called an **array variable** or **array value**. By
> analogy with the mathematical concepts [vector](./vector.md) and
> [matrix](./matrix%20%28mathematics%29.md), array types with one and two indices are
> often called **vector type** and **matrix type**, respectively. More
> generally, a multidimensional array type can be called a **tensor type**, by
> analogy with the physical concept, [tensor](./tensor.md).
So in general array is a 1 way storing several items (such as integers). Usually
array store the same type of items (this depending on language). Every item in
array indexed (by integer number starting from 0) and you can access array item
by index (key in array). As rule index starting from [0](./zero-based%20numbering.md)
to `n-1` where `n` is a number of items in array.

In general array is ==list of data elements==.
Size of an array is ==how many data elements the array holds==.
<!--SR:!2023-07-15,2,230-->

The index of an array is the number that identifies ==where a piece of data
lives== inside the array.

In most programming languages, arrays are ==zero-indexed==, meaning that the
first element of the array is at index 0, the second element is at index 1, and
so on.

```mermaid
graph LR
    A[Array] --- |Index 0| B(1)
    A --- |Index 1| C(2)
    A --- |Index 2| D(3)
    A --- |Index 3| E(4)
```


When you create array ([initialization (programming)](./initialization%20%28programming%29.md)) you must set array size
(number of items stored in the array). Size of array is fixed. Also, computer
==allocate some [memory](./computer%20memory.md)== for array during its
initialization.


When allocating an array the computer always keeps track: ? Beginning address
and array size


An array is stored such that the **position of each element** can be computed
from its **index tuple** by a mathematical formula. So a computer can find the
value at any index by performing simple addition.

| value          | A   | B   | C   | D   | E   | F   | G   | H   | I   | J   |
| :------------- | :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| memory address | 10  | 11  | 12  | 13  | 14  | 15  | 16  | 17  | 18  | 19  |
| index          | 0   | 1   | 2   | 3   | 4   | 5   | 6   | 7   | 8   | 9   |

Read value at index 3:

1. Array begins from memory address 10
2. Index 3 will be exactly 3 positions after address 10
3. So, memory address for index 3 is 13
4. Read value from memory address 13 = D

Examples, how to use [array in programming languages](./array%20in%20programming%20languages.md).

Array operations explained in [array operations](./array%20operations.md).

## Ordered array

Ordered array is same as array, but with one difference: elements in ordered
array are ==sorted in some order== (usually ascending or descending), and when you
modify array, you must keep it sorted.

In worst case insertion in ordered array is ==$N+2$ steps==.