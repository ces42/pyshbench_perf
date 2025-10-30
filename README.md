# pyshbench
This is a modified version of [hazzl/pyshbench](https://github.com/hazzl/pyshbench/), a benchmarking tool for the stockfish chess engine implemented in python.

**NOTE:** you will probably need to edit the cpuset variable to use this on your computer

The `pyshbench_perf` script operates like `pyshbench` but measures clock cycles instead of elapsed time. Consequently, it is insensitive to changing clock speeds, and thus much more precise. However, some cpus can only execute certain instructions (AVX2, AVX512) at lower clock speeds. So `pyshbench_perf` might not be helpful if one of the versions you are comparing uses more vectorized instructions that the other.


