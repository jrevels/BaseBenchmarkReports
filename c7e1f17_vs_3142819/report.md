# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@c7e1f179cd0a3924019e96ee0857cd805531755e](https://github.com/jrevels/julia/commit/c7e1f179cd0a3924019e96ee0857cd805531755e) vs [jrevels/julia@3142819516da68d5d928bf66456ad633bc53c915](https://github.com/jrevels/julia/commit/3142819516da68d5d928bf66456ad633bc53c915)

*Triggered By:* [link](https://github.com/jrevels/julia/pull/5#issuecomment-224360284)

*Tag Predicate:* `"array" && !"linalg"`

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

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4565
Commit c7e1f17 (2016-06-07 17:50 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28214.9140625 MB free)
Uptime: 979456.0 sec
Load Avg:  0.9970703125  1.0146484375  0.9833984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     847830 s          0 s     246769 s   96601947 s          3 s
#2  3501 MHz    1226220 s          0 s     101266 s   96559546 s          0 s
#3  3501 MHz     458715 s          0 s     102676 s   97330134 s          0 s
#4  3501 MHz     332904 s          0 s      82972 s   97494601 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4563
Commit 3142819 (2016-06-06 22:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28129.3125 MB free)
Uptime: 983030.0 sec
Load Avg:  0.9970703125  0.96923828125  0.94970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     954169 s          0 s     256155 s   96842694 s          3 s
#2  3501 MHz    1352453 s          0 s     109573 s   96782045 s          0 s
#3  3501 MHz     515532 s          0 s     108393 s   97624289 s          0 s
#4  3501 MHz     371836 s          0 s      88177 s   97807365 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
