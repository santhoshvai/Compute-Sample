# Compute and Mempry -Sample

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