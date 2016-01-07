# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@adffe19](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125) vs [JuliaLang/julia@bb73f34](https://github.com/JuliaLang/julia/commit/bb73f3489d837e3339fce2c1aab283d3b2e97a4c)

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195664)

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
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 0.97 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.98 | 1.02 | 1.0 | 1.0 |
| `(:sumvector,"Array{Int64,2}",100000)` | 0.99 | 0.99 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.04 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int64,2}",100)` | 0.8 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.99 | 1.01 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100000)` | 1.0 | 0.99 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.98 | 1.07 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.08 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.99 | 0.97 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100)` | 1.12 | 0.9 | 1.0 | 1.0 |
| `(:sumvector,"Array{Float32,2}",100000)` | 1.0 | 1.02 | 1.0 | 1.0 |
| `(:sumvector,"Array{Float32,2}",100)` | 1.01 | 1.06 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.9 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 1.02 | 1.02 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",100000)` | 1.01 | 1.01 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Float32,2}",100)` | 0.97 | 0.95 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.02 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.01 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.15 | 0.93 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.95 | 1.03 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.18 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.11 | 0.84 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.03 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int64,2}",100000)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.01 | 0.98 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100000)` | **1.25 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.02 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.98 | 1.02 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",100000)` | 1.01 | 1.01 | 1.0 | 1.0 |
| `(:sumelt,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Float32,2}",100)` | 0.97 | 0.94 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100000)` | 1.0 | 1.04 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 0.97 | 1.05 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.98 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.96 | 0.95 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.97 | 0.94 | 1.0 | 1.0 |
| `(:sumeach,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 0.98 | 1.14 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 0.99 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.0 | 1.02 | 1.0 | 1.0 |
| `(:sumcartesian,"BitArray{2}",100)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.8 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Float32,2}",100000)` | 1.01 | 1.01 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Float32,2}",100)` | 1.16 | 0.84 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.98 | 1.03 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | **1.24 {R}** | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.06 | 0.91 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.16 | 0.87 | 1.0 | 1.0 |
| `(:sumelt,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.87 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.0 | 1.04 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.72 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 0.99 | 1.05 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 0.99 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 0.98 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumeach,"Array{Int64,2}",100000)` | 1.14 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 0.98 | 0.96 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.0 | 1.04 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.98 | 1.04 | 1.0 | 1.0 |
| `(:sumvector,"Array{Int64,2}",100)` | 0.99 | 1.01 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Int64,2}",100000)` | 1.14 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.97 | 1.05 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.12 | 0.83 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"Array{Int64,2}",100)` | 0.99 | 1.03 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.98 | 1.07 | 1.0 | 1.0 |
| `(:sumelt,"Array{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 1.01 | 1.02 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.98 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 0.99 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"Array{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.02 | 1.05 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 0.81 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 0.98 | 1.06 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",100000)` | 1.01 | 1.01 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlinear,"BitArray{2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"Array{Int64,2}",100)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 0.98 | 0.96 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",100000)` | 0.99 | 1.05 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.16 | 0.86 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.01 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}",100000)` | 1.0 | 1.01 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.96 | 1.0 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"Array{Int64,2}",100)` | 1.12 | 0.83 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 0.86 | 1.0 | 1.0 | 1.0 |
| `(:sumcartesian,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.97 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BitArray{2}",100)` | 1.01 | 1.02 | 1.0 | 1.0 |
| `(:sumrange,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 0.96 | 0.95 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 0.99 | 0.99 | 1.0 | 1.0 |
| `(:sumcartesian,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.81 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100)` | 1.08 | 0.98 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int64,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumrange,"BitArray{2}",100000)` | 0.98 | 1.05 | 1.0 | 1.0 |
| `(:sumcolon,"BitArray{2}",100)` | 0.98 | 1.03 | 1.0 | 1.0 |
| `(:sumelt,"SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1}",100000)` | 1.08 | 1.0 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 1.0 | 1.03 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100000)` | 1.0 | 0.96 | 1.0 | 1.0 |
| `(:sumlinear,"Array{Int64,2}",100000)` | 1.03 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100)` | 0.99 | 1.02 | 1.0 | 1.0 |
| `(:sumvector,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 1.0 | 1.04 | 1.0 | 1.0 |
| `(:sumelt,"BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int64,2}",100000)` | 0.86 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100)` | 1.17 | 0.87 | 1.0 | 1.0 |
| `(:sumlinear,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}",100000)` | 0.99 | 1.0 | 1.0 | 1.0 |
| `(:sumcolon,"BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int64,2}",100)` | 0.99 | 1.01 | 1.0 | 1.0 |
| `(:sumeach,"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}",100)` | 1.0 | 1.0 | 1.0 | 1.0 |
| `(:sumlogical,"BitArray{2}",100000)` | 0.99 | 1.02 | 1.0 | 1.0 |

## Version Info

#### Primary Build

```
Julia Version 0.4.3-pre+6
Commit adffe19 (2015-12-11 00:38 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (28553.4453125 MB free)
Uptime: 8.530225e6 sec
Load Avg:  0.99951171875  1.0146484375  1.19287109375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1   800 MHz   80118415 s        216 s   14773173 s  756046815 s         14 s
#2  3501 MHz   12605226 s        148 s    7312190 s  832135077 s          0 s
#3  3501 MHz    8717603 s        888 s    6912582 s  836519991 s          0 s
#4   800 MHz    7750766 s        518 s    7058749 s  837317552 s          0 s
#5   800 MHz    8734428 s        969 s    7747229 s  836385451 s          0 s
#6   800 MHz    5097473 s        609 s    7587820 s  840233437 s          0 s
#7   800 MHz    4145275 s       2516 s    7392536 s  841317452 s          0 s
#8  3501 MHz    3137998 s       1602 s    7413374 s  842373491 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

#### Comparison Build

```
Julia Version 0.4.2
Commit bb73f34 (2015-12-06 21:47 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.3 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (28500.43359375 MB free)
Uptime: 8.534508e6 sec
Load Avg:  1.0029296875  0.99951171875  1.21337890625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1   800 MHz   80220148 s        216 s   14785363 s  756339855 s         14 s
#2   800 MHz   12677143 s        148 s    7322562 s  832449455 s          0 s
#3   800 MHz    8773012 s        888 s    6920361 s  836864723 s          0 s
#4   800 MHz    7802967 s        518 s    7065026 s  837677158 s          0 s
#5  3501 MHz    8756636 s        969 s    7753751 s  836779840 s          0 s
#6   800 MHz    5119388 s        609 s    7594216 s  840628892 s          0 s
#7   800 MHz    4166162 s       2516 s    7398618 s  841711527 s          0 s
#8  3501 MHz    3158136 s       1602 s    7418455 s  842771851 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```

