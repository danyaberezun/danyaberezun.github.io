---
layout: default
---

This page contains a (non-exhaustive) list of topics (and research areas) for student projects, one- and two- term projects, diplomas, and graduation thesis.

The list of tasks/topics is not exhaustive and highly varies depending on a student's prior experience and knowledge.
Please, do not hesitate to contact me for more details.

---

# Relational programming with miniKanren/OCanren

***Keywords***: relational/logic programming, profiling, embedded languages

### Description

[OCanren](https://ocanren.readthedocs.io/en/latest/) is a strongly-typed embedding of [miniKanren](http://minikanren.org/) relational programming language into [OCaml](http://ocaml.org).
Nowadays, the implementation of OCanren strongly resembles [faster-miniKanren](https://github.com/michaelballantyne/faster-miniKanren).
Previous implementation was based on [microKanren](http://webyrd.net/scheme-2013/papers/HemannMuKanren2013.pdf) with [disequality constraints](http://scheme2011.ucombinator.org/papers/Alvis2011.pdf).

### Actual topics/projects:
* [Easy, introduction project] Implement a set of useful programs on OCanren; for example, a schedule generator for a university that takes into account the restrictions and wishes of the university and teachers
* Visualiser of miniKanren execution
* OCanren/miniKanren profiler gathering information about relations calls
* Dynamic compiler for OCanren
* **OCanren search parallelization**.  The crucial part of of any relational programming language is the search of answers. The goal of the project is to research and development of a suitable way to parallelize the search in order to speed it up.
* Enrich [Haskell^{-1}](https://www-ps.informatik.uni-kiel.de/~fte/papers/Haskell-1.pdf) approach with miniKanren interleaving and compare with existing miniKanren implementations
* Embed minikanren into mainstream language like Kotlin

Useful links:
* [Fail Fast and Profile On: Towards a miniKanren Profiler](https://drive.google.com/file/d/1ldMlExvR7Sb-M5wJVgayzHokMxinuWYg/view)
* [Some criteria for implementations of conjunction and disjunction in microKanren](https://drive.google.com/file/d/18OzQurXbmoeFn-bJUDZCZ-FPkGwo5mFL/view)
* [Efficient fair conjunction for structurally-recursive relations](https://popl21.sigplan.org/details/pepm-2021-papers/9/Efficient-Fair-Conjunction-for-Structurally-Recursive-Relations)

***Knowledge in the following areas would be a plus***:
* Basic knowledge in programming languages theory
* Basic knowledge in programming languages formal semantics
* Experience with functional programming paradigm (Haskell/OCaml/Scheme/Racket/...) 
* Basic knowledge of logic/relational programming

---

# Lama compiler and infrastructure

***Keywords***: compilers, semantics, static analisys, code generation

[Lama](https://github.com/PLTools/Lama) is a programming language developed by JetBrains Research for educational purposes (as an exemplary language to introduce the domain of programming languages, compilers, and tools).
It currently exists for x86_64 architecture only.
There are many directions for its (and its infrastructure) development, both scientific and purely technical:

* Implement a lsp-server (together with a basic plugin for VSCode/IntelliJ which runs the server for all .lama files); useful links: [ocaml-lsp](https://github.com/ocaml/ocaml-lsp), [lsp-spec](https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/)
* Implement a native compiler to ARM (32 and/or 64) [the task can be naturally extended with advanced register allocation]
* Implement a native compiler to x86_64 [the task can be naturally extended with advanced register allocation]
* Lama memory management; current garbage collector is a tiny simplest mark-and-copy stop-the-world algorithm; it can be improved in a number of ways: mark-and-compact, generational (partial) GC, concurrent and/or parallel GC, ...
* Support compilation into OCaml; useful link: [Malfunctional](https://web.archive.org/web/20170725050716/https://www.cl.cam.ac.uk/~sd601/papers/malfunction.pdf)
* Develop a weak (or at least gradual) type system
* Compiler into LLVM-IR; This task can be extended later to support specialization of the generated IR subset
* Implement a tool set for support different static analysis approaches
* Partial evaluator for generated x86_32 GASM subset
* Concurrency
* Make tag hashes smarter (a-la like in ocaml)
* ...

***Requirements***

* Basic knowledge of functional programming
* The very basic knowledge about compiler design
* Ability to read documentation and papers in English
* Desire to work and learn something new =)

---

# Patching OCaml and ML-like languages

***Keywords***: functional programming, OCaml, compilation 

### Description

[OCaml](http://ocaml.org) is one of the mainstream functional programming languages.
The project aims to bring new features in ML-like languages and produce some patches fixing ad-hoc or poorly designed language features such as polymorphic variants, active patterns, and modules.

### Actual topics/projects:
* ML to .Net\\
  Long-term goal: port OCaml with all the features into .Net   {% comment %} .Net has RTTI ;) {% endcomment %} \\
  Short-term goal: miniML & SML to .Net \\
  Useful links: [ocamil](https://github.com/nojb/ocamil), [smldotnet](https://github.com/kaveman-/smldotnet), [a paper](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.58.4305&rep=rep1&type=pdf), [miniML](https://gitlab.com/Kakadu/fp2020-materials-private/-/tree/master/miniml)
  {% comment %} [kakadu's parser for miniML](https://gitlab.com/Kakadu/fp2020-materials-private/-/tree/master/miniml) {% endcomment %}
* OCaml to JVM
* Patching polymorphic variants for OCaml\\
  Usefull links: [a paper](https://arxiv.org/pdf/1606.01106.pdf), [Tommaso Petrucciani PhD thesis](https://tel.archives-ouvertes.fr/tel-02119930/document) and [prototype](https://gitlab.math.univ-paris-diderot.fr/petrucciani/setvariants/-/tree/master)
 
***Knowledge in the following areas would be a plus***:
* Basic knowledge in programming languages theory
* Basic knowledge in programming languages formal semantics
* Experience with functional programming paradigm (Haskell/OCaml/Scheme/…) 

---

# Metacomputations

***Keywords***: functional programming, metacomputations, program specialization, inverse programming

### Description

The aim of this project is research and practical application of metacomputation techniques such as partial evaluation, supercompilation, distillation, and inverse programming.

### Actual topics/projects:
* On-the-fly specialization/SC as a plugin for IDE\\
  Goal: implement high-level specialization for some mainstream language as a plugin for IDE
* Enrich [Haskell^{-1}](https://www-ps.informatik.uni-kiel.de/~fte/papers/Haskell-1.pdf) approach with miniKanren interleaving and compare with existing miniKanren implementations
* DSL compiler generation\\
  Goal: automatically generate a compiler from the DSL implementation
* Machine code specialization\\
  Short-term goal: enrich and reimplement approach from [the paper](https://dl.acm.org/doi/10.1145/2858965.2814321) to tiny subsect of X86 generated by [training compiler for Lama](https://github.com/JetBrains-Research/Lama)
* [research] Trace-based Just-in-Time Type Specialization for Dynamic Languages
* [research] Just-in-Time Value Specialization
* [research] Representation-Based Just-In-Time Specialization and the Psyco Prototype for Python
* [research] Guided just-in-time specialization
* [research] Optimizing Matlab through Just-In-Time Specialization
* [long-term] Framework for semantics-based program/infrastructure generation

***Knowledge in the following areas would be a plus***:
* Basic knowledge in programming languages theory
* Basic knowledge in programming languages formal semantics
* Experience with functional programming paradigm (Haskell/OCaml/Scheme/…) 
* Some knowledge in automatic program transformation and generation

---

{% comment %}
Здесь представлен список тем для студенческих проектов, курсовых, дипломов и выпускных работ.

Если Вы заинтересованы в поиске темы в одной из моих областей интересов, но не нашли подходящей ниже и/или таковая уже занята --- просто напишите мне и мы постараемся сформулировать её вместе.

Сводная табличка тем: (см. описание ниже)
=========================================

|№  | Тема | Область | Свободна? |
|----------|:-------------|:------|:------:|
| 1 | Semi-local LCS + oneAPI (DPC++) | Semi-Local LCS and SA | Да |
| 2 | Semi-local LCS vs. Accel-alignment | Semi-Local LCS and SA | Да |
| 3 | Beta-версия плагина для языка Vyper | Software Engineering / Vyper / Smart-Contracts | Нет |
| 5 | Специализация низкоуровнего кода | Program Specialization | Да |
| 6 | Специализация трассирующих call-by-name интерпретаторов | Specialization and Traversal-Based Normalization | Да |


Описание тем
=========================================

## 1. Semi-local LCS + oneAPI (DPC++)

Задачи полу-локального поиска --- расширение стандартных задач поиска наибольшей общей подпоследовательности и выравнивания строк.
Актуальной является задача эффективной реализации существующих алгоритмов под разные архитектуры.
DPC++ --- своеобразное развитие языка C++, позволяющее использовать код для любой архитектуры (в т.ч. CUDA, FPGA, CPU, ...).
*Задача*: взять существующую реализацию ряда алгоритмов полулокального поиска (из нашей статьи на ICPP'21), адаптировать их для DPC++, протестировать на платформах, сравниться с битовым алгоритмом Hyyro.

Возможность публикацуии: на интеловскую конфу с эвалюэйшеном

Связанные работы: Наша статья на ICPP'21 (увы, пока нет в свободном доступе)

Курс: 3,4

Сложность: 3 (норм)

## 2. Semi-local LCS vs. Accel-alignment
Accel-align --- новый инструмент для выравнивания последовательностей (потенциально state-of-the-art).
Задача аккуратно разобраться в его сути, а также сравнить с недавно реализованными (нашими) алгоритмами полулокального поиска (провести evaluation с https://github.com/NikitaMishin/semilocal).

Возможность публикацуии: на студенческую конфу

Курс: 2, (м.б. 3)

Сложность: 3 (норм)

## 3. Beta-версия плагина для языка Vyper

Vyper --- набирающий популярность язык для написания смарт-контрактов, имеет pythonic синтаксис, не Тьюринг полный, реализован максимально безопасно. Отсутствует полноценная поддержка в Intellij Platform.
Есть частично готовый плагин для языка Vyper. Есть ряд issues, связанных с тем, что плагина нет в магазине плагинов в Intellij Platform.
Задача стоит в расширении функциональности плагина, а также завершения его в минимальный work product (чтобы любой пользователь мог его установить через магазин).

Студент в процессе разработки: 

1. научиться писать плагины под Intellij Platform
2. прокачает написание кода на Kotlin
3. Выгодно тем, что если студенту понравится, то он будет в принципе готов быть джуном (мю) в команде разработки плагинов
4. Много технических деталей
5. Чтение чужого кода, написание кода (возможно придется написать заново)
6. Добавление новых фич:
  - Поддержка ошибок компиляции в коде
  - Анализ кода
  - Инфраструктура тестирования (Например, можно посмотреть на то, как сделано тестирование с помощью DSL для Scala)
  - Autocomplete
  - ....

Связанные работы: Курсовые Мишина и Тюрина

Возможность публикации: На студенческую или/ техническую конфу

Курс: 2, (м.б. 3)

Сложность: 3 (норм); много разных вариантов развития плагина

## 4. Специализация низкоуровнего кода

Специализация кода, генерируемого компилятором с курса компиляторов на его целевом языке. В идеале --- добиться его самоприменения.

Связанные работы:
- PE of C
- partial evaluation of machine code

Возможность публикации: Да (например, тематический воркшоп уровня B)

Курс: 3, 4

Сложность: >= 4

## 5. Специализация трассирующих call-by-name интерпретаторов

Проверить утверждение (formally + implement) про то, что трассирующая нормализация действительно позволяет с помощью umix генерировать хорошие компиляторы для языков по их интерпретаторам, по крайней мере в случае call-by-name интерпретатора.

Возможность публикации: На студенческой конфе и/или м.б. на тематическом воркшопе

Курс: 2--3 курс

Сложность: ~2--3, но надо будет разобраться со специализацией и Scheme


# Недооформленные темы / идеи

## Semi-local algorithms with AVX512 [Semi-Local LCS and SA]

Intra-processor parallelism in AVX512Subword-parallel iterative combing on AVX512BW (combing logic via VPCMPUB, VPMAXUB/VPMINUB).
Bit-parallel iterative combing on AVX512VL+AVX512F (combing logic via VPTERNLOGD).

Должно быть публикабельно в нормальном месте

3--4 курс

норм (2.5 -- 3)

## Сайт для поиска конференций (+ phd и т.п.)   [Инф.поиск + соц.сети + сайты]

Создать "сайт-инфраструктуру" для поиска всякой академической информации а-ля конференции, phd, вакансии и т.п.	?!

stringology, conferenceraks, wikicfp

2--3 курс

~2, много разных вариантов развития

## [Specialization]

Разработать general framework для генерации всего-всего (интерпретаторов, компиляторов, чекеров, верификаторов,…) по описанию семантики языков --- a la K-framework, но круче ;)

Да

Any

1--2

Сложно (4--5)


## [Specialization]

On-the-fly specialization аки плагин для IDE (профилятора)

TODO: research a little
Да

- Trace-based Just-in-Time Type Specialization for Dynamic Languages
- Just-in-Time Value Specialization
- Representation-Based Just-In-Time Specialization and the Psyco Prototype for Python
- Guided just-in-time specialization
- Optimizing Matlab through Just-In-Time Specialization
TODO
TODO

## Абстрактная интерпретация для C

Static analysis	TODO: research

TODO

TODO

3, 4, мага

TODO

## Верификация полу-локальных алгосов и теории на Coq [Verification]

TODO: specify what and how exactly

TODO

TODO

3, 4, мага

TODO


## Haskell^{-1} + interleaving ~===~ minicanren?

(automatic function inversion in haskell. Teegen, Prott, Bunkenburg)

## Dynamic compiler for ocanren

## TODO

implement an interpreter for some invertible language in minikanren and check that we can run it in different directions
{% endcomment %}