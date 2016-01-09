# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@c70ab26](https://github.com/jrevels/julia/commit/c70ab26bb677c92f0d8e0ae41c3035217a4b111f) vs [JuliaLang/julia@adffe19](https://github.com/JuliaLang/julia/commit/adffe19dfb704444789429bffa51f4e05b386125)

*Tag Predicate:* `"linalg"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2#issuecomment-170158142)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory.

The ratio values in the below table equal `head_result / comparison_result` for each corresponding
metric. Thus, `x < 1.0` would denote an improvement, while `x > 1.0` would denote a regression.
In reality, only results that exceed `1.2` are counted as regressions (a default tolerance of
`0.2` is applied to account for the variance of our test hardware). For convenience, regressions are
marked with an **{R}**.

Definitions for the below benchmarks can be found in [JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl).

| Benchmark ID | time | % of time spent in GC | bytes allocated | number of allocations |
|--------------|------|-----------------------|-----------------|-----------------------|
| `(:svdfact,256)` | 0.99 | 1.05 | 1.0 | 1.0 |
| `(:gemv,64)` | 0.99 | 1.06 | 1.0 | 1.0 |
| `(:hermeig,1024)` | 1.04 | 0.97 | 1.0 | 1.0 |
| `(:realeig,1024)` | 1.03 | 1.14 | 1.0 | 0.93 |
| `(:hermeig,256)` | 0.94 | 0.89 | 1.0 | 1.0 |
| `(:qrfact,1024)` | 1.03 | 1.03 | 1.0 | 1.0 |
| `(:lucompletepivSub!,500)` | 0.98 | 0.93 | 1.0 | 1.01 |
| `(:axpy!,16)` | 1.13 | 1.0 | 1.0 | 1.0 |
| `(:lufact,16)` | 0.99 | 0.99 | 0.97 | 1.0 |
| `(:cholfact,16)` | 0.76 | 0.94 | 0.82 | 0.45 |
| `(:axpy!,4)` | **1.2 {R}** | 1.0 | 1.0 | 1.0 |
| `(:cholfact,4)` | 0.41 | 0.87 | 0.38 | 0.45 |
| `(:realeig,256)` | 0.97 | 1.01 | 0.98 | 0.98 |
| `(:lufact,4)` | 0.99 | 0.84 | 0.86 | 1.0 |
| `(:qrfact,256)` | 1.01 | **1.31 {R}** | 1.0 | 1.0 |
| `(:axpy!,64)` | 1.12 | 1.0 | 1.0 | 1.0 |
| `(:lufact,64)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:cholfact,64)` | 0.95 | 1.0 | 0.99 | 0.5 |
| `(:A_mul_B!,1024)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:svdfact,16)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:svdfact,4)` | 1.04 | 1.0 | 0.98 | 1.0 |
| `(:lucompletepivSub!,1000)` | 1.1 | 1.02 | 1.0 | 1.0 |
| `(:A_mul_B!,256)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:lucompletepivCopy!,250)` | 1.01 | 1.04 | 1.0 | **1.34 {R}** |
| `(:svdfact,64)` | 1.0 | 1.07 | 1.0 | 1.0 |
| `(:hermeig,16)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:schurfact,1024)` | 1.05 | 1.02 | 1.0 | 1.0 |
| `(:hermeig,4)` | 1.02 | 1.0 | 0.99 | 1.0 |
| `(:lucompletepivCopy!,100)` | 1.13 | 1.03 | 1.0 | **1.35 {R}** |
| `(:realeig,16)` | **1.32 {R}** | 1.01 | 0.93 | 1.07 |
| `(:qrfact,16)` | 0.99 | 1.0 | 0.99 | 1.0 |
| `(:realeig,4)` | 0.94 | 1.0 | 0.72 | 0.62 |
| `(:hermeig,64)` | 0.99 | 1.05 | 1.0 | 1.0 |
| `(:schurfact,256)` | 1.0 | 0.9 | 1.0 | 1.0 |
| `(:qrfact,4)` | 1.01 | 1.0 | 0.92 | 1.0 |
| `(:dot,1024)` | 0.95 | **Inf {R}** | 1.0 | 1.0 |
| `(:symeig,1024)` | 1.02 | 0.99 | 1.0 | 1.0 |
| `(:realeig,64)` | 0.94 | 0.46 | 0.95 | 1.0 |
| `(:qrfact,64)` | 0.94 | 0.0 | 1.0 | 1.0 |
| `(:A_mul_B!,16)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:dot,256)` | 0.98 | 1.09 | 1.0 | 1.0 |
| `(:symeig,256)` | 0.98 | 1.06 | 1.0 | 1.0 |
| `(:A_mul_B!,4)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:gemv,1024)` | 0.93 | 1.0 | 1.0 | 1.0 |
| `(:A_mul_B!,64)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:gemv,256)` | 0.89 | 1.17 | 1.0 | 1.0 |
| `(:schurfact,16)` | 0.85 | **Inf {R}** | 1.0 | 1.0 |
| `(:lucompletepivCopy!,500)` | 0.99 | 1.01 | 1.0 | **1.34 {R}** |
| `(:schurfact,4)` | 1.15 | 1.0 | 1.01 | 1.05 |
| `(:lucompletepivSub!,250)` | 0.99 | 1.02 | 1.0 | 0.99 |
| `(:schurfact,64)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:dot,16)` | 0.47 | **5.47 {R}** | 1.0 | 1.0 |
| `(:symeig,16)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:axpy!,1024)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:lucompletepivSub!,100)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:lufact,1024)` | 1.02 | 1.09 | 1.0 | 1.0 |
| `(:dot,4)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:cholfact,1024)` | 1.09 | 0.9 | 1.0 | 0.5 |
| `(:symeig,4)` | 1.05 | 1.0 | 0.98 | 1.0 |
| `(:lucompletepivCopy!,1000)` | 1.05 | 1.05 | 1.0 | **1.28 {R}** |
| `(:dot,64)` | 1.01 | 0.99 | 1.0 | 1.0 |
| `(:cholfact,256)` | 1.05 | **1.56 {R}** | 1.0 | 0.5 |
| `(:axpy!,256)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:symeig,64)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:lufact,256)` | 0.98 | 0.95 | 1.0 | 1.0 |
| `(:gemv,16)` | 1.05 | 0.94 | 1.0 | 1.0 |
| `(:svdfact,1024)` | 1.03 | 1.07 | 1.0 | 1.0 |
| `(:gemv,4)` | 1.0 | 1.01 | 1.0 | 1.0 |

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev
Commit c70ab26 (2016-01-04 02:04 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (1032.73828125 MB free)
Uptime: 8.671674e6 sec
Load Avg:  5.720703125  3.30810546875  2.25439453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15698517 s      16288 s   21210452 s  826043364 s          7 s
#2  3501 MHz   14768620 s      16164 s   17205248 s  832988261 s          2 s
#3  3501 MHz   14597616 s      14589 s   17394283 s  833169450 s          1 s
#4  3501 MHz   14258646 s      10538 s   16743112 s  834196896 s          0 s
#5  3501 MHz   14394128 s     151302 s   14701020 s  837123410 s          0 s
#6  3501 MHz   14153367 s     103771 s   12323366 s  839980407 s          0 s
#7  3501 MHz   14339394 s     106558 s   13168950 s  838887652 s          0 s
#8  3501 MHz   14403337 s      58683 s   13190320 s  838771173 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.3-pre+6
Commit adffe19 (2015-12-11 00:38 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (980.23828125 MB free)
Uptime: 8.675853e6 sec
Load Avg:  4.1494140625  2.79931640625  1.91357421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15754986 s      16288 s   21227172 s  826367045 s          8 s
#2  3501 MHz   14851876 s      16164 s   17223658 s  833276283 s          2 s
#3  3501 MHz   14655708 s      14806 s   17412568 s  833487639 s          1 s
#4  3501 MHz   14322397 s      10538 s   16758785 s  834520760 s          0 s
#5  3501 MHz   14423325 s     151401 s   14717332 s  837488946 s          0 s
#6  3501 MHz   14176572 s     103886 s   12339518 s  840352430 s          0 s
#7  3501 MHz   14366501 s     106558 s   13183259 s  839256093 s          0 s
#8  3501 MHz   14427389 s      58683 s   13205264 s  839144762 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

