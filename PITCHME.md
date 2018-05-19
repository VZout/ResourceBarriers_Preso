@title[Title]

# Resource Barriers

(For modern graphics API's)

<span cla<strong>Viktor Zoutman</strong></span>, November 20 2017

---

@title[Contents]

### Contents 

- What is a barrier
- Hardware
- Caches
- DirectX12's barriers

---

@title[What is a barrier]

## "Barrier"
- Synchronization point
- Fence


## "Memory Barrier"
- Lock free programming
 
---

@title[Concurrency]

## Why and when barriers?

- Dependencies
- Basic Concurrency Issues
- Super Scalar Pipeline
- Multithreading / Interprocess Communication

---

@title[GPU]

## GPU architecture

- Massive amount of cores
- Embarrasangly parallel problems
- Serial command buffers(lists) but prallel executation.

// insert image from NISIGHT

---

@title[GPU]

- ROP's (Render output unit)
- Overlapping draws and dispatches 
- Higher throughput
- Flush / Wait for idle |
- Bloom

---

@title[Caches]

## CPU Caches & Concurrency

- Multiple L1 caches
- Shared L2 & L3 cache
- Cache coherency

---

@title[Caches]

## GPU Caches

- Barriers for caches.

---

@title[Caches]

## Memory Bandwidth in modern games.

- 8294400 |
- * 8 bytes |
- X for GBuffers |
* * 4 (x4 mssa) |

---

@title[Caches]

- Compression build into ROP's
- Compression by comparing neighbouring pixels.
- Barriers for pixel reads & writes

---

@title[D3D12]

## Barriers in DirectX and Vulkan

- High level
- Describes the flow of data
- What about DX11 and OGL?
