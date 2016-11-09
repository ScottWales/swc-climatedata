---
title: "Optimising analyses"
teaching: 10
exercises: 5
questions:
- "How can I make my analysis faster"
objectives:
- "Explain the basics of optimisation"
- "Explain memory limits and lazy loading"
- "Explore Dask and chunking"
keypoints:
- "The easiest way to be faster is to do less work"
- "Reading the opposite end of an array is slow, reading from disk is slower"
- "Filling up memory makes the computer grind to a halt"
---

No-one likes their code to run slow. There are a number of ways you can improve performance

Reasons your calculations can run slow:

 * You're doing more work than you need to
 * Accessing memory out of order
 * Your computer's memory is full

### Reduce your workload

The fastest way to do a calculation is to not need to do it at all. Has someone
else done the same calculation?

Use appropriate input data - don't get 3-hourly when monthly would work fine

If needed subset data before other operations

### Memory and Caches

When working with big arrays the order that you read memory can be important.
Computer memory is (to first order) linear, arrays are flattened in memory. -
it's quick to access data close in memory, but slow to access data far away.
Data is read into fast cache in chunks

Prefer whole-array operations to creating your own loops

As much as possible do the same operation on every grid point, avoid conditionals

> ## Example: Loop access patterns
> Let's look at different ways of iterating over loops
{: .callout}

### Full memory

When your computer's memory is full, there are a few things that can happen

 * Bits of memory that aren't being used can be written to disk, to be read back later when needed (swapping memory)
 * The computer can attempt to free up memory by killing a running program (OOM killer) (Generally happens at NCI)

You may hear your computer's hard disk churning
Or processor usage takes a nosedive

Reading and writing to disk is much much slower than RAM

Free up memory after use - Python will automatically free memory for you when exiting functions (garbage collection), in some other languages you need to manually free

Operate on less data at once - rather than load a bunch of files to average them together, load them one at a time, close them when done

Xarray can also automatically split data into chunks, only working on a bit of the whole field at a time
 * Will also do some parallelisation, but can only read serially

> ## Example: Chunking 0.25 degree ocean data
> What are the benefits of chunking with really big files (not using OPENDAP here!)
> 70 GB file `/g/data/v45/mom/mom01v3/output060/temp_snap.nc`
{: .callout}

