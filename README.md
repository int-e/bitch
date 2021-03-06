# bit** programming language

This repository contains two implementation of
https://github.com/Helen0903/bitch, one in Haskell, and the other in C++.

(Note that despite the offensive name, the language itself is surprisingly interesting.)

The following distinguishing features are implemented:

* big integers, offering unbounded memory

* the additional operation <code>%</code> dumps the current state and the
  next instruction

  format:
  <code>% .. accumulator (in hex) | reverse storage .. instruction</code>

  example:
  <code>% .. 0000 0000 0000 0001 | 8000 0000 0000 0000 .. ^^[1</code>

## files

* [hs/bit-h.hs](hs/bit-h.hs): Haskell interpreter source
* [cc/shifty.cc](cc/shifty.cc): C++ interpreter source
* [examples/cat](examples/cat), [examples/rev](examples/rev): cat and reverse
* [examples/hello](examples/hello): Hello, world!
* [examples/rot13](examples/rot13): rot13, generated from [examples/rot13.pp](examples/rot13.pp)
* [examples/rot13-lut](examples/rot13-lut): another rot13, generated from [examples/rot13.pp](examples/rot13-lut.pp)
* [examples/quine](examples/quine): quine
* [examples/brainfuck](examples/brainfuck): Brainfuck interpreter, generated from [examples/brainfuck.pp](examples/brainfuck.pp)
