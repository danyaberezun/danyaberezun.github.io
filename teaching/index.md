---
layout: default
---

---

## Intoruction to Functional programming

The course is an introduction to functional programming.
We will discuss some basic concepts and approaches in this area, such as lambda calculus and reduction orders, lazy evaluation, type systems and type inference, polymorphism, inductive and functional data structures, folds, memoization, continuations, algebraic data structures, functors, monads, recursion schemes, proof of program properties, etc.
We will also see how these concepts and approaches solve important and interesting practical problems.
Students will learn how to create applications in a pure functional programming language **Haskell**.
Besides coding, students will learn how to test their programs, and how to use developers tools to debug and improve programs’ efficiency.
The course provides solid ground for using the functional programming paradigm in mainstream languages and is a prerequisite for many programming languages theory courses.

Readings (together with [Ekaterina Verbitskaia](https://kajigor.github.io/)):

| Place | Year | Role | Comments | Matherials |
| :--- | :--- | :--- | :--- | :--- |
| [Neapolis University](https://www.nup.ac.cy/department-of-computer-science/) | Spring 2023 | Lectures + practices | Short week intensive | |
| [Jacobs University<br />(now Constructor University)](https://www.jacobs-university.de/) | Autumn 2022 | Lecturer | | Lectures (see below) <br /> [Practice](https://github.com/kajigor/fp-2022-jub-fall/) |
|<img width=150/>|<img width=100/>|<img width=120/>| <img width=150/>| <img width=150/>|

Lectures:

- [Intro, ADT]({{ site.baseurl }}{% link /teaching/assets/FP/2022/intro_adt.pdf %})
- [Lazy, Forcing, Tail Recursion]({{ site.baseurl }}{% link /teaching/assets/FP/2022/haskell-specifics.pdf %})
- [Functional Data Structures]({{ site.baseurl }}{% link /teaching/assets/FP/2022/functional-data-structures.pdf %})
- [Lambda-calculus: basics]({{ site.baseurl }}{% link /teaching/assets/FP/2022/lcalc2.pdf %})
- [Lambda-calculus: reduction strategies, CR]({{ site.baseurl }}{% link /teaching/assets/FP/2022/reductions.pdf %})
- [Simple types, System F, Hindley--Milner]({{ site.baseurl }}{% link /teaching/assets/FP/2022/types.pdf %})
- [Continuations]({{ site.baseurl }}{% link /teaching/assets/FP/2022/continuations.pdf %})
- [Zippers and "Optics"]({{ site.baseurl }}{% link /teaching/assets/FP/2022/zippers_lens_prism.pdf %})

---

## Introduction into Metacomputations (Введение в метавычисления)

[ENG]
The course is an introduction into metacomputations, a field of computer science that deals meta-programs design.
Meta-program is a program that manipulate other programs as data, including generating other programs as a result of its work.
The area is closely related to program optimizations and programming languages semantic, as well as exposure to program generation.
Students are introduced to the concepts of Futamura projections, program specialization, supercompilation, distillation and so on.
In practice, it is expected that both a self-applied tiny Pascal-like language specializer capable of generating programming language compilers by their interpreters and a positive supercompiler of simple functional language would be implemented.

[RUS]
Курс является вводным в метавычисления --- области информатики, занимающейся проектированием мета-программ, т.е. программ, манипулирующих другими программами как данными, в том числе, порождая последние как результат своей работы.
Эта область тесно связана как с программными оптимизациями и семантиками языков программирования, так и с автоматической генерацией программ.
Слушатели знакомятся с понятиями проекций Футамуры, специализации программ, суперкомпиляции, дистилляции и т.п.
На практике ожидается, что каждый реализует как самоприменимый специализатор игрушечного Pascal-подобного языка, способный порождать компиляторы языков программирования по их интерпретаторам, так и позитивный суперкомпилятор простого функционального.

**Videos**:
* [Open lecture / Открытая лекция по метавычислениям (RU)](https://youtu.be/1j4TEWOMoQs)
* [Lecutres records / Записи лекций (RU)](https://www.youtube.com/playlist?list=PL1X5sYUeXRNdCAY8LcMARSbyn2n20KTrm)

**Past readings**:

| Place | Year | Role |
| :--- | :--- | :--- |
| HSE + IFMO | 2021 | Lectures + practices |
| HSE + IFMO | 2020 | Lectures + practices |
| HSE + IFMO | 2019 | Lectures + practices |
| HSE + IFMO | 2018 | Lectures + practices |
| AU  | 2017 | Lectures + practices |
| AU  | 2016 | Lectures + practices |
|<img width=150/>|<img width=100/>|<img width=120/>|

**Bibliography**:

* [N.D. Jones, C.K. Gomard, and P. Sestoft. Partial Evaluation and Automatic Program Generation](https://www.itu.dk/people/sestoft/pebook/)
* Partial Evaluation Practice and Theory, Lecture Notes in Computer Science, J.Hatcliff, T.Morgensen, P.Thiemann
* Logic-Based Program Synthesis and Transformation, editor Maurizio Gabbrielli
* K.Launchbury, Projection factorisations in partial evaluation
* [A series of PEPM workshop proceedings](https://popl23.sigplan.org/home/PEPM-2023)
* [A series of META workshop proceedings](http://meta2016.pereslavl.ru/index.html)
* Staged multi-result supercompilation: Filtering by transformation by Sergei Grechanik, Ilya Klyuchnikov, Sergei Romanenko
* Geoff W. Hamilton. The Next 700 Program Transformers. LOPSTR 2021: 113-134


---

## Compilers

[ENG]
The course is an introduction to the field of programming languages, compilers, and other language tools.
The course includes some basic concepts and approaches in the area, such as the operational semantics of programming languages, intermediate representation of programs, interpretation, program transformations, etc.
It also shows how these concepts and approaches solve important and interesting practical problems.
It is assumed that students in the process of completing assignments by the end of the course will implement a full-fledged compiler to machine code for a simple but fully functional imperative programming language ([Lama](https://github.com/JetBrains-Research/Lama)) containing expressions, assignments, control constructs, higher-order functions, and dynamic data structures.
The same language is used as the main source language throughout the course.

* [Paper describing the course (TFPIE’21): Reimplementing the Wheel: Teaching Compilers with a Small Self-Contained One](https://arxiv.org/pdf/2207.12698.pdf)

Past readings:

| Place | Year | Role |
| :--- | :--- | :--- |
| [Constructor University](https://www.jacobs-university.de/) | Spring 2023 | Lectures + practices |
| [Neapolis University](https://www.nup.ac.cy/department-of-computer-science/) | Spring 2023 | Lectures + practices |
|<img width=150/>|<img width=120/>|<img width=200/>|

**Bibliography**:

* [A brilliant list of books on compiler construction](gcc.gnu.org/wiki/ListOfCompilerBooks)
* [Compiler GCC](gcc.gnu.org)
* [Infrastructure LLVM](llvm.org)
* N.Wirth. Compiler Construction
* F.Nielson, H-R.Nielson. Semantics with Applications. A formal introduction
* D.Knuth. Semantics of context-free languages
* G.Hutton, E.Meijer. Monadic parser combinators
* [x86 instruction set description](http://www.felixcloutier.com/x86)

***[RUS] Введения в компиляторы / Языки программирования и компиляторы***

Данный курс представляет собой начальное введение в область языков программирования, компиляторов и других языковых инструментов.
Курс включает некоторые основные понятия и подходы в данной области, такие, как операционная семантика языков программирования, промежуточное представление программ, интерпретация, преобразования программ и т.д.,
а также показывается, как эти понятия и подходы решают важные и интересные практические задачи.
Предполагается, что слушатели в процессе выполнения заданий к концу курса реализуют полноценный компилятор в машинный код для простого, но вполне функционального языка императивного программирования ([Lama](https://github.com/JetBrains-Research/Lama)), содержащего выражения, присваивания, конструкции управления, функции высших порядков и динамические структуры данных.
В качестве основного инструмента в рамках курса будет использован тот же самый язык.

(RU)
* [Более подробное описание и программа курса](https://my.compscicenter.ru/courses/2021-spring/1.879-compilers/)
* [Lecture records 1 / Записи лекций 1](https://www.youtube.com/playlist?list=PL1X5sYUeXRNfA3rJ6fnSekJALaqvW094-)
* [Lecture records 2 / Записи лекций 2](https://www.youtube.com/playlist?list=PL1X5sYUeXRNdvV1DxB2j5F-O3XlkqptcD)

Past readings (together with [Dmitri Boulytchev (Дмитрий Юрьевич Булычев)](https://github.com/dboulytchev/)):

| Place | Year | Role |
| :--- | :--- | :--- |
| HSE + IFMO | Autumn 2021 | Lectures + practices (2 times) |
| CSC + ETU  | Spring 2021 | Practices |
| HSE + IFMO | Autumn 2020 | Lectures + practices |
| FMCS SPbU  | Autumn 2020 | Lectures + practices |
| CSC + ETU  | Spring 2020 | Lectures + practices (2 times) |
| HSE + IFMO | Autumn 2019 | Lectures + practices |
| CSC + ETU  | Spring 2019 | Lectures + practices (2 times) |
| HSE + IFMO | Autumn 2018 | Lectures + practices (2 times) |
| CSC + ETU  | Spring 2018 | Lectures + practices |
| AU         | Autumn 2017 | Practices |
|<img width=150/>|<img width=120/>|<img width=200/>|

Past readings (Language processors design technologies and tools / Технологии и инструменты построения языковых процессоров (together with [Anton Podkopaev (Антон Викторович Подкопаев)](https://podkopaev.net/)):

| Place | Year | Role |
| :--- | :--- | :--- |
| IFMO | Осень 2017 | Lectures + practices |
| AU   | Осень 2016 | Lectures + practices |
| IFMO | Осень 2016 | Lectures + practices |
| IFMO | Осень 2015 | Lectures + practices |
|<img width=100/>|<img width=100/>|<img width=120/>|

---

## Other

| Course | Year | Place | Role |
| :--- | :--- | :--- | :--- |
| Mathematical logic in Computer Science (Математическая логика в Информатике) | Spring 2021 | FMCS SPbU | Practices |
| Operational Systems (Операционные Системы) | Spring 2021 | FMCS SPbU | Practices |
| Linux Basics (Основы Linux) | Autumn 2020 | FMCS SPbU | Lectures + practices |
| Programming Basics (Основы Программирования) | Autumn 2020 | FMCS SPbU | Practices |
| Computer Architecture (Архитектура компьютерных систем) | Autumn 2020 | FMCS SPbU | Practices |
| Introduction into OOP (Введение в ООП) | Autumn 2020 | FMCS SPbU | Practices |
|<img width=400/>|<img width=120/>|<img width=120/>| |

---

