---
date: 2023-03-18
draft: true
sr-due: 2023-03-16
sr-ease: 250
sr-interval: 3
tags:
- inbox
- definition
---

# Control flow

Remember, you start loop from 0 and check condition by ==N== if you use `<`
[boolean expression](./boolean%20expression.md). So it's canonical to write some like this:

```c
int i = 0;
int N = 10; // easly readable bounday condition

while (i < N) {  // we use <, not <= to execute N times instead of N+1
                 // and it's easy imagine like I need iterate N times
    // do something
    i++;
}
```