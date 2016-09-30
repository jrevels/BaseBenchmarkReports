# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@234b24e5248c798222de97d4a505397ba764feaf](https://github.com/jrevels/julia/commit/234b24e5248c798222de97d4a505397ba764feaf) vs [jrevels/julia@0287a9971ea4d740d2bc5e205423e2ae5bdf4124](https://github.com/jrevels/julia/commit/0287a9971ea4d740d2bc5e205423e2ae5bdf4124)

*Triggered By:* [link](https://github.com/jrevels/julia/pull/6#issuecomment-250840453)

*Tag Predicate:* `"factorization"`

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
| `["linalg","factorization",("chol","Matrix",1024)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("chol","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("cholfact","Matrix",1024)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("cholfact","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.83 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Diagonal",1024)]` | 1.05 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Diagonal",256)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","LowerTriangular",1024)]` | 0.98 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","LowerTriangular",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.03 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eig","UpperTriangular",1024)]` | 0.96 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","UpperTriangular",256)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.89 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Diagonal",1024)]` | 1.05 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 1.16 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","LowerTriangular",1024)]` | 0.97 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","LowerTriangular",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.03 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 0.99 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","UpperTriangular",1024)]` | 0.97 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","UpperTriangular",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Matrix",1024)]` | 0.94 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Matrix",256)]` | 1.02 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 0.78 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 0.99 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Matrix",1024)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 1.06 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 1.09 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("qr","Matrix",1024)]` | 0.98 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("qr","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("qrfact","Matrix",1024)]` | 1.04 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("qrfact","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 1.03 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Bidiagonal",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.74 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.04 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","LowerTriangular",1024)]` | 1.02 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","LowerTriangular",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Matrix",1024)]` | 1.10 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","UpperTriangular",1024)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","UpperTriangular",256)]` | 1.00 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Bidiagonal",1024)]` | 0.97 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Bidiagonal",256)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.78 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.04 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","LowerTriangular",1024)]` | 1.06 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","LowerTriangular",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Matrix",1024)]` | 1.01 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Matrix",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","UpperTriangular",1024)]` | 0.99 (0%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","UpperTriangular",256)]` | 1.00 (0%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.813
Commit 0287a99 (2016-09-28 04:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19432.1015625 MB free)
Uptime: 1.0911894e7 sec
Load Avg:  0.974609375  0.52783203125  0.29638671875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2391223 s          0 s    2165852 s  1083866380 s         35 s
#2  3501 MHz    9107901 s          0 s     814410 s  1080712732 s          2 s
#3  3501 MHz    2466131 s          0 s     971870 s  1087099076 s          5 s
#4  3501 MHz    1996546 s          0 s     797446 s  1087969313 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.813
Commit 0287a99 (2016-09-28 04:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (19429.84765625 MB free)
Uptime: 1.091208e7 sec
Load Avg:  1.0029296875  0.7548828125  0.427734375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    2391242 s          0 s    2165932 s  1083884794 s         35 s
#2  3501 MHz    9126056 s          0 s     814465 s  1080713103 s          2 s
#3  3501 MHz    2466390 s          0 s     971889 s  1087117379 s          5 s
#4  3501 MHz    1996562 s          0 s     797456 s  1087987869 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
