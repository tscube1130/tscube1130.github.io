---
title: "NanoMatch: Building a Sub-Microsecond Limit Order Book in C++20"
date: 2026-05-26
categories: [projects]
tags: [cpp, systems, low-latency, trading]
---

*Detailed writeup coming soon.*

## Overview

NanoMatch is a ultra-low latency limit order book (LOB) matching engine built in C++20,
achieving a median matching latency of **79.6ns** and a sustained throughput of
**20.64 million orders per second**.

## Key Engineering Decisions

- Zero-allocation hot path using custom cache-aligned memory arenas
- Zero-copy market data ingestion via OS-level `mmap`
- Branchless integer parsing
- 278% latency reduction over standard STL implementations (validated with Linux perf)

*Full writeup with design decisions, benchmarks, and lessons learned — coming soon.*
