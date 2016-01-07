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
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.92 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100)` | **2.86 {R}** | 0.41 | 1.13 | 1.17 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.96 | 1.01 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.07 {R}** | 0.45 | **1.27 {R}** | **1.5 {R}** |
| `(:sumvector,"Array{Int64,2}",100000)` | **2.98 {R}** | 0.49 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.8 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.77 {R}** | 0.62 | 1.02 | **1.4 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100000)` | 0.9 | 1.09 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **3.74 {R}** | 0.49 | **1.43 {R}** | **2.0 {R}** |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.93 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.58 {R}** | 0.67 | 1.02 | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 1.07 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100)` | 0.99 | 1.11 | 1.06 | **1.5 {R}** |
| `(:sumvector,"Array{Float32,2}",100000)` | **3.75 {R}** | 0.49 | **1.43 {R}** | **2.0 {R}** |
| `(:sumvector,"Array{Float32,2}",100)` | **3.41 {R}** | 0.66 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.05 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | **1.3 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **2.49 {R}** | 0.54 | **1.27 {R}** | **1.67 {R}** |
| `(:sumcolon,"Array{Float32,2}",100000)` | 0.96 | 1.09 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",100)` | 1.18 | 0.83 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **3.16 {R}** | 0.7 | **1.37 {R}** | **1.67 {R}** |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.95 | 1.08 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.17 | 0.92 | 1.03 | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **2.79 {R}** | 0.49 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 0.99 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.7 {R}** | 0.58 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.17 | 0.93 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **3.54 {R}** | 0.51 | **1.43 {R}** | **2.0 {R}** |
| `(:sumrange,"Array{Int64,2}",100000)` | **3.07 {R}** | 0.45 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.92 | 1.08 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100000)` | 0.88 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.96 | 1.02 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.94 | 1.09 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **2.9 {R}** | 0.45 | **1.3 {R}** | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.01 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",100000)` | **2.94 {R}** | 0.44 | **1.3 {R}** | **1.5 {R}** |
| `(:sumrange,"Array{Float32,2}",100)` | **1.49 {R}** | 0.73 | 1.03 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100000)` | **2.45 {R}** | 0.56 | **1.27 {R}** | **1.67 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **2.79 {R}** | 0.61 | **1.37 {R}** | **2.0 {R}** |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.94 | 1.05 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 0.99 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.78 {R}** | 0.62 | 1.03 | **1.4 {R}** |
| `(:sumeach,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.83 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.2 | 0.8 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **2.57 {R}** | 0.55 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **3.28 {R}** | 0.44 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.05 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.81 {R}** | 0.47 | **1.33 {R}** | **1.67 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.8 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.73 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **2.84 {R}** | 0.46 | **1.3 {R}** | **1.5 {R}** |
| `(:sumlogical,"Array{Float32,2}",100000)` | **2.55 {R}** | 0.54 | **1.27 {R}** | **1.67 {R}** |
| `(:sumlogical,"Array{Float32,2}",100)` | 1.15 | 0.95 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.93 | 1.07 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 0.99 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.94 | 1.08 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.21 {R}** | 0.92 | 1.04 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **2.36 {R}** | 0.57 | **1.27 {R}** | **1.67 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **2.45 {R}** | 0.57 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.58 {R}** | 0.67 | 1.02 | **1.5 {R}** |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 0.99 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.97 | 1.05 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **3.22 {R}** | 0.69 | **1.43 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.95 | 1.03 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.42 {R}** | 0.7 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **3.33 {R}** | 0.52 | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.73 {R}** | 0.51 | **1.25 {R}** | **1.4 {R}** |
| `(:sumvector,"Array{Int64,2}",100)` | **2.93 {R}** | 0.57 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"Array{Int64,2}",100000)` | 0.77 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.89 | 1.06 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.17 | 0.93 | 1.04 | **1.67 {R}** |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.95 | 1.04 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100)` | 1.05 | 1.06 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.06 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.94 | 1.08 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.43 {R}** | 0.58 | **1.25 {R}** | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.98 | 1.07 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.06 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.76 {R}** | 0.61 | 1.03 | **1.5 {R}** |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **3.45 {R}** | 0.68 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.74 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.61 {R}** | 0.5 | **1.27 {R}** | **1.4 {R}** |
| `(:sumvector,"BitArray{2}",100000)` | 1.12 | **1.3 {R}** | **1.37 {R}** | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.81 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int64,2}",100)` | **1.38 {R}** | 0.79 | 1.02 | **1.5 {R}** |
| `(:sumlinear,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.46 {R}** | 0.69 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",100000)` | 0.67 | **1.46 {R}** | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **1.39 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.19 | 0.93 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.07 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.03 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.39 {R}** | 0.56 | **1.25 {R}** | **1.5 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100)` | 1.13 | 0.96 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.32 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.63 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.86 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",100)` | 1.11 | **1.32 {R}** | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.73 {R}** | 0.63 | 1.03 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.05 {R}** | 0.48 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.75 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.97 | 1.11 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100000)` | **1.3 {R}** | 0.99 | **1.25 {R}** | **1.4 {R}** |
| `(:sumcolon,"BitArray{2}",100)` | **2.46 {R}** | 0.39 | 0.91 | 0.75 |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **2.78 {R}** | 0.6 | **1.33 {R}** | **1.67 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.98 | 1.02 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100000)` | 1.09 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.4 {R}** | 0.7 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **2.99 {R}** | 0.58 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 1.16 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.19 | 0.92 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.21 {R}** | 0.77 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100000)` | 1.1 | 1.18 | **1.23 {R}** | **1.5 {R}** |

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
Memory: 31.383678436279297 GB (26794.87109375 MB free)
Uptime: 8.529842e6 sec
Load Avg:  1.0146484375  1.03173828125  1.19677734375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1060383 s        488 s    1735520 s  847658943 s          1 s
#2  3501 MHz     618184 s        146 s     484250 s  851430521 s          0 s
#3  3501 MHz     692619 s       1228 s     561491 s  851355966 s          0 s
#4  3501 MHz     251211 s        126 s     491754 s  851874492 s          0 s
#5  3501 MHz     272785 s       2937 s      67810 s  852603916 s          0 s
#6  3501 MHz     152254 s       1095 s      59194 s  852743674 s          0 s
#7  3501 MHz     287036 s        567 s     101776 s  852541683 s          0 s
#8  3501 MHz     146376 s        588 s      52466 s  852756193 s          0 s

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
Memory: 31.383678436279297 GB (26636.01171875 MB free)
Uptime: 8.53395e6 sec
Load Avg:  1.0029296875  0.98828125  1.15625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1154672 s        488 s    1745815 s  847947499 s          1 s
#2  3501 MHz     690348 s        146 s     492387 s  851734470 s          0 s
#3  3501 MHz     749066 s       1228 s     567891 s  851683560 s          0 s
#4  3501 MHz     307450 s        126 s     497536 s  852210415 s          0 s
#5  3501 MHz     293998 s       2937 s      73056 s  852984149 s          0 s
#6  3501 MHz     172440 s       1095 s      64593 s  853122458 s          0 s
#7  3501 MHz     307215 s        567 s     107120 s  852919237 s          0 s
#8  3501 MHz     165595 s        588 s      56902 s  853138805 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

