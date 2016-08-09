# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@e8972d3ae13574d16f90521bad6a6fdc30ff12e2](https://github.com/jrevels/julia/commit/e8972d3ae13574d16f90521bad6a6fdc30ff12e2) vs [jrevels/julia@189a60441df73035d49450621f4550f71a212e98](https://github.com/jrevels/julia/commit/189a60441df73035d49450621f4550f71a212e98)

*Triggered By:* [link](https://github.com/jrevels/julia/pull/5#issuecomment-238630144)

*Tag Predicate:* `"string"`

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
Memory: 31.383651733398438 GB (21872.4375 MB free)
Uptime: 6.409718e6 sec
Load Avg:  0.83251953125  0.3662109375  0.16845703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1915722 s          0 s    1286158 s  636161727 s         22 s
#2  3501 MHz    4436106 s          0 s     418920 s  635836103 s          0 s
#3  3501 MHz    1884610 s          0 s     635455 s  638037205 s          3 s
#4  3501 MHz    1482517 s          0 s     542150 s  638668583 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.57
Commit ec15da7 (2016-08-06 08:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21870.75390625 MB free)
Uptime: 6.409807e6 sec
Load Avg:  0.873046875  0.49365234375  0.23193359375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1915734 s          0 s    1286207 s  636170469 s         22 s
#2  3501 MHz    4444455 s          0 s     419040 s  635836474 s          0 s
#3  3501 MHz    1884883 s          0 s     635471 s  638045756 s          3 s
#4  3501 MHz    1482520 s          0 s     542164 s  638677405 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
