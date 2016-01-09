# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@c70ab26](https://github.com/jrevels/julia/commit/c70ab26bb677c92f0d8e0ae41c3035217a4b111f) vs [JuliaLang/julia@adffe19](https://github.com/JuliaLang/julia/commit/adffe19dfb704444789429bffa51f4e05b386125)

*Tag Predicate:* `"array" && "indexing"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2#issuecomment-170157999)

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
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.98 | 0.96 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | **1.36 {R}** | 0.97 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | 1.01 | 1.02 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | **2.63 {R}** | 0.52 | **1.27 {R}** | **1.38 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | **1.3 {R}** | 0.96 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | **1.66 {R}** | 0.92 | 1.03 | **1.4 {R}** |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.72 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"Array{Float32,2}",(3,5))` | **2.37 {R}** | 0.63 | **1.34 {R}** | **1.77 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | 0.98 | 1.05 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int32,2}",(300,500))` | 1.15 | **1.4 {R}** | 1.04 | **1.66 {R}** |
| `(:sumrange,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.96 | 1.05 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",(300,500))` | 1.09 | 0.99 | 1.06 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | **2.41 {R}** | 0.61 | **1.34 {R}** | **1.77 {R}** |
| `(:sumlinear,"BitArray{2}",(3,5))` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",(3,5))` | 0.9 | 1.14 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | **2.42 {R}** | 0.6 | **1.35 {R}** | **1.83 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | 0.89 | 1.14 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | **1.94 {R}** | 0.72 | **1.21 {R}** | **1.38 {R}** |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | **1.2 {R}** | 0.96 | 1.04 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | **1.66 {R}** | 1.0 | **1.43 {R}** | **2.0 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int32,2}",(3,5))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | 0.87 | 1.14 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | **1.72 {R}** | **1.22 {R}** | 1.03 | **1.5 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | **1.26 {R}** | 0.95 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.92 | 1.05 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",(300,500))` | 0.95 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",(3,5))` | **1.52 {R}** | 1.01 | **1.31 {R}** | **1.59 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",(3,5))` | **2.97 {R}** | 0.48 | **1.29 {R}** | **1.48 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | 0.7 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",(3,5))` | 1.05 | 0.94 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | **2.83 {R}** | 0.48 | **1.29 {R}** | **1.48 {R}** |
| `(:sumelt,"Array{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | 1.19 | 0.98 | 1.04 | **1.66 {R}** |
| `(:sumvector,"Array{Int32,2}",(3,5))` | **2.48 {R}** | 0.62 | **1.35 {R}** | **1.83 {R}** |
| `(:sumeach,"Array{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | **3.74 {R}** | 0.38 | **1.3 {R}** | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | **1.7 {R}** | **1.22 {R}** | 1.03 | **1.5 {R}** |
| `(:sumcolon,"Array{Int32,2}",(3,5))` | 0.9 | 1.09 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int32,2}",(300,500))` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",(300,500))` | 0.68 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Float32,2}",(3,5))` | **2.05 {R}** | 0.72 | **1.22 {R}** | **1.48 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | **3.05 {R}** | 1.0 | **1.43 {R}** | **2.0 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | 0.95 | 1.03 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | **2.02 {R}** | 0.74 | **1.22 {R}** | **1.48 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | 1.19 | 0.95 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | 0.95 | **Inf {R}** | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | **2.23 {R}** | 0.63 | **1.31 {R}** | **1.59 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | 1.09 | 0.99 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",(3,5))` | **1.36 {R}** | 1.0 | **1.25 {R}** | **1.4 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | 1.08 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | **1.76 {R}** | 0.82 | **1.23 {R}** | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | 1.18 | 0.97 | 1.04 | **1.66 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | 0.91 | 1.09 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.97 | 1.01 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.96 | 1.04 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | **1.82 {R}** | 0.18 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int32,2}",(3,5))` | **3.95 {R}** | 0.35 | **1.3 {R}** | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.96 | 1.03 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | 0.83 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",(3,5))` | **1.25 {R}** | 0.98 | 1.2 | **1.4 {R}** |
| `(:sumelt,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | **2.48 {R}** | 0.59 | **1.34 {R}** | **1.77 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | **1.54 {R}** | 0.92 | 1.03 | **1.5 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | 0.96 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | **2.61 {R}** | 0.52 | **1.27 {R}** | **1.4 {R}** |
| `(:sumeach,"Array{Float32,2}",(3,5))` | 0.97 | 1.01 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int32,2}",(3,5))` | **1.81 {R}** | 0.8 | **1.23 {R}** | **1.5 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.93 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.97 | 0.96 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | 1.06 | 0.95 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | 0.87 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",(3,5))` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | **1.2 {R}** | 0.96 | 1.04 | **1.66 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | 1.05 | 1.01 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",(3,5))` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | **1.73 {R}** | 0.83 | **1.21 {R}** | **1.4 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | **2.48 {R}** | 0.63 | **1.35 {R}** | **1.83 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | **2.96 {R}** | 0.48 | **1.29 {R}** | **1.48 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | **2.1 {R}** | 0.0 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | 0.94 | 1.06 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.02 | 0.99 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"Array{Float32,2}",(300,500))` | **3.38 {R}** | 1.0 | **1.43 {R}** | **2.0 {R}** |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.95 | 1.03 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",(3,5))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(3,5))` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | **1.21 {R}** | 0.95 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(300,500))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.98 | 0.99 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.97 | 0.99 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | **1.55 {R}** | 1.0 | **1.37 {R}** | **1.67 {R}** |
| `(:sumcartesian,"BitArray{2}",(3,5))` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",(300,500))` | 1.17 | 0.99 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | 0.95 | 0.57 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int32,2}",(3,5))` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | **1.64 {R}** | 0.92 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | **2.07 {R}** | 0.71 | **1.22 {R}** | **1.48 {R}** |
| `(:sumlinear,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.92 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BitArray{2}",(3,5))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int32,2}",(3,5))` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"Array{Int32,2}",(300,500))` | **3.89 {R}** | **Inf {R}** | **1.43 {R}** | **2.0 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | **3.02 {R}** | 0.46 | **1.3 {R}** | **1.5 {R}** |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 1.0 | **1.24 {R}** | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",(300,500))` | **1.62 {R}** | 1.0 | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | **1.56 {R}** | 0.93 | 1.03 | **1.5 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | 0.93 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int32,2}",(300,500))` | 1.13 | 0.96 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int32,2}",(3,5))` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.96 | 1.01 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",(300,500))` | **3.62 {R}** | **Inf {R}** | 0.91 | 0.75 |
| `(:sumrange,"Array{Float32,2}",(300,500))` | **1.39 {R}** | 0.95 | 1.03 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | **2.39 {R}** | 0.6 | **1.31 {R}** | **1.56 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(300,500))` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | **1.94 {R}** | **Inf {R}** | **1.37 {R}** | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | **1.74 {R}** | 0.91 | 1.03 | **1.4 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(300,500))` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(3,5))` | 0.93 | 1.08 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}",(3,5))` | **1.85 {R}** | 0.79 | **1.23 {R}** | **1.5 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(300,500))` | **1.56 {R}** | 0.93 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.97 | 1.03 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Float32,2}",(3,5))` | 1.08 | 0.93 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}",(300,500))` | 1.18 | 0.97 | 1.04 | **1.66 {R}** |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.9 | 1.09 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}",(3,5))` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(300,500))` | 0.99 | **1.25 {R}** | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",(3,5))` | 0.96 | 1.03 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Float32,2}",(300,500))` | 1.1 | 0.96 | 1.04 | **1.66 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",(3,5))` | 1.06 | 0.97 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",(3,5))` | 1.0 | 1.1 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int32,2}",(300,500))` | **1.36 {R}** | 0.95 | 1.03 | **1.5 {R}** |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",(300,500))` | **1.22 {R}** | 0.97 | 1.04 | **1.5 {R}** |
| `(:sumrange,"BitArray{2}",(300,500))` | **3.74 {R}** | **Inf {R}** | 1.13 | 1.17 |

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
Memory: 31.383678436279297 GB (26598.0078125 MB free)
Uptime: 8.672033e6 sec
Load Avg:  2.06103515625  2.341796875  2.0185546875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1249443 s        488 s    1792458 s  861554389 s          1 s
#2  3501 MHz     761772 s        146 s     529720 s  865396882 s          0 s
#3  3501 MHz     812013 s       1244 s     600968 s  865370952 s          0 s
#4  3501 MHz     356407 s        126 s     532308 s  865917073 s          0 s
#5  3501 MHz     326678 s       2937 s      97742 s  866727331 s          0 s
#6  3501 MHz     194829 s       1095 s      91496 s  866874037 s          0 s
#7  3501 MHz     353176 s        623 s     128993 s  866650730 s          0 s
#8  3501 MHz     185863 s        588 s      83196 s  866894343 s          0 s

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
Memory: 31.383678436279297 GB (26540.984375 MB free)
Uptime: 8.677138e6 sec
Load Avg:  1.859375  2.36572265625  1.986328125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1313361 s        488 s    1820593 s  861951856 s          1 s
#2  3501 MHz     882487 s        146 s     552536 s  865735190 s          0 s
#3  3501 MHz     881537 s       1244 s     629469 s  865765420 s          0 s
#4  3501 MHz     469555 s        126 s     547660 s  866287814 s          0 s
#5  3501 MHz     348343 s       2937 s     124918 s  867184644 s          0 s
#6  3501 MHz     216114 s       1095 s     118604 s  867331115 s          0 s
#7  3501 MHz     374768 s        623 s     155870 s  867104673 s          0 s
#8  3501 MHz     205560 s        588 s     109232 s  867353352 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

