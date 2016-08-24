# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@3e65d68f23bd7e26cdff11e437b22ee7db494906](https://github.com/jrevels/julia/commit/3e65d68f23bd7e26cdff11e437b22ee7db494906)

*Triggered By:* [link](https://github.com/jrevels/julia/commit/3e65d68f23bd7e26cdff11e437b22ee7db494906#commitcomment-18764212)

*Tag Predicate:* `"string"`

*Daily Job:* 2016-08-24 vs 2016-08-23

## Results

*Note: If Chrome is your browser, I strongly recommend installing the [Wide GitHub](https://chrome.google.com/webstore/detail/wide-github/kaalofacklcidaampbokdplbklpeldpj?hl=en)
extension, which makes the result table easier to read.*

Below is a table of this job's results, obtained by running the benchmarks found in
[JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl). The values
listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`,
and can be used to index into the BaseBenchmarks suite to retrieve the corresponding
benchmarks.

The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.

A ratio greater than `1.0` denotes a possible regression (marked with :x:), while a ratio less
than `1.0` denotes a possible improvement (marked with :white_check_mark:). Only significant results - results
that indicate possible regressions or improvements - are shown below (thus, an empty table means that all
benchmark results remained invariant between builds).

| ID | time ratio | memory ratio |
|----|------------|--------------|
| `["string","join"]` | 1.54 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["io","read"]`
- `["problem","spellcheck"]`
- `["string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.57
Commit ec15da7 (2016-08-06 08:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (23819.2734375 MB free)
Uptime: 7.707705e6 sec
Load Avg:  0.806640625  0.3212890625  0.2080078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1920664 s          0 s    1544218 s  765358453 s         25 s
#2  3501 MHz    4512218 s          0 s     520396 s  765374123 s          1 s
#3  3501 MHz    1888266 s          0 s     716506 s  767687328 s          3 s
#4  3501 MHz    1484946 s          0 s     576839 s  768398740 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
