---
title: Algebraic Effects
tag: PL
---

Algebraic effect intros and literature

<!--more-->

Algebraic effects

### Eff

Work by Matija Pretnar and Andrej Bauer

[Tutorial paper](https://www.sciencedirect.com/science/article/pii/S1571066115000705)

[OPLSS course](https://www.cs.uoregon.edu/research/summerschool/summer18/topics.php#Bauer) by Andrej Bauer

### All sorts of implementation

[Handlers in Action](https://dl.acm.org/doi/10.1145/2544174.2500590) (focused on Haskell but also has racket, SML, OCaml implementation)

Richer Type systems (Frank): [Do be do be do](https://dl.acm.org/doi/10.1145/3009837.3009897)

### Comparison to Monads

[Monad transformers and modular algebraic effects: what binds them together](https://dl.acm.org/doi/10.1145/3331545.3342595)

### Recent papers

**WasmFX** (typed continuation proposal for wasm's exception handling feature). [[Wasm Research Day 2023 talk]](https://youtu.be/gNb0M312Wds?si=kONvK1oyEtBPjdmX), the 2022 talk has no recording but there are [[slides and code]](https://www.cs.cmu.edu/~wasm/wasm-research-day-2022.html) [[OOPSLA 23 paper]](https://dl.acm.org/doi/10.1145/3622814)

**Koka-lang** [[PLDI24 paper]](https://dl.acm.org/doi/pdf/10.1145/3656398)

### Delimited Continuations

Now in Scala/Haskell/OCaml

Ken Shan did a lot of work on inter-defining control operators


### Questions

In *Effect Handlers via Generalised Continuations* (JFP 20), they claimed catamorphism <-> deep handlers, mutumorphisms <-> shallow handlers. How to interpret this? (Do I really know case-splits and folds?)

How to think of `shift0/reset0` as closest to algebraic effect handlers? *On the Expressive Power of User-Defined Effects* seems to give a straightforward translation from `shift0/reset0` to effect handlers.

(More to come...)
