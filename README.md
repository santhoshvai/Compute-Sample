# Compute and Memory -Sample

## Compute

* Slow function performance can be fixed by batching and caching
  * Used `traceview` to find that fibonacci is slow
  * caching applied to it to make it fast enough

* Blocking the UI thread
  * used `traceview` to find that image sepia filter function was slow
  * moved to background thread using an `asyncTask`

* container performance - dataStructure
  * used `systrace` to find performance number is milliseconds
  * replacing integer array with hashmap made the function faster

## Memory

* Memory Leaks
  * Used `Memory Monitor` and `Heap Viewer` tool to find memory leaks
  * When you add listeners, be sure to clean them up.
  * An `Allocation Tracker` can also find memory leaks

* Memory chrun - lots of new allocations at same time - like in a for loop
  * Used `systrace` to find that many GC events occurred and where the allocations happen
  * replaced string concatenation with string buffer to fix it

## TOOLS

* [Systrace Walkthrough](http://developer.android.com/tools/performance/systrace/index.html)
* [TraceView Walkthrough](http://developer.android.com/tools/performance/traceview/index.html)
* [Memory Monitor Walkthrough](http://developer.android.com/tools/performance/memory-monitor/index.html)
* [Heap Viewer Walkthrough](http://developer.android.com/tools/performance/heap-viewer/index.html)
* [Allocation Tracker Walkthrough](http://developer.android.com/tools/performance/allocation-tracker/index.html)
