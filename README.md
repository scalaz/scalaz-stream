# scalaz-stream

## Goal

A high-performance, purely-functional streaming interface, with compositional semantics and a small, principled core that facilitates easy reasoning.

## Introduction & Highlights

* Purely functional
* Minimal Core
* Resource Safety
* High Performance
* IO Module

## Competition

| | FS2 | Monix | Akka Streams | 
---|---|---|---
Purely-functional| ✓ | x | x |
Minimal Core | ✓ | x | x |
Resource Safety | ✓ | ✓ | x |
High Performance | ✓ | ✓ | ✓ |
Back Pressure | ✓ | ✓ | ✓ |
IO Module | ✓ | ✓ | ✓ |

## Open questions

* Pull or Push based ?
* Design
  * Free Monad Based
    - Stack Safety independent of the target moand
  * Tagless Final
    - Stack Safety is dependent on the target monad, ZIO can be used but then we specialize to soon and maybe that’s fine.
  * Chunking 
    - For performance reasons, Streams should not work on a single elements but "chunks" of elements.


