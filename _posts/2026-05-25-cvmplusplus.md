---
title: "CVM++: Engineering a Bytecode Compiler and Stack-Based Virtual Machine from Scratch"
date: 2026-05-25
categories: [projects]
tags: [cpp, compilers, virtual-machine, languages]
---

*Detailed writeup coming soon.*

## Overview

CVM++ is a Turing-complete, stack-based Virtual Machine and Bytecode Compiler
built entirely in C++17 — no external parser generators (Flex, Bison) used.

## Architecture

A strict 4-phase execution pipeline:

1. **Lexical Analyzer** — custom tokenizer
2. **Recursive Descent Parser** — handwritten, no generators
3. **AST Generation** — abstract syntax tree construction
4. **Bytecode Emitter** — compiles AST to stack-based bytecode

The VM supports dynamic call frames, global memory scoping, iterative control flow,
and native runtime exception handling.

*Full writeup with design decisions, language spec, and implementation details — coming soon.*
