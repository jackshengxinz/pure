# Serverless Traces

## Data Scheme

|Variable|Description|
|--------|-----------|
|`cpu`|CPU allocation in `cpu.shares`|
|`memory`|memory allocation in MB|
|`duration`|function execution time in ms|
|`maxRss`|maximum resident set size used in kilobytes|
|`fsRead`|the number of times the file system had to perform input|
|`fsWrite`|the number of times the file system had to perform output|
|`vContextSwitches`|the number of times a CPU context switch resulted due to a process voluntarily giving up the processor before its time slice was completed (usually to await availability of a resource)|
|`ivContextSwitches`|the number of times a CPU context switch resulted due to a higher priority process becoming runnable or because the current process exceeded its time slice|
|`userDiff`|CPU time spent in user mode in microseconds|
|`sysDiff`|CPU time spent in system mode in microseconds|
|`rss`|resident set size (in bytes), the amount of space occupied in the main memory device (that is a subset of the total allocated memory) for the process|
|`heapTotal`|total size of the heap in bytes|
|`heapUsed`|size of the actually used heap in bytes|
|`external`|the memory usage of C++ objects bound to JavaScript objects managed by V8 (in bytes)|
|`elMin`|minimum recorded event loop delay|
|`elMax`|maximum recorded event loop delay|
|`elMean`|average recorded event loop delay|
|`elStd`|the standard deviation of the recorded event loop delay|
|`bytecodeMetadataSize`|the size of bytecode and metadata in heap (in bytes)|
|`heapPhysical`|the total physical size of the heap|
|`heapAvailable`|the total available heap size|
|`heapLimit`|the limit of the heap size|
|`mallocMem`|the malloced memory size in heap|
|`netByRx`|received bytes|
|`netPkgRx`|received network packets|
|`netByTx`|transmitted bytes|
|`netPkgTx`|transmitted network packets|
|`memory_util`|memory utilization|
|`cpu_util`|cpu utilization|
```
