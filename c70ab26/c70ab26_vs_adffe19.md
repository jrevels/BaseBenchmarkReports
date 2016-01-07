# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@c70ab26](https://github.com/jrevels/julia/commit/c70ab26bb677c92f0d8e0ae41c3035217a4b111f) vs [JuliaLang/julia@adffe19](https://github.com/JuliaLang/julia/commit/adffe19dfb704444789429bffa51f4e05b386125)

*Executed On Merge Commit?* true

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
| `(:sumlinear,"Array{Float32,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.95 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100)` | **2.76 {R}** | 0.41 | 1.13 | 1.17 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.97 | 1.01 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.07 {R}** | 0.45 | **1.27 {R}** | **1.5 {R}** |
| `(:sumvector,"Array{Int64,2}",100000)` | **3.01 {R}** | 0.47 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.82 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int64,2}",100)` | 0.79 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.68 {R}** | 0.62 | 1.02 | **1.4 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100000)` | 0.94 | 1.11 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **3.77 {R}** | 0.49 | **1.43 {R}** | **2.0 {R}** |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.54 {R}** | 0.68 | 1.02 | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.04 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100)` | 1.11 | 1.0 | 1.06 | **1.5 {R}** |
| `(:sumvector,"Array{Float32,2}",100000)` | **3.74 {R}** | 0.49 | **1.43 {R}** | **2.0 {R}** |
| `(:sumvector,"Array{Float32,2}",100)` | **3.38 {R}** | 0.65 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.02 | 1.01 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **2.62 {R}** | 0.54 | **1.27 {R}** | **1.67 {R}** |
| `(:sumcolon,"Array{Float32,2}",100000)` | 1.0 | 1.03 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",100)` | 1.17 | 0.87 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **3.1 {R}** | 0.71 | **1.37 {R}** | **1.67 {R}** |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.96 | 1.05 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.33 {R}** | 0.84 | 1.03 | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **2.91 {R}** | 0.5 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.95 | 0.97 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.61 {R}** | 0.58 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.32 {R}** | 0.84 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **3.61 {R}** | 0.51 | **1.43 {R}** | **2.0 {R}** |
| `(:sumrange,"Array{Int64,2}",100000)` | **3.15 {R}** | 0.44 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.94 | 1.13 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100000)` | 1.11 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.95 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.95 | 1.05 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.96 | 1.08 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **2.92 {R}** | 0.44 | **1.3 {R}** | **1.5 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.02 | 0.94 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",100000)` | **2.94 {R}** | 0.44 | **1.3 {R}** | **1.5 {R}** |
| `(:sumrange,"Array{Float32,2}",100)` | **1.47 {R}** | 0.75 | 1.03 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100000)` | **2.62 {R}** | 0.53 | **1.27 {R}** | **1.67 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **2.82 {R}** | 0.63 | **1.37 {R}** | **2.0 {R}** |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.96 | 1.08 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.97 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.8 {R}** | 0.61 | 1.03 | **1.4 {R}** |
| `(:sumeach,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.79 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.25 {R}** | 0.91 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | **2.63 {R}** | 0.52 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **3.53 {R}** | 0.42 | **1.27 {R}** | **1.5 {R}** |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.05 | 0.99 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.85 {R}** | 0.48 | **1.33 {R}** | **1.67 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **2.82 {R}** | 0.45 | **1.3 {R}** | **1.5 {R}** |
| `(:sumlogical,"Array{Float32,2}",100000)` | **2.59 {R}** | 0.52 | **1.27 {R}** | **1.67 {R}** |
| `(:sumlogical,"Array{Float32,2}",100)` | **1.34 {R}** | 0.82 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.96 | 1.09 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 0.98 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.03 | 0.98 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | **1.38 {R}** | 0.77 | 1.04 | **1.5 {R}** |
| `(:sumelt,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.88 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | **2.49 {R}** | 0.56 | **1.27 {R}** | **1.67 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.78 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | **2.54 {R}** | 0.54 | **1.27 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.54 {R}** | 0.67 | 1.02 | **1.5 {R}** |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.03 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.01 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **3.17 {R}** | 0.69 | **1.43 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.74 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.92 | 1.02 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100000)` | 1.17 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.37 {R}** | 0.74 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **3.37 {R}** | 0.52 | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.78 {R}** | 0.52 | **1.25 {R}** | **1.4 {R}** |
| `(:sumvector,"Array{Int64,2}",100)` | **2.98 {R}** | 0.59 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"Array{Int64,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.93 | 1.02 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | **1.31 {R}** | 0.87 | 1.04 | **1.67 {R}** |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.92 | 1.05 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100)` | 1.06 | 0.97 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.96 | 1.05 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | **2.54 {R}** | 0.56 | **1.25 {R}** | **1.5 {R}** |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.05 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.7 {R}** | 0.64 | 1.03 | **1.5 {R}** |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.94 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **3.41 {R}** | 0.69 | **1.43 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.06 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.65 {R}** | 0.48 | **1.27 {R}** | **1.4 {R}** |
| `(:sumvector,"BitArray{2}",100000)` | 1.17 | **1.21 {R}** | **1.37 {R}** | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.83 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.11 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int64,2}",100)` | **1.38 {R}** | 0.77 | 1.02 | **1.5 {R}** |
| `(:sumlinear,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.43 {R}** | 0.71 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.07 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",100000)` | 0.53 | **1.78 {R}** | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | **1.37 {R}** | 0.8 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 0.97 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | **2.47 {R}** | 0.53 | **1.25 {R}** | **1.5 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.07 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100)` | **1.28 {R}** | 0.87 | 1.04 | **1.67 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.19 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.83 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",100)` | 1.15 | **1.25 {R}** | **1.37 {R}** | **1.67 {R}** |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.71 {R}** | 0.64 | 1.03 | **1.5 {R}** |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | **3.08 {R}** | 0.46 | **1.37 {R}** | **2.0 {R}** |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 1.06 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.04 | 1.01 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100000)` | 1.01 | **1.24 {R}** | **1.25 {R}** | **1.4 {R}** |
| `(:sumcolon,"BitArray{2}",100)` | **2.38 {R}** | 0.38 | 0.91 | 0.75 |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.1 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **2.77 {R}** | 0.63 | **1.33 {R}** | **1.67 {R}** |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.99 | 1.06 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | **1.31 {R}** | 0.73 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **2.96 {R}** | 0.61 | **1.37 {R}** | **2.0 {R}** |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 1.02 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | **1.37 {R}** | 0.77 | 1.04 | **1.67 {R}** |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.19 | 0.77 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100000)` | 1.12 | 1.14 | **1.23 {R}** | **1.5 {R}** |

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
Memory: 31.383678436279297 GB (28771.43359375 MB free)
Uptime: 8.511232e6 sec
Load Avg:  1.0029296875  1.0146484375  1.3876953125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1   800 MHz   79967432 s        216 s   14750843 s  754364531 s         14 s
#2   800 MHz   12464775 s        148 s    7290480 s  830461264 s          0 s
#3  3501 MHz    8601600 s        888 s    6895742 s  834787284 s          0 s
#4   800 MHz    7638144 s        518 s    7044176 s  835569453 s          0 s
#5  1200 MHz    8636373 s        969 s    7730443 s  834611553 s          0 s
#6  3501 MHz    5055798 s        609 s    7574564 s  838404051 s          0 s
#7   800 MHz    4103762 s       2516 s    7379615 s  839484642 s          0 s
#8  3501 MHz    3099107 s       1602 s    7403074 s  840533804 s          0 s

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
Memory: 31.383678436279297 GB (28609.7421875 MB free)
Uptime: 8.515287e6 sec
Load Avg:  0.9970703125  0.994140625  1.19091796875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1   800 MHz   80055289 s        216 s   14762579 s  754648640 s         14 s
#2   800 MHz   12532027 s        148 s    7300388 s  830760123 s          0 s
#3   800 MHz    8661995 s        888 s    6903317 s  835111141 s          0 s
#4   800 MHz    7695585 s        518 s    7050852 s  835900089 s          0 s
#5  1800 MHz    8672959 s        969 s    7737487 s  834968674 s          0 s
#6  3501 MHz    5076798 s        609 s    7580986 s  838775506 s          0 s
#7  3501 MHz    4125051 s       2516 s    7386035 s  839858411 s          0 s
#8   800 MHz    3118702 s       1602 s    7408082 s  840909106 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

