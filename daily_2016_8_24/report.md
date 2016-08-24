# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@3e65d68f23bd7e26cdff11e437b22ee7db494906](https://github.com/jrevels/julia/commit/3e65d68f23bd7e26cdff11e437b22ee7db494906)

*Triggered By:* [link](https://github.com/jrevels/julia/commit/3e65d68f23bd7e26cdff11e437b22ee7db494906#commitcomment-18764011)

*Tag Predicate:* `"string"`

*Daily Job:* 2016-08-24

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

| ID | time | GC time | memory | allocations |
|----|------|---------|--------|-------------|
| `["io","read","read"]` | 6.86 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["io","read","readstring"]` | 28.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["problem","spellcheck","spellcheck"]` | 9.00 s (15%) | 1.57 s | 5.50 gb (1%) | 111879414 |
| `["string","join"]` | 104.68 ms (40%) | 36.30 ms | 128.99 mb (1%) | 20 |
| `["string","replace"]` | 146.11 μs (15%) | 0.00 ns | 12.11 kb (1%) | 6 |

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
Memory: 31.383651733398438 GB (23813.72265625 MB free)
Uptime: 7.70699e6 sec
Load Avg:  0.775390625  0.3232421875  0.20947265625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1919246 s          0 s    1544040 s  765288719 s         25 s
#2  3501 MHz    4503915 s          0 s     520292 s  765311038 s          1 s
#3  3501 MHz    1887998 s          0 s     716442 s  767616176 s          3 s
#4  3501 MHz    1484899 s          0 s     576789 s  768327341 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
