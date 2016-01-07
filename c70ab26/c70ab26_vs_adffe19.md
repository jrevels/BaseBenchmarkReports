# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@c70ab26](https://github.com/jrevels/julia/commit/c70ab26bb677c92f0d8e0ae41c3035217a4b111f) vs [JuliaLang/julia@adffe19](https://github.com/JuliaLang/julia/commit/adffe19dfb704444789429bffa51f4e05b386125)

*Tag Predicate:* `"arrays" || "indexing"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2#issuecomment-169505410)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory. Note that it's technically possible
for this JSON data to get out of sync with the below table. This would only happen in case
of a network error during the job, and as such is very unlikely. Just in case, you can always
verify that they are synced up by checking the commit history of both files.

The ratio values in the below table equal `head_result / comparison_result` for each corresponding
metric. Thus, `x < 1.0` would denote an improvement, while `x > 1.0` would denote a regression.
In reality, only results that exceed `1.2` are counted as regressions (a default tolerance of
`0.2` is applied to account for the variance of our test hardware). For convenience, regressions are
marked with an **{R}**.

Definitions for the below benchmarks can be found in [JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl).

| Benchmark ID | time | % of time spent in GC | bytes allocated | number of allocations |
|--------------|------|-----------------------|-----------------|-----------------------|
| `(:sumlinear,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100)` | **3.2 {R}** | 0.36 | 1.13 | 1.17 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.98 | 1.05 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.3 {R}** | 0.4 | **1.27 {R}** | **1.5 {R}** |
| `(:sumvector,"Array{Int64,2}",100000)` | **3.23 {R}** | 0.46 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.83 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.68 {R}** | 0.67 | 1.02 | **1.4 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100000)` | 0.91 | 1.11 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **3.94 {R}** | 0.47 | **1.43 {R}** | **2.0 {R}** |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.61 {R}** | 0.7 | 1.02 | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 1.07 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100)` | 1.07 | 1.12 | 1.06 | **1.5 {R}** |
| `(:sumvector,"Array{Float32,2}",100000)` | **3.97 {R}** | 0.47 | **1.43 {R}** | **2.0 {R}** |
| `(:sumvector,"Array{Float32,2}",100)` | **3.6 {R}** | 0.61 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.08 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **2.85 {R}** | 0.47 | **1.27 {R}** | **1.67 {R}** |
| `(:sumcolon,"Array{Float32,2}",100000)` | 0.95 | 1.12 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",100)` | **1.29 {R}** | 0.9 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **3.23 {R}** | 0.64 | **1.37 {R}** | **1.67 {R}** |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.98 | 1.01 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.23 {R}** | 0.96 | 1.03 | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **3.08 {R}** | 0.48 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.13 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.02 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.54 {R}** | 0.67 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.22 {R}** | 0.99 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **3.73 {R}** | 0.49 | **1.43 {R}** | **2.0 {R}** |
| `(:sumrange,"Array{Int64,2}",100000)` | **3.3 {R}** | 0.4 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.92 | 1.1 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100000)` | 0.88 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.97 | 1.03 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.93 | 1.15 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **3.19 {R}** | 0.4 | **1.3 {R}** | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 0.99 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",100000)` | **3.16 {R}** | 0.4 | **1.3 {R}** | **1.5 {R}** |
| `(:sumrange,"Array{Float32,2}",100)` | **1.51 {R}** | 0.74 | 1.03 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100000)` | **2.78 {R}** | 0.49 | **1.27 {R}** | **1.67 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **2.91 {R}** | 0.61 | **1.37 {R}** | **2.0 {R}** |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 1.03 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.05 | 1.04 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.95 {R}** | 0.61 | 1.03 | **1.4 {R}** |
| `(:sumeach,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.84 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.21 {R}** | 0.91 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **2.89 {R}** | 0.47 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **3.17 {R}** | 0.41 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.98 {R}** | 0.47 | **1.33 {R}** | **1.67 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.95 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **1.27 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **3.03 {R}** | 0.41 | **1.3 {R}** | **1.5 {R}** |
| `(:sumlogical,"Array{Float32,2}",100000)` | **2.85 {R}** | 0.48 | **1.27 {R}** | **1.67 {R}** |
| `(:sumlogical,"Array{Float32,2}",100)` | **1.22 {R}** | 0.99 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.18 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.93 | 1.08 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 0.98 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.12 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.27 {R}** | 0.94 | 1.04 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **2.64 {R}** | 0.51 | **1.27 {R}** | **1.67 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.11 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **2.78 {R}** | 0.49 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.6 {R}** | 0.7 | 1.02 | **1.5 {R}** |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.03 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **3.33 {R}** | 0.7 | **1.43 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.96 | 0.99 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.44 {R}** | 0.76 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **3.43 {R}** | 0.51 | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.92 {R}** | 0.46 | **1.25 {R}** | **1.4 {R}** |
| `(:sumvector,"Array{Int64,2}",100)` | **3.11 {R}** | 0.59 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"Array{Int64,2}",100000)` | 0.89 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.92 | 1.06 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.19 | 1.0 | 1.04 | **1.67 {R}** |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.94 | 1.04 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100)` | 1.11 | 0.97 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.02 | 1.02 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.64 {R}** | 0.53 | **1.25 {R}** | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.03 | 1.06 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.73 {R}** | 0.65 | 1.03 | **1.5 {R}** |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **3.57 {R}** | 0.64 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **1.29 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.74 {R}** | 0.46 | **1.27 {R}** | **1.4 {R}** |
| `(:sumvector,"BitArray{2}",100000)` | **1.34 {R}** | 1.03 | **1.37 {R}** | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.82 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.11 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int64,2}",100)` | **1.46 {R}** | 0.79 | 1.02 | **1.5 {R}** |
| `(:sumlinear,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.42 {R}** | 0.73 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",100000)` | 0.67 | **1.43 {R}** | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.26 {R}** | 0.96 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.04 | 1.02 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.6 {R}** | 0.51 | **1.25 {R}** | **1.5 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.08 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100)` | 1.18 | 1.01 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.19 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.86 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",100)` | **1.34 {R}** | 1.11 | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.75 {R}** | 0.64 | 1.03 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.23 {R}** | 0.43 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **1.31 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.98 | 1.14 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100000)` | **1.23 {R}** | 0.99 | **1.25 {R}** | **1.4 {R}** |
| `(:sumcolon,"BitArray{2}",100)` | **2.89 {R}** | 0.36 | 0.91 | 0.75 |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **2.92 {R}** | 0.58 | **1.33 {R}** | **1.67 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.97 | 1.04 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100000)` | 1.07 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.38 {R}** | 0.8 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **3.06 {R}** | 0.59 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 1.19 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.26 {R}** | 0.96 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.21 {R}** | 0.93 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100000)` | **1.23 {R}** | 1.06 | **1.23 {R}** | **1.5 {R}** |

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
Memory: 31.383678436279297 GB (1043.41796875 MB free)
Uptime: 8.561062e6 sec
Load Avg:  1.005859375  1.0146484375  1.19873046875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15571474 s      15323 s   21145106 s  815309063 s          7 s
#2  3501 MHz   14635579 s      15834 s   17147340 s  822264210 s          2 s
#3  3501 MHz   14470806 s      14352 s   17340434 s  822416778 s          1 s
#4  3501 MHz   14146281 s      10292 s   16690737 s  823419335 s          0 s
#5  3501 MHz   14291665 s     149109 s   14666450 s  826255594 s          0 s
#6  3501 MHz   14105929 s      99529 s   12292737 s  829043525 s          0 s
#7  3501 MHz   14292405 s     103068 s   13136938 s  827957756 s          0 s
#8  3501 MHz   14355141 s      57184 s   13160820 s  827832823 s          0 s

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
Memory: 31.383678436279297 GB (958.51171875 MB free)
Uptime: 8.56548e6 sec
Load Avg:  1.02197265625  1.0  1.130859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15637272 s      15323 s   21154161 s  815655032 s          7 s
#2  3501 MHz   14699246 s      15834 s   17157012 s  822604637 s          2 s
#3  3501 MHz   14528326 s      14352 s   17348871 s  822769940 s          1 s
#4  3501 MHz   14198276 s      10338 s   16698348 s  823784725 s          0 s
#5  3501 MHz   14344336 s     149109 s   14675846 s  826629209 s          0 s
#6  3501 MHz   14126884 s      99631 s   12298944 s  829452640 s          0 s
#7  3501 MHz   14312466 s     103228 s   13143212 s  828364429 s          0 s
#8  3501 MHz   14378620 s      57288 s   13166462 s  828238396 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

