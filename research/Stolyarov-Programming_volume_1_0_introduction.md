---
author:
  - Андрей Викторович Столяров
date: 2021
external:
  - http://www.stolyarov.info/books/programming_intro/vol1
tags:
  - research
  - inbox
  - SR_programming
sr-due: 2024-01-26
sr-interval: 1
sr-ease: 130
directory:
  - ~/Computer/programming/Столяров-Программирование
---

# Introduction 1, philosophical (Предисловие 1, философское)

Author tell how he wrote this book, what difficulties he had and how
crowdfunding project helped him to write this book.

With crowdfunding project author can live and write book, without spending time
on other jobs. In total author spend 2200 hours (he tracks time somehow) to
write 3 volumes, books wasn't written from scratch (previous works and lectures
was used).

Author also doesn't like current situation with publishers, which make money on
books.

I think this preface is like historical reference, how he wrote this book. Also
was told which topics was touched ([[Pascal]], `NASM`, [[C]],
[[Operating_system|OS]], paradigms, etc.) and reworked during writing this book,
who helped author and other aspects of writing process.

# Introduction 2, methodical (Предисловие 2, методическое)

You can study programming only by yourself (maybe too categorical).

Learning programming by writing GUI applications (event-driven approach) is bad
idea.

Main tool of professional Unix user is **organized** command line
([[Command-line_interface_CLI|CLI]]).

Command line interface is more powerful and flexible than GUI, you can work with
it faster, less stress on hands, operations are easier to remember and so on.

You can write CLI program much easier than GUI program. This open new learning
opportunities and customization of OS (hobby programming).

Reasons why Unix is the most suitable OS for learning programming:

### Mathematical reason (Математическая причина)

Any [[Computer_programming|program]] is a record of ==algorithm== on some
programming language.
<!--SR:!2024-02-25,4,187-->

On very fundamental level no-one knows what algorithm it is, that's why we have
[[Computational_problem|computational problems]], and theoretical
[[Computer_science|computer science]].

Algorithm make transformation from set of [[Word|words]] (chains of symbols over
some alphabet) into the same ==set==.
For this transformation can exist more than one algorithm (countless) or not
exist.
<!--SR:!2024-03-04,15,227-->

Algorithm is such a "thing" which read input word, do something **constructive**
and return another word.

The same way works many programs from Unix family. STDIN → transformations →
STDOUT (filters) and you can combine them using pipes.

### Psychological reason (Психологическая причина)

Programming can't be learned in traditional ways, it's more craft and need you
do a lot of practice which solve real world problems (not just write code to
learn some algorithm or theory). This is why pet projects are important, some
pet projects can be transformed into very useful projects (GNU/Linux,
open-source projects, etc.). And when you get real users of your software you
are established as programmer and can congratulate yourself.

### Ergonomic reason (Эргономическая причина)

You can't replace CLI usability with any graphical UI. And you must learn CLI
as soon as possible (I use it every day, but still not very effective).

### Pedagogical reason (Педагогическая причина)

Is good idea to educate someone, when you haven't enough experience and when
you're even not trying to use proven learning materials?
&#10;
Don't need to learn someone programming if you don't know what is in fundamental
level. And if you really want to learn someone find good proven education path.
Bad teachers can mislead a newbie student, for example start learning
programming with making GUI (focusing on UI, not a program logic), which is bad
idea. It can traumatize student mindset, and he will have many problems to
relearn programming in future (if he can do it) and think programming is boring
process (will not know what he lost).
<!--SR:!2024-02-24,4,182-->

### Language determines thinking (Язык определяет мышления)

Why need to learn form "simple" languages, which providing basic concepts and
not too complicated?
&#10;
Stating learning programming from complex programming languages (like Java, C++
and even C) is bad idea, newbie learners will have hard been understanding their
concepts and not really will learn programming.

Knowing [[Data_structure|data structures]] is important, if you're not
understanding difference (and in result where they can be used) between `vector`
and `list` in C++ and you **won't understand it** this is bad sign.

Mixing C and C++ is bad idea (maintainability reason).

Why learning C as first programming language is not so good?
&#10;
C as first programming language is not suitable, you need to understand pointers
first and work with them (and it's hard).
<!--SR:!2024-02-23,3,162-->

Why knowing language on fundamental level is important?
&#10;
Understanding code as "magic commands" is not good for good programmers, you
need to understand code on very low level to create truly effective programs.
<!--SR:!2024-02-23,3,162-->

In C you haven't procedures, only functions. Even assignment, increment are
arithmetic operations. And in C formally any actions (which is core of C) are
creating [[Side_effect|side effect]].

> Side effect can be appeared only when evaluating expression.
Side effect this is arbitrary change, which occurring when evaluating expression
and then can be somehow ==detected==.
<!--SR:!2024-02-28,10,227-->

Unlike C, C++ and functional programming languages, in [[Pascal]] there mostly
no side effects.

```c
while((dest++ = * src++));
```
Why you should not write code like this? To avoid side effects and make this
less cryptic.
Yes in C you can't avoid side effects anyway, but in other languages you can.

When knowledge of C can be useful?
&#10;
Writing in C is requirement, you need to understand how computer and operating
system is working on subconscious level to write really **quality programs**.
<!--SR:!2024-02-22,2,152-->

Learning C, here are some requirements in understanding pointers and
recursion, which can help some another language ([[Pascal]]):
- language fully support pointers
- you can use language without pointers
- using pointers you can extend your capabilities (real necessity)

Is deep learning Pascal (in details) is needed when you learn general
programming?
&#10;
Not really. You learn not Pascal, you learn programming by using Pascal, and you
can omit some Pascal specific features.
<!--SR:!2024-02-23,5,182-->

Why need to learning Assembly language (at least basics)?
&#10;
Big role in understanding programming is taking [[Assembly_language|Assembly
language]]. You can never write programs in it (prefer C is recommended), but
you must understand how it works to understand what you are really doing,
understand OS kernel, how to interact with it, understand system calls, deeply
understand data structures, etc. And you need usually also learn it before C
(but after Pascal). You can use any assembly to learn, need to get understanding
how to work with registers and memory areas, understand stack frame, interrupts,
etc.

So chain to learn programming is: ==Pascal → Assembly → C → C++== (special
author's vision), OS, I/O, processes, sockets, multithreading, mutex objects and
semaphores, critical sections, etc.
<!--SR:!2024-02-24,3,162-->

# Introduction 3, parting words (Предисловие 3, напутственное)

First who created things which works on their own (automatically) are watch
mechanics. XVIII century - Jaquet-Droz ==automata== (most complex is penman,
containing 6000 details).
<!--SR:!2024-02-23,5,202-->

![Jaquet-Droz The Writer Automaton From 1774 In Action](https://www.youtube.com/watch?v=ux2KW20nqHU)
_Jaquet-Droz The Writer Automaton From 1774 In Action_

He not only invented these automata machines, hi also spent a lot of time to
make required tools and details, so making some complex automation system was
combination of many different skills, finances and physical labor.

With programmable computers you can avoid ==material== requirements to make
something useful and great. Program itself is finished product. Programming is
the most creative profession in engineering and technical professions.
<!--SR:!2024-02-22,4,182-->

What is 2 main things which are important for programmer?
&#10;
Self-education and practice is requirement to be programmer.
<!--SR:!2024-02-22,1,132-->

Author also tells you need to use CLI to learn something from this book (I use
it daily), which give you abilities to write simple programs and find program
users.

Programming requires maximum intellectual tension and not everyone can withstand
it!

# Book structure (Структура книги и соглашения, используемые в тексте).

Here mostly general information about books and volumes.