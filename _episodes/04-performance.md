---
title: "Optimising analyses"
teaching: 30
exercises: 10
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


 * Subset the data, explore chunking options
   * Explain Dask, memory limits

 * Load multiple files with chunking
   * Compare loops vs whole-array operations
