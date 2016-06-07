# Benchmark Report

## Job Properties

*Commit(s):* [jrevels/julia@3142819516da68d5d928bf66456ad633bc53c915](https://github.com/jrevels/julia/commit/3142819516da68d5d928bf66456ad633bc53c915)

*Triggered By:* [link](https://github.com/jrevels/julia/commit/3142819516da68d5d928bf66456ad633bc53c915#commitcomment-17773535)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-07

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
| `["array","bool","bitarray_bool_load!"]` | 3.30 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","bitarray_true_fill!"]` | 3.12 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","bitarray_true_load!"]` | 2.40 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_bool_load!"]` | 1.32 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_true_fill!"]` | 33.31 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_true_load!"]` | 325.54 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","cat",("catnd",5)]` | 29.43 μs (15%) | 0.00 ns | 19.06 kb (1%) | 98 |
| `["array","cat",("catnd",500)]` | 1.83 ms (15%) | 0.00 ns | 11.46 mb (1%) | 110 |
| `["array","cat",("catnd_setind",5)]` | 10.84 μs (15%) | 0.00 ns | 15.98 kb (1%) | 40 |
| `["array","cat",("catnd_setind",500)]` | 1.54 ms (15%) | 0.00 ns | 11.46 mb (1%) | 43 |
| `["array","cat",("hcat",5)]` | 6.18 μs (15%) | 0.00 ns | 1.36 kb (1%) | 10 |
| `["array","cat",("hcat",500)]` | 635.72 μs (15%) | 0.00 ns | 7.63 mb (1%) | 18 |
| `["array","cat",("hcat_setind",5)]` | 205.00 ns (15%) | 0.00 ns | 1.00 kb (1%) | 5 |
| `["array","cat",("hcat_setind",500)]` | 854.65 μs (15%) | 0.00 ns | 7.63 mb (1%) | 6 |
| `["array","cat",("hvcat",5)]` | 20.98 μs (15%) | 0.00 ns | 3.81 kb (1%) | 39 |
| `["array","cat",("hvcat",500)]` | 2.07 ms (15%) | 0.00 ns | 15.26 mb (1%) | 49 |
| `["array","cat",("hvcat_setind",5)]` | 253.00 ns (15%) | 0.00 ns | 1.13 kb (1%) | 9 |
| `["array","cat",("hvcat_setind",500)]` | 926.51 μs (15%) | 0.00 ns | 7.63 mb (1%) | 10 |
| `["array","cat",("vcat",5)]` | 7.14 μs (15%) | 0.00 ns | 1.48 kb (1%) | 14 |
| `["array","cat",("vcat",500)]` | 966.43 μs (15%) | 0.00 ns | 7.63 mb (1%) | 16 |
| `["array","cat",("vcat_setind",5)]` | 211.00 ns (15%) | 0.00 ns | 1.00 kb (1%) | 5 |
| `["array","cat",("vcat_setind",500)]` | 910.40 μs (15%) | 0.00 ns | 7.63 mb (1%) | 6 |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 12.87 ms (15%) | 0.00 ns | 76.29 mb (1%) | 3 |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 39.75 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 39.74 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 12.66 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 24.03 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 24.04 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","Array{Float64,1}")]` | 78.01 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 215.77 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 244.77 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 78.80 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 104.26 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 117.96 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","growth",("append!",2048)]` | 3.56 μs (15%) | 0.00 ns | 53.36 kb (1%) | 0 |
| `["array","growth",("append!",256)]` | 437.00 ns (15%) | 0.00 ns | 5.10 kb (1%) | 0 |
| `["array","growth",("append!",8)]` | 27.00 ns (15%) | 0.00 ns | 132.00 bytes (1%) | 0 |
| `["array","growth",("prerend!",2048)]` | 2.77 μs (15%) | 0.00 ns | 49.80 kb (1%) | 0 |
| `["array","growth",("prerend!",256)]` | 906.00 ns (15%) | 0.00 ns | 6.58 kb (1%) | 0 |
| `["array","growth",("prerend!",8)]` | 40.00 ns (15%) | 0.00 ns | 132.00 bytes (1%) | 0 |
| `["array","growth",("push_multiple!",2048)]` | 8.14 μs (15%) | 0.00 ns | 32.06 kb (1%) | 1 |
| `["array","growth",("push_multiple!",256)]` | 1.20 μs (15%) | 0.00 ns | 6.02 kb (1%) | 0 |
| `["array","growth",("push_multiple!",8)]` | 38.00 ns (15%) | 0.00 ns | 133.00 bytes (1%) | 0 |
| `["array","growth",("push_single!",2048)]` | 3.08 μs (15%) | 0.00 ns | 10.45 kb (1%) | 8 |
| `["array","growth",("push_single!",256)]` | 2.94 μs (15%) | 0.00 ns | 7.34 kb (1%) | 8 |
| `["array","growth",("push_single!",8)]` | 2.92 μs (15%) | 0.00 ns | 6.94 kb (1%) | 8 |
| `["array","index",("sumcartesian","1.0:1.0:1.0e8")]` | 616.78 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","100000000:-1:1")]` | 51.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","1:100000000")]` | 51.54 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","Array{Float32,2}")]` | 1.05 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 1.00 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BitArray{2}")]` | 9.69 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.01 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 94.97 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 245.86 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","100000000:-1:1")]` | 93.56 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","1:100000000")]` | 88.96 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 227.73 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 212.67 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 240.93 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 217.78 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 243.32 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1500 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 216.96 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1500 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 241.79 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 221.65 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BitArray{2}")]` | 146.61 μs (40%) | 0.00 ns | 101.56 kb (1%) | 2000 |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 324.52 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 219.39 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 39.73 ms (40%) | 0.00 ns | 76.29 mb (1%) | 4 |
| `["array","index",("sumeach","1.0:1.0:1.0e8")]` | 616.20 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","100000000:-1:1")]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","Array{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","Array{Int32,2}")]` | 20.04 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.36 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 95.19 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BitArray{2}")]` | 8.45 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.01 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","linspace(1.0,2.0,10000000)")]` | 96.03 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","1.0:1.0:1.0e8")]` | 615.52 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","100000000:-1:1")]` | 25.65 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","Array{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","Array{Int32,2}")]` | 87.67 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.36 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 103.11 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.24 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 3.24 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.24 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 3.24 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BitArray{2}")]` | 8.50 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.11 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.08 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","linspace(1.0,2.0,10000000)")]` | 94.89 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 615.55 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 517.94 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 257.84 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","Array{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 87.62 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.36 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 103.14 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 419.11 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 439.88 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 419.12 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 439.91 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 8.44 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.46 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.46 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 94.89 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","1.0:1.0:1.0e8")]` | 616.27 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","100000000:-1:1")]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","Array{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 20.04 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.36 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 95.22 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 194.19 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 153.04 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 194.18 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 153.02 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BitArray{2}")]` | 8.45 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumlinear","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.13 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.00 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","linspace(1.0,2.0,10000000)")]` | 96.03 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 273.83 ms (40%) | 5.34 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","100000000:-1:1")]` | 242.88 ms (40%) | 5.33 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","1:100000000")]` | 241.37 ms (40%) | 5.34 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 270.75 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 271.12 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 274.43 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 274.21 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 281.94 μs (40%) | 0.00 ns | 851.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 281.72 μs (40%) | 0.00 ns | 851.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 274.65 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 274.97 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BitArray{2}")]` | 502.94 μs (40%) | 0.00 ns | 601.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 520.87 μs (40%) | 0.00 ns | 1.40 mb (1%) | 4005 |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 521.20 μs (40%) | 0.00 ns | 1.40 mb (1%) | 4005 |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 28.35 ms (40%) | 0.00 ns | 39.34 mb (1%) | 13 |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 251.74 ms (40%) | 6.96 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","100000000:-1:1")]` | 113.24 ms (40%) | 6.93 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","1:100000000")]` | 102.85 ms (40%) | 6.96 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","Array{Float32,2}")]` | 242.13 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","Array{Int32,2}")]` | 222.95 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 245.20 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 224.81 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 246.72 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2500 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 231.44 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2500 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 242.44 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 222.99 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BitArray{2}")]` | 152.47 μs (40%) | 0.00 ns | 132.81 kb (1%) | 3000 |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 321.28 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 218.68 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 43.95 ms (40%) | 4.16 ms | 76.29 mb (1%) | 6 |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 199.00 ns (40%) | 0.00 ns | 336.00 bytes (1%) | 4 |
| `["array","index",("sumvector","100000000:-1:1")]` | 210.00 ns (40%) | 0.00 ns | 320.00 bytes (1%) | 4 |
| `["array","index",("sumvector","1:100000000")]` | 182.00 ns (40%) | 0.00 ns | 320.00 bytes (1%) | 4 |
| `["array","index",("sumvector","Array{Float32,2}")]` | 31.20 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","Array{Int32,2}")]` | 31.09 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 31.47 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 32.02 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 37.42 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 37.77 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 31.70 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 32.20 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BitArray{2}")]` | 116.97 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 64.36 μs (40%) | 0.00 ns | 187.63 kb (1%) | 3501 |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 64.37 μs (40%) | 0.00 ns | 187.63 kb (1%) | 3501 |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 203.00 ns (40%) | 0.00 ns | 336.00 bytes (1%) | 4 |
| `["array","reverse","rev_load_fast!"]` | 757.10 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_load_slow!"]` | 1.88 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_loadmul_fast!"]` | 3.15 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_loadmul_slow!"]` | 3.41 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","setindex!",("setindex!",1)]` | 895.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",2)]` | 897.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",3)]` | 1.06 μs (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",4)]` | 1.07 μs (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",5)]` | 1.04 μs (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.97 ms (15%) | 0.00 ns | 5.84 mb (1%) | 2225 |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 3.01 s (15%) | 1.17 s | 5.03 gb (1%) | 26829 |
| `["array","subarray",("lucompletepivCopy!",250)]` | 42.73 ms (15%) | 16.18 ms | 83.61 mb (1%) | 5675 |
| `["array","subarray",("lucompletepivCopy!",500)]` | 359.29 ms (15%) | 149.87 ms | 651.65 mb (1%) | 11425 |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.97 ms (15%) | 0.00 ns | 5.84 mb (1%) | 2225 |
| `["array","subarray",("lucompletepivSub!",1000)]` | 3.01 s (15%) | 1.17 s | 5.03 gb (1%) | 26829 |
| `["array","subarray",("lucompletepivSub!",250)]` | 42.71 ms (15%) | 16.15 ms | 83.61 mb (1%) | 5675 |
| `["array","subarray",("lucompletepivSub!",500)]` | 359.51 ms (15%) | 149.92 ms | 651.65 mb (1%) | 11425 |
| `["io","read","readstring"]` | 70.00 ns (15%) | 0.00 ns | 208.00 bytes (1%) | 3 |
| `["io","read"]` | 14.59 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","arithmetic",("*","Bidiagonal","Bidiagonal",1024)]` | 49.54 ms (30%) | 0.00 ns | 24.00 mb (1%) | 7 |
| `["linalg","arithmetic",("*","Bidiagonal","Bidiagonal",256)]` | 922.89 μs (30%) | 0.00 ns | 1.50 mb (1%) | 7 |
| `["linalg","arithmetic",("*","Bidiagonal","Vector",1024)]` | 1.03 ms (30%) | 0.00 ns | 8.01 mb (1%) | 4 |
| `["linalg","arithmetic",("*","Bidiagonal","Vector",256)]` | 56.04 μs (30%) | 0.00 ns | 514.22 kb (1%) | 4 |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.26 μs (30%) | 0.00 ns | 8.34 kb (1%) | 9 |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.49 μs (30%) | 0.00 ns | 2.33 kb (1%) | 8 |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 2.33 μs (30%) | 0.00 ns | 8.34 kb (1%) | 9 |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.51 μs (30%) | 0.00 ns | 2.33 kb (1%) | 8 |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 34.72 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 1.08 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",1024)]` | 108.75 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 9.10 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Matrix","Matrix",1024)]` | 47.70 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("*","Matrix","Matrix",256)]` | 827.71 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 217.30 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 11.27 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","SymTridiagonal","SymTridiagonal",1024)]` | 49.52 ms (30%) | 0.00 ns | 24.00 mb (1%) | 7 |
| `["linalg","arithmetic",("*","SymTridiagonal","SymTridiagonal",256)]` | 921.82 μs (30%) | 0.00 ns | 1.50 mb (1%) | 7 |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.77 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 655.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Tridiagonal","Tridiagonal",1024)]` | 49.55 ms (30%) | 0.00 ns | 24.00 mb (1%) | 9 |
| `["linalg","arithmetic",("*","Tridiagonal","Tridiagonal",256)]` | 924.23 μs (30%) | 0.00 ns | 1.50 mb (1%) | 9 |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 1.93 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 633.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 34.65 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 1.07 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",1024)]` | 109.82 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 8.89 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.63 μs (30%) | 0.00 ns | 32.59 kb (1%) | 9 |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.50 μs (30%) | 0.00 ns | 8.59 kb (1%) | 9 |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 866.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 339.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.15 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 48.94 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.12 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 49.32 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.80 μs (30%) | 0.00 ns | 16.31 kb (1%) | 5 |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 712.00 ns (30%) | 0.00 ns | 4.31 kb (1%) | 5 |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.54 μs (30%) | 0.00 ns | 32.59 kb (1%) | 8 |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.29 μs (30%) | 0.00 ns | 8.59 kb (1%) | 8 |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.13 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 49.26 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 888.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 351.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.73 μs (30%) | 0.00 ns | 32.59 kb (1%) | 9 |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.43 μs (30%) | 0.00 ns | 8.59 kb (1%) | 9 |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 898.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 332.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.14 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 48.86 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.12 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 48.53 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 1.77 μs (30%) | 0.00 ns | 16.31 kb (1%) | 5 |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 702.00 ns (30%) | 0.00 ns | 4.31 kb (1%) | 5 |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.59 μs (30%) | 0.00 ns | 32.59 kb (1%) | 8 |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.35 μs (30%) | 0.00 ns | 8.59 kb (1%) | 8 |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.13 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 48.56 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 897.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 343.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 5.06 μs (30%) | 0.00 ns | 8.34 kb (1%) | 9 |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 2.19 μs (30%) | 0.00 ns | 2.33 kb (1%) | 8 |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 38.40 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 1.32 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("/","Matrix","Matrix",1024)]` | 104.29 ms (30%) | 5.19 ms | 40.01 mb (1%) | 20 |
| `["linalg","arithmetic",("/","Matrix","Matrix",256)]` | 2.52 ms (30%) | 0.00 ns | 2.50 mb (1%) | 20 |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 33.65 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 1.05 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",1024)]` | 8.40 μs (30%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",256)]` | 2.20 μs (30%) | 0.00 ns | 2.13 kb (1%) | 1 |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 5.05 μs (30%) | 0.00 ns | 8.34 kb (1%) | 9 |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 2.17 μs (30%) | 0.00 ns | 2.33 kb (1%) | 8 |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 5.07 μs (30%) | 0.00 ns | 8.34 kb (1%) | 9 |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 2.21 μs (30%) | 0.00 ns | 2.33 kb (1%) | 8 |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 37.71 ms (30%) | 0.00 ns | 8.00 mb (1%) | 5 |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 1.24 ms (30%) | 0.00 ns | 512.14 kb (1%) | 5 |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",1024)]` | 516.65 μs (30%) | 0.00 ns | 8.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",256)]` | 33.58 μs (30%) | 0.00 ns | 2.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","Matrix","Matrix",1024)]` | 87.07 ms (30%) | 0.00 ns | 16.01 mb (1%) | 11 |
| `["linalg","arithmetic",("\\","Matrix","Matrix",256)]` | 2.25 ms (30%) | 0.00 ns | 1.00 mb (1%) | 11 |
| `["linalg","arithmetic",("\\","Matrix","Vector",1024)]` | 24.91 ms (30%) | 0.00 ns | 8.02 mb (1%) | 10 |
| `["linalg","arithmetic",("\\","Matrix","Vector",256)]` | 684.02 μs (30%) | 0.00 ns | 516.45 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",1024)]` | 16.58 μs (30%) | 0.00 ns | 24.55 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 4.72 μs (30%) | 0.00 ns | 6.55 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 38.57 μs (30%) | 0.00 ns | 58.19 kb (1%) | 28 |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 14.57 μs (30%) | 0.00 ns | 21.66 kb (1%) | 20 |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 37.59 ms (30%) | 0.00 ns | 8.00 mb (1%) | 5 |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 1.25 ms (30%) | 0.00 ns | 512.14 kb (1%) | 5 |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",1024)]` | 561.22 μs (30%) | 0.00 ns | 8.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",256)]` | 32.70 μs (30%) | 0.00 ns | 2.16 kb (1%) | 3 |
| `["linalg","blas","asum"]` | 138.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","axpy!"]` | 206.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","blascopy!"]` | 138.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","dot"]` | 101.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","dotc"]` | 260.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["linalg","blas","dotu"]` | 260.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["linalg","blas","gbmv!"]` | 194.00 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gbmv"]` | 195.06 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","gemm!"]` | 47.66 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gemm"]` | 47.73 ms (15%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","blas","gemv!"]` | 237.05 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gemv"]` | 220.67 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","ger!"]` | 728.86 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","her!"]` | 1.94 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","herk!"]` | 112.47 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","herk"]` | 112.13 ms (15%) | 0.00 ns | 16.00 mb (1%) | 3 |
| `["linalg","blas","nrm2"]` | 271.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","sbmv!"]` | 223.08 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","sbmv"]` | 225.34 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","scal!"]` | 213.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","scal"]` | 980.00 ns (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","symm!"]` | 47.60 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","symm"]` | 47.71 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","symv!"]` | 114.93 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","symv"]` | 116.57 μs (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","syr!"]` | 551.11 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","syrk!"]` | 28.41 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","syrk"]` | 28.72 ms (15%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","blas","trmm!"]` | 28.07 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trmm"]` | 29.06 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","trmv!"]` | 121.78 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trmv"]` | 120.21 μs (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","trsm!"]` | 31.16 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trsm"]` | 32.07 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","trsv!"]` | 119.99 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trsv"]` | 119.23 μs (20%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","factorization",("chol","Matrix",1024)]` | 12.79 ms (25%) | 0.00 ns | 8.00 mb (1%) | 6 |
| `["linalg","factorization",("chol","Matrix",256)]` | 391.77 μs (25%) | 0.00 ns | 512.17 kb (1%) | 6 |
| `["linalg","factorization",("cholfact","Matrix",1024)]` | 12.97 ms (25%) | 0.00 ns | 8.00 mb (1%) | 6 |
| `["linalg","factorization",("cholfact","Matrix",256)]` | 388.85 μs (25%) | 0.00 ns | 512.17 kb (1%) | 6 |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 238.21 ms (25%) | 31.60 ms | 102.31 mb (1%) | 4591914 |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 12.55 ms (25%) | 0.00 ns | 6.07 mb (1%) | 262433 |
| `["linalg","factorization",("eig","Diagonal",1024)]` | 829.61 μs (25%) | 0.00 ns | 8.03 mb (1%) | 2061 |
| `["linalg","factorization",("eig","Diagonal",256)]` | 62.95 μs (25%) | 0.00 ns | 516.47 kb (1%) | 265 |
| `["linalg","factorization",("eig","LowerTriangular",1024)]` | 74.67 ms (25%) | 5.17 ms | 32.03 mb (1%) | 20 |
| `["linalg","factorization",("eig","LowerTriangular",256)]` | 2.26 ms (25%) | 0.00 ns | 2.01 mb (1%) | 19 |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.49 s (25%) | 5.45 ms | 32.32 mb (1%) | 115 |
| `["linalg","factorization",("eig","Matrix",256)]` | 51.83 ms (25%) | 0.00 ns | 2.09 mb (1%) | 78 |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 108.45 ms (25%) | 0.00 ns | 16.28 mb (1%) | 57 |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 5.70 ms (25%) | 0.00 ns | 1.07 mb (1%) | 53 |
| `["linalg","factorization",("eig","UpperTriangular",1024)]` | 68.24 ms (25%) | 5.22 ms | 24.03 mb (1%) | 17 |
| `["linalg","factorization",("eig","UpperTriangular",256)]` | 1.97 ms (25%) | 0.00 ns | 1.51 mb (1%) | 16 |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 238.30 ms (25%) | 31.55 ms | 102.31 mb (1%) | 4591914 |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 12.57 ms (25%) | 0.00 ns | 6.07 mb (1%) | 262433 |
| `["linalg","factorization",("eigfact","Diagonal",1024)]` | 813.04 μs (25%) | 0.00 ns | 8.03 mb (1%) | 2061 |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 59.96 μs (25%) | 0.00 ns | 516.47 kb (1%) | 265 |
| `["linalg","factorization",("eigfact","LowerTriangular",1024)]` | 74.76 ms (25%) | 5.26 ms | 32.03 mb (1%) | 20 |
| `["linalg","factorization",("eigfact","LowerTriangular",256)]` | 2.28 ms (25%) | 0.00 ns | 2.01 mb (1%) | 19 |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.49 s (25%) | 5.43 ms | 32.32 mb (1%) | 113 |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 51.86 ms (25%) | 0.00 ns | 2.09 mb (1%) | 76 |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 108.48 ms (25%) | 0.00 ns | 16.28 mb (1%) | 57 |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 5.70 ms (25%) | 0.00 ns | 1.07 mb (1%) | 53 |
| `["linalg","factorization",("eigfact","UpperTriangular",1024)]` | 68.36 ms (25%) | 5.20 ms | 24.03 mb (1%) | 17 |
| `["linalg","factorization",("eigfact","UpperTriangular",256)]` | 1.96 ms (25%) | 0.00 ns | 1.51 mb (1%) | 16 |
| `["linalg","factorization",("lu","Matrix",1024)]` | 32.85 ms (25%) | 5.20 ms | 24.02 mb (1%) | 33 |
| `["linalg","factorization",("lu","Matrix",256)]` | 810.00 μs (25%) | 0.00 ns | 1.51 mb (1%) | 33 |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 13.89 ms (25%) | 5.43 ms | 24.64 mb (1%) | 13344 |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 488.92 μs (25%) | 0.00 ns | 1.64 mb (1%) | 2586 |
| `["linalg","factorization",("lufact","Matrix",1024)]` | 24.50 ms (25%) | 0.00 ns | 8.01 mb (1%) | 7 |
| `["linalg","factorization",("lufact","Matrix",256)]` | 664.77 μs (25%) | 0.00 ns | 514.30 kb (1%) | 7 |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 13.41 μs (25%) | 0.00 ns | 40.75 kb (1%) | 8 |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 4.27 μs (25%) | 0.00 ns | 10.75 kb (1%) | 8 |
| `["linalg","factorization",("qr","Matrix",1024)]` | 160.41 ms (25%) | 5.23 ms | 32.60 mb (1%) | 2097 |
| `["linalg","factorization",("qr","Matrix",256)]` | 3.80 ms (25%) | 0.00 ns | 2.15 mb (1%) | 294 |
| `["linalg","factorization",("qrfact","Matrix",1024)]` | 63.09 ms (25%) | 0.00 ns | 8.56 mb (1%) | 17 |
| `["linalg","factorization",("qrfact","Matrix",256)]` | 1.82 ms (25%) | 0.00 ns | 656.44 kb (1%) | 13 |
| `["linalg","factorization",("schur","Matrix",1024)]` | 1.25 s (25%) | 0.00 ns | 16.30 mb (1%) | 25 |
| `["linalg","factorization",("schur","Matrix",256)]` | 47.66 ms (25%) | 0.00 ns | 1.08 mb (1%) | 21 |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 1.26 s (25%) | 0.00 ns | 16.30 mb (1%) | 25 |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 47.61 ms (25%) | 0.00 ns | 1.08 mb (1%) | 21 |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 65.69 ms (25%) | 4.00 ms | 48.13 mb (1%) | 30 |
| `["linalg","factorization",("svd","Bidiagonal",256)]` | 5.46 ms (25%) | 0.00 ns | 3.03 mb (1%) | 29 |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 18.42 ms (25%) | 10.71 ms | 48.42 mb (1%) | 8242 |
| `["linalg","factorization",("svd","Diagonal",256)]` | 517.15 μs (25%) | 0.00 ns | 3.09 mb (1%) | 1319 |
| `["linalg","factorization",("svd","LowerTriangular",1024)]` | 572.49 ms (25%) | 10.39 ms | 64.13 mb (1%) | 26 |
| `["linalg","factorization",("svd","LowerTriangular",256)]` | 16.65 ms (25%) | 0.00 ns | 4.03 mb (1%) | 25 |
| `["linalg","factorization",("svd","Matrix",1024)]` | 598.79 ms (25%) | 10.35 ms | 56.13 mb (1%) | 24 |
| `["linalg","factorization",("svd","Matrix",256)]` | 17.58 ms (25%) | 0.00 ns | 3.53 mb (1%) | 23 |
| `["linalg","factorization",("svd","UpperTriangular",1024)]` | 573.29 ms (25%) | 10.41 ms | 64.13 mb (1%) | 26 |
| `["linalg","factorization",("svd","UpperTriangular",256)]` | 16.79 ms (25%) | 0.00 ns | 4.03 mb (1%) | 25 |
| `["linalg","factorization",("svdfact","Bidiagonal",1024)]` | 58.02 ms (25%) | 4.07 ms | 40.13 mb (1%) | 25 |
| `["linalg","factorization",("svdfact","Bidiagonal",256)]` | 5.39 ms (25%) | 0.00 ns | 2.53 mb (1%) | 24 |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 21.73 ms (25%) | 10.73 ms | 56.42 mb (1%) | 8246 |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 607.08 μs (25%) | 0.00 ns | 3.59 mb (1%) | 1323 |
| `["linalg","factorization",("svdfact","LowerTriangular",1024)]` | 570.79 ms (25%) | 10.41 ms | 56.13 mb (1%) | 21 |
| `["linalg","factorization",("svdfact","LowerTriangular",256)]` | 16.55 ms (25%) | 0.00 ns | 3.53 mb (1%) | 20 |
| `["linalg","factorization",("svdfact","Matrix",1024)]` | 595.33 ms (25%) | 10.39 ms | 48.13 mb (1%) | 19 |
| `["linalg","factorization",("svdfact","Matrix",256)]` | 17.51 ms (25%) | 0.00 ns | 3.03 mb (1%) | 18 |
| `["linalg","factorization",("svdfact","UpperTriangular",1024)]` | 574.18 ms (25%) | 10.62 ms | 56.13 mb (1%) | 21 |
| `["linalg","factorization",("svdfact","UpperTriangular",256)]` | 16.70 ms (25%) | 0.00 ns | 3.53 mb (1%) | 20 |
| `["micro","fib"]` | 36.25 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["micro","mandel"]` | 115.50 μs (15%) | 0.00 ns | 4.44 kb (1%) | 1 |
| `["micro","parseint"]` | 259.67 μs (15%) | 0.00 ns | 234.38 kb (1%) | 5000 |
| `["micro","pisum"]` | 34.55 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["micro","quicksort"]` | 268.17 μs (15%) | 0.00 ns | 39.14 kb (1%) | 2 |
| `["micro","randmatmul"]` | 45.62 ms (15%) | 0.00 ns | 22.89 mb (1%) | 9 |
| `["micro","randmatstat"]` | 44.39 ms (15%) | 0.00 ns | 18.65 mb (1%) | 67008 |
| `["parallel","remotecall",("identity",1024)]` | 265.79 μs (15%) | 0.00 ns | 26.95 kb (1%) | 470 |
| `["parallel","remotecall",("identity",2)]` | 250.70 μs (15%) | 0.00 ns | 24.78 kb (1%) | 466 |
| `["parallel","remotecall",("identity",4096)]` | 280.15 μs (15%) | 0.00 ns | 33.11 kb (1%) | 475 |
| `["parallel","remotecall",("identity",512)]` | 271.23 μs (15%) | 0.00 ns | 25.98 kb (1%) | 474 |
| `["parallel","remotecall",("identity",64)]` | 269.94 μs (15%) | 0.00 ns | 24.95 kb (1%) | 468 |
| `["problem","fem","sparse_fem"]` | 222.63 ms (15%) | 16.00 ms | 119.02 mb (1%) | 203 |
| `["problem","go","go_game"]` | 737.70 ms (15%) | 128.58 ms | 388.15 mb (1%) | 3018122 |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.24 s (15%) | 565.14 ms | 2.04 gb (1%) | 1853876 |
| `["problem","imdb","centrality"]` | 1.01 s (15%) | 53.14 ms | 97.88 mb (1%) | 822192 |
| `["problem","json","parse_json"]` | 1.33 ms (15%) | 0.00 ns | 722.50 kb (1%) | 17878 |
| `["problem","laplacian","laplace_iter_devec"]` | 14.11 ms (15%) | 0.00 ns | 64.17 kb (1%) | 5 |
| `["problem","laplacian","laplace_iter_sub"]` | 146.27 ms (15%) | 43.95 ms | 181.34 mb (1%) | 21507 |
| `["problem","laplacian","laplace_iter_vec"]` | 111.37 ms (15%) | 71.37 ms | 302.22 mb (1%) | 46083 |
| `["problem","laplacian","laplace_sparse_matvec"]` | 139.16 ms (15%) | 5.98 ms | 24.73 mb (1%) | 98736 |
| `["problem","monte carlo","euro_option_devec"]` | 33.11 ms (15%) | 0.00 ns | 19.40 mb (1%) | 508 |
| `["problem","monte carlo","euro_option_vec"]` | 64.04 ms (15%) | 21.64 ms | 95.82 mb (1%) | 4508 |
| `["problem","raytrace"]` | 1.23 s (15%) | 106.03 ms | 267.38 mb (1%) | 7277262 |
| `["problem","seismic",("seismic","Float32")]` | 615.73 μs (15%) | 0.00 ns | 938.16 kb (1%) | 15 |
| `["problem","seismic",("seismic","Float64")]` | 1.13 ms (15%) | 0.00 ns | 1.83 mb (1%) | 13 |
| `["problem","simplex"]` | 38.51 ms (15%) | 0.00 ns | 326.11 kb (1%) | 2414 |
| `["problem","spellcheck"]` | 13.85 s (15%) | 2.71 s | 6.44 gb (1%) | 103905231 |
| `["problem","stockcorr"]` | 437.37 ms (15%) | 243.48 ms | 231.63 mb (1%) | 30016 |
| `["problem","ziggurat"]` | 5.52 s (15%) | 1.96 s | 6.65 gb (1%) | 13000002 |
| `["scalar","arithmetic",("add","BigFloat","BigFloat")]` | 101.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 192.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 104.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 283.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 299.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 298.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 218.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 218.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 201.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Int64")]` | 130.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","UInt64")]` | 129.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 192.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","BigInt")]` | 126.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 194.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 128.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 412.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 414.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 205.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 194.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 320.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 321.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Int64")]` | 124.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","UInt64")]` | 122.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 103.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 195.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 203.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 286.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 358.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 359.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 230.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 226.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 204.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 205.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 134.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 132.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 283.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 128.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 286.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 211.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 578.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 586.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 215.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{UInt64}")]` | 199.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 407.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 407.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 137.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 124.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 299.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 411.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 365.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 617.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 298.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 411.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 355.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 583.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 217.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 205.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 243.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 214.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 218.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 191.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 227.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigInt}")]` | 198.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 321.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 204.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 407.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 203.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 320.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 204.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 416.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","BigFloat")]` | 130.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Int64","BigInt")]` | 124.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 132.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 137.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","BigFloat")]` | 129.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","UInt64","BigInt")]` | 123.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 131.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 124.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","BigFloat","BigFloat")]` | 224.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 225.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 982.00 ns (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.18 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 369.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 376.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 376.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 376.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 233.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 234.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Int64")]` | 88.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigFloat","UInt64")]` | 87.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigInt","BigFloat")]` | 326.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","BigInt","BigInt")]` | 424.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.10 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.31 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 652.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 655.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 658.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 657.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 445.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 446.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 335.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 334.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 322.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 393.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigFloat}")]` | 1.18 μs (50%) | 0.00 ns | 1.15 kb (1%) | 23 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigInt}")]` | 1.36 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float32}")]` | 1.36 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float64}")]` | 1.40 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Int64}")]` | 1.38 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{UInt64}")]` | 1.36 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 407.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 410.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 188.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 187.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 511.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 701.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigFloat}")]` | 1.37 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 1.67 μs (50%) | 0.00 ns | 1.41 kb (1%) | 32 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float32}")]` | 1.56 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float64}")]` | 1.58 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 1.86 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 1.88 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 745.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 752.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 602.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 601.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 472.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 724.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigFloat}")]` | 1.40 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigInt}")]` | 1.58 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 11.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Int64}")]` | 20.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{UInt64}")]` | 20.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 471.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 737.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigFloat}")]` | 1.41 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigInt}")]` | 1.55 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float32}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float64}")]` | 13.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Int64}")]` | 17.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{UInt64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 329.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 676.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigFloat}")]` | 1.33 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 1.86 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float32}")]` | 25.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 10.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{UInt64}")]` | 8.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 327.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 677.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigFloat}")]` | 1.37 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 1.87 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Float32}")]` | 15.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Float64}")]` | 15.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Int64}")]` | 8.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 7.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 309.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 446.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.12 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.34 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","Float32","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 309.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 445.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.12 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.32 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","BigFloat")]` | 235.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 409.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 961.00 ns (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.14 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","Int64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{Float64}")]` | 9.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","BigFloat")]` | 235.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 409.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 948.00 ns (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.13 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","UInt64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 137.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 193.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 231.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 346.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 363.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 363.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 183.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 183.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 201.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Int64")]` | 87.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigFloat","UInt64")]` | 87.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 193.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","BigInt")]` | 127.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 352.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 210.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 625.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 640.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Int64}")]` | 201.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Complex{UInt64}")]` | 198.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 353.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 352.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Int64")]` | 126.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","UInt64")]` | 125.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 231.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 358.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 652.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 850.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 883.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 884.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 537.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 531.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 413.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 378.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 183.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 186.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 346.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 209.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 859.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigInt}")]` | 569.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.44 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 1.44 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 576.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{UInt64}")]` | 574.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 646.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 653.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Int64")]` | 202.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","UInt64")]` | 200.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 363.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 626.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 886.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 1.44 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 370.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 626.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 895.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 1.44 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 182.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigInt")]` | 199.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 536.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 575.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 183.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigInt")]` | 198.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 525.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigInt}")]` | 569.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 201.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 352.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 380.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 654.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 352.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 378.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 651.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","BigFloat")]` | 88.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","Int64","BigInt")]` | 126.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 188.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Int64","Complex{BigInt}")]` | 203.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","BigFloat")]` | 87.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","UInt64","BigInt")]` | 125.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 186.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigInt}")]` | 199.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","BigFloat","BigFloat")]` | 87.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 170.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 176.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 335.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 349.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 349.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 284.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 282.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 180.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 180.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Int64")]` | 108.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigFloat","UInt64")]` | 107.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 172.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","BigInt")]` | 127.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 256.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 206.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 486.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 493.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Int64}")]` | 285.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","BigInt","Complex{UInt64}")]` | 276.00 ns (50%) | 0.00 ns | 176.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 306.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 307.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigInt","Int64")]` | 124.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","UInt64")]` | 123.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 90.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 173.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 189.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 267.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 342.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 342.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 205.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 211.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 182.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 182.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 110.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 109.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 260.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 130.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 268.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 213.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 589.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 592.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 213.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{UInt64}")]` | 199.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 392.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 393.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 137.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 125.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 273.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 399.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 342.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 591.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 272.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 398.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 342.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 591.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 199.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 158.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 210.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 159.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 196.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 149.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 210.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigInt}")]` | 150.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 180.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 305.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 265.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 481.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 180.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 307.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 265.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 481.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","BigFloat")]` | 111.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Int64","BigInt")]` | 76.00 ns (50%) | 0.00 ns | 56.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 198.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Int64","Complex{BigInt}")]` | 159.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","BigFloat")]` | 110.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","UInt64","BigInt")]` | 74.00 ns (50%) | 0.00 ns | 56.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 207.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigInt}")]` | 151.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","BigFloat")]` | 130.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("add","BigInt")]` | 126.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 567.00 ns (40%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","fastmath",("add","Complex{BigInt}")]` | 560.00 ns (40%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","BigFloat")]` | 223.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("div","BigInt")]` | 423.00 ns (40%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","fastmath",("div","Complex{BigFloat}")]` | 1.17 μs (40%) | 0.00 ns | 1.15 kb (1%) | 23 |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 1.68 μs (40%) | 0.00 ns | 1.41 kb (1%) | 32 |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 10.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{UInt64}")]` | 7.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","BigFloat")]` | 101.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("mul","BigInt")]` | 126.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 203.00 ns (40%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 211.00 ns (40%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","fastmath",("mul","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","BigFloat")]` | 87.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("sub","BigInt")]` | 127.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 190.00 ns (40%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 212.00 ns (40%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","fastmath",("sub","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","BigFloat")]` | 15.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","BigInt")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{BigFloat}")]` | 28.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{BigInt}")]` | 10.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("iseven","BigInt")]` | 164.00 ns (25%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","predicate",("iseven","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("iseven","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","BigFloat")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{BigFloat}")]` | 11.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","BigFloat")]` | 3.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{BigFloat}")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","BigFloat")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{BigFloat}")]` | 16.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 5.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","BigFloat")]` | 15.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","BigInt")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","BigFloat")]` | 3.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{BigFloat}")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isodd","BigInt")]` | 164.00 ns (25%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","predicate",("isodd","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isodd","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["shootout","binary_trees"]` | 31.25 ms (15%) | 0.00 ns | 11.92 mb (1%) | 515432 |
| `["shootout","fannkuch"]` | 139.88 μs (15%) | 0.00 ns | 336.00 bytes (1%) | 3 |
| `["shootout","fasta"]` | 12.82 μs (15%) | 0.00 ns | 16.83 kb (1%) | 813 |
| `["shootout","k_nucleotide"]` | 102.37 ms (15%) | 16.70 ms | 52.19 mb (1%) | 762695 |
| `["shootout","mandelbrot"]` | 3.51 ms (15%) | 0.00 ns | 9.53 kb (1%) | 58 |
| `["shootout","meteor_contest"]` | 2.65 s (15%) | 444.01 ms | 1.04 gb (1%) | 52393026 |
| `["shootout","nbody"]` | 159.90 μs (15%) | 0.00 ns | 448.00 bytes (1%) | 6 |
| `["shootout","nbody_vec"]` | 2.88 ms (15%) | 0.00 ns | 8.01 mb (1%) | 105035 |
| `["shootout","pidigits"]` | 27.34 ms (15%) | 13.32 ms | 63.47 mb (1%) | 101225 |
| `["shootout","regex_dna"]` | 6.19 ms (15%) | 0.00 ns | 3.27 mb (1%) | 8754 |
| `["shootout","revcomp"]` | 11.63 ms (15%) | 0.00 ns | 1.96 mb (1%) | 12369 |
| `["shootout","spectralnorm"]` | 1.44 ms (15%) | 0.00 ns | 8.89 kb (1%) | 404 |
| `["simd",("axpy!","Float32",4095)]` | 233.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float32",4096)]` | 220.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float64",4095)]` | 448.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float64",4096)]` | 441.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int32",4095)]` | 287.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int32",4096)]` | 272.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int64",4095)]` | 1.61 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int64",4096)]` | 1.61 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float32",4095)]` | 13.22 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float32",4096)]` | 13.22 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float64",4095)]` | 13.65 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float64",4096)]` | 13.63 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int32",4095)]` | 182.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int32",4096)]` | 181.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int64",4095)]` | 325.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int64",4096)]` | 283.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float32",4095)]` | 235.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float32",4096)]` | 227.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float64",4095)]` | 453.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float64",4096)]` | 450.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int32",4095)]` | 279.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int32",4096)]` | 272.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int64",4095)]` | 1.98 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int64",4096)]` | 1.98 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("local_arrays","Float32",4095)]` | 878.95 μs (20%) | 0.00 ns | 373.64 kb (1%) | 19494 |
| `["simd",("local_arrays","Float32",4096)]` | 878.80 μs (20%) | 0.00 ns | 373.72 kb (1%) | 19499 |
| `["simd",("local_arrays","Float64",4095)]` | 849.58 μs (20%) | 0.00 ns | 421.03 kb (1%) | 19491 |
| `["simd",("local_arrays","Float64",4096)]` | 849.02 μs (20%) | 0.00 ns | 421.11 kb (1%) | 19496 |
| `["simd",("local_arrays","Int32",4095)]` | 822.30 μs (20%) | 0.00 ns | 373.64 kb (1%) | 19494 |
| `["simd",("local_arrays","Int32",4096)]` | 825.21 μs (20%) | 0.00 ns | 373.72 kb (1%) | 19499 |
| `["simd",("local_arrays","Int64",4095)]` | 846.42 μs (20%) | 0.00 ns | 421.50 kb (1%) | 19497 |
| `["simd",("local_arrays","Int64",4096)]` | 844.38 μs (20%) | 0.00 ns | 421.58 kb (1%) | 19502 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 217.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 201.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 216.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 201.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 438.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 427.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 438.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 427.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 293.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 280.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 294.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 280.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("manual_example!","Float32",4095)]` | 332.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float32",4096)]` | 320.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float64",4095)]` | 644.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float64",4096)]` | 638.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int32",4095)]` | 337.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int32",4096)]` | 328.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int64",4095)]` | 1.14 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int64",4096)]` | 1.12 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float32",4095)]` | 78.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float32",4096)]` | 78.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float64",4095)]` | 142.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float64",4096)]` | 142.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int32",4095)]` | 59.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int32",4096)]` | 58.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int64",4095)]` | 87.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int64",4096)]` | 90.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float32",4095)]` | 882.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float32",4096)]` | 870.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float64",4095)]` | 1.75 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float64",4096)]` | 1.75 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int32",4095)]` | 127.97 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int32",4096)]` | 127.97 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int64",4095)]` | 659.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int64",4096)]` | 653.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","insertionsort",("sort forwards","ascending")]` | 68.86 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","descending")]` | 580.01 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","ones")]` | 171.78 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","random")]` | 289.05 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort reverse","ascending")]` | 580.00 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","descending")]` | 71.77 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","ones")]` | 192.71 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","random")]` | 286.29 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 31.69 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","descending")]` | 579.98 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","ones")]` | 133.10 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","random")]` | 288.99 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 579.86 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","descending")]` | 32.81 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","ones")]` | 154.69 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","random")]` | 286.28 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 102.15 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 930.91 ms (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 270.54 μs (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm forwards","random")]` | 713.87 ms (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 926.04 ms (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 103.50 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 291.40 μs (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm reverse","random")]` | 706.41 ms (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 85.73 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 930.89 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 254.31 μs (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 713.82 ms (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 926.00 ms (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 86.90 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 274.21 μs (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 706.37 ms (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","issorted",("forwards","ascending")]` | 21.94 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","descending")]` | 24.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","ones")]` | 86.49 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","random")]` | 28.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("reverse","ascending")]` | 389.00 ns (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","descending")]` | 23.14 μs (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","ones")]` | 85.98 μs (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","random")]` | 388.00 ns (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","mergesort",("sort forwards","ascending")]` | 676.43 μs (15%) | 0.00 ns | 586.56 kb (1%) | 12 |
| `["sort","mergesort",("sort forwards","descending")]` | 884.13 μs (15%) | 0.00 ns | 586.56 kb (1%) | 12 |
| `["sort","mergesort",("sort forwards","ones")]` | 801.29 μs (15%) | 0.00 ns | 586.64 kb (1%) | 13 |
| `["sort","mergesort",("sort forwards","random")]` | 3.68 ms (15%) | 0.00 ns | 586.64 kb (1%) | 13 |
| `["sort","mergesort",("sort reverse","ascending")]` | 884.78 μs (15%) | 0.00 ns | 586.67 kb (1%) | 15 |
| `["sort","mergesort",("sort reverse","descending")]` | 678.23 μs (15%) | 0.00 ns | 586.67 kb (1%) | 15 |
| `["sort","mergesort",("sort reverse","ones")]` | 837.13 μs (15%) | 0.00 ns | 586.75 kb (1%) | 16 |
| `["sort","mergesort",("sort reverse","random")]` | 3.71 ms (15%) | 0.00 ns | 586.75 kb (1%) | 16 |
| `["sort","mergesort",("sort! forwards","ascending")]` | 638.28 μs (15%) | 0.00 ns | 195.55 kb (1%) | 3 |
| `["sort","mergesort",("sort! forwards","descending")]` | 845.00 μs (15%) | 0.00 ns | 195.55 kb (1%) | 3 |
| `["sort","mergesort",("sort! forwards","ones")]` | 764.76 μs (15%) | 0.00 ns | 195.63 kb (1%) | 4 |
| `["sort","mergesort",("sort! forwards","random")]` | 3.64 ms (15%) | 0.00 ns | 195.63 kb (1%) | 4 |
| `["sort","mergesort",("sort! reverse","ascending")]` | 845.72 μs (15%) | 0.00 ns | 195.56 kb (1%) | 3 |
| `["sort","mergesort",("sort! reverse","descending")]` | 639.28 μs (15%) | 0.00 ns | 195.56 kb (1%) | 3 |
| `["sort","mergesort",("sort! reverse","ones")]` | 798.11 μs (15%) | 0.00 ns | 195.64 kb (1%) | 4 |
| `["sort","mergesort",("sort! reverse","random")]` | 3.67 ms (15%) | 0.00 ns | 195.64 kb (1%) | 4 |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.02 ms (15%) | 0.00 ns | 586.30 kb (1%) | 7 |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.25 ms (15%) | 0.00 ns | 586.30 kb (1%) | 7 |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.20 ms (15%) | 0.00 ns | 586.41 kb (1%) | 10 |
| `["sort","mergesort",("sortperm forwards","random")]` | 5.42 ms (15%) | 0.00 ns | 586.41 kb (1%) | 10 |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.25 ms (15%) | 0.00 ns | 586.31 kb (1%) | 7 |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.02 ms (15%) | 0.00 ns | 586.31 kb (1%) | 7 |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.21 ms (15%) | 0.00 ns | 586.42 kb (1%) | 10 |
| `["sort","mergesort",("sortperm reverse","random")]` | 5.42 ms (15%) | 0.00 ns | 586.42 kb (1%) | 10 |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 998.46 μs (15%) | 0.00 ns | 195.56 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.23 ms (15%) | 0.00 ns | 195.56 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.19 ms (15%) | 0.00 ns | 195.67 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! forwards","random")]` | 5.41 ms (15%) | 0.00 ns | 195.67 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.23 ms (15%) | 0.00 ns | 195.58 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 999.08 μs (15%) | 0.00 ns | 195.58 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.19 ms (15%) | 0.00 ns | 195.69 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! reverse","random")]` | 5.41 ms (15%) | 0.00 ns | 195.69 kb (1%) | 7 |
| `["sort","quicksort",("sort forwards","ascending")]` | 308.80 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","descending")]` | 326.06 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","ones")]` | 592.85 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","random")]` | 2.30 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort reverse","ascending")]` | 346.09 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","descending")]` | 328.48 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","ones")]` | 614.78 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","random")]` | 2.32 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort! forwards","ascending")]` | 270.71 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","descending")]` | 288.30 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","ones")]` | 553.36 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","random")]` | 2.26 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","ascending")]` | 306.17 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","descending")]` | 288.80 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","ones")]` | 575.62 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","random")]` | 2.28 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 459.42 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","quicksort",("sortperm forwards","descending")]` | 485.47 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","quicksort",("sortperm forwards","ones")]` | 749.51 μs (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","quicksort",("sortperm forwards","random")]` | 3.57 ms (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 483.27 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","quicksort",("sortperm reverse","descending")]` | 458.59 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","quicksort",("sortperm reverse","ones")]` | 769.76 μs (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","quicksort",("sortperm reverse","random")]` | 3.60 ms (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 441.72 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 467.69 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 732.72 μs (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! forwards","random")]` | 3.56 ms (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 466.68 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 440.65 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 752.37 μs (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! reverse","random")]` | 3.58 ms (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sparse","index",("spmat","array",10)]` | 27.52 μs (25%) | 0.00 ns | 2.91 kb (1%) | 31 |
| `["sparse","index",("spmat","array",100)]` | 437.56 μs (25%) | 0.00 ns | 37.67 kb (1%) | 313 |
| `["sparse","index",("spmat","array",1000)]` | 4.99 ms (25%) | 0.00 ns | 721.39 kb (1%) | 3015 |
| `["sparse","index",("spmat","col","array",10)]` | 8.26 μs (15%) | 0.00 ns | 1.52 kb (1%) | 18 |
| `["sparse","index",("spmat","col","array",100)]` | 9.45 μs (15%) | 0.00 ns | 3.91 kb (1%) | 18 |
| `["sparse","index",("spmat","col","array",1000)]` | 46.07 μs (15%) | 0.00 ns | 26.27 kb (1%) | 18 |
| `["sparse","index",("spmat","col","logical",10)]` | 317.00 ns (15%) | 0.00 ns | 752.00 bytes (1%) | 8 |
| `["sparse","index",("spmat","col","logical",100)]` | 815.00 ns (15%) | 0.00 ns | 1.86 kb (1%) | 8 |
| `["sparse","index",("spmat","col","logical",1000)]` | 6.44 μs (15%) | 0.00 ns | 12.92 kb (1%) | 8 |
| `["sparse","index",("spmat","col","range",10)]` | 151.00 ns (15%) | 0.00 ns | 480.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","col","range",100)]` | 155.00 ns (15%) | 0.00 ns | 608.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","col","range",1000)]` | 251.00 ns (15%) | 0.00 ns | 1.78 kb (1%) | 5 |
| `["sparse","index",("spmat","integer",10)]` | 12.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","integer",100)]` | 14.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","integer",1000)]` | 15.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","logical",10)]` | 377.00 ns (25%) | 0.00 ns | 816.00 bytes (1%) | 7 |
| `["sparse","index",("spmat","logical",100)]` | 8.39 μs (25%) | 0.00 ns | 7.02 kb (1%) | 7 |
| `["sparse","index",("spmat","logical",1000)]` | 147.68 μs (25%) | 0.00 ns | 142.45 kb (1%) | 9 |
| `["sparse","index",("spmat","range",10)]` | 209.00 ns (25%) | 0.00 ns | 896.00 bytes (1%) | 4 |
| `["sparse","index",("spmat","range",100)]` | 2.37 μs (25%) | 0.00 ns | 16.67 kb (1%) | 4 |
| `["sparse","index",("spmat","range",1000)]` | 53.24 μs (25%) | 0.00 ns | 501.95 kb (1%) | 6 |
| `["sparse","index",("spmat","row","array",10)]` | 181.00 ns (15%) | 0.00 ns | 288.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","row","array",100)]` | 1.25 μs (15%) | 0.00 ns | 736.00 bytes (1%) | 9 |
| `["sparse","index",("spmat","row","array",1000)]` | 19.80 μs (15%) | 0.00 ns | 1.38 kb (1%) | 11 |
| `["sparse","index",("spmat","row","logical",10)]` | 184.00 ns (15%) | 0.00 ns | 416.00 bytes (1%) | 6 |
| `["sparse","index",("spmat","row","logical",100)]` | 1.02 μs (15%) | 0.00 ns | 832.00 bytes (1%) | 6 |
| `["sparse","index",("spmat","row","logical",1000)]` | 11.59 μs (15%) | 0.00 ns | 4.78 kb (1%) | 10 |
| `["sparse","index",("spmat","row","range",10)]` | 157.00 ns (15%) | 0.00 ns | 288.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","row","range",100)]` | 902.00 ns (15%) | 0.00 ns | 448.00 bytes (1%) | 7 |
| `["sparse","index",("spmat","row","range",1000)]` | 15.32 μs (15%) | 0.00 ns | 1.38 kb (1%) | 11 |
| `["sparse","index",("spmat","splogical",10)]` | 153.00 ns (25%) | 0.00 ns | 192.00 bytes (1%) | 3 |
| `["sparse","index",("spmat","splogical",100)]` | 900.00 ns (25%) | 0.00 ns | 192.00 bytes (1%) | 3 |
| `["sparse","index",("spmat","splogical",1000)]` | 7.67 ms (25%) | 0.00 ns | 352.00 bytes (1%) | 3 |
| `["sparse","index",("spvec","array",1000)]` | 45.98 μs (15%) | 0.00 ns | 27.11 kb (1%) | 20 |
| `["sparse","index",("spvec","array",10000)]` | 641.16 μs (15%) | 0.00 ns | 239.23 kb (1%) | 23 |
| `["sparse","index",("spvec","array",100000)]` | 8.21 ms (15%) | 0.00 ns | 2.30 mb (1%) | 23 |
| `["sparse","index",("spvec","integer",1000)]` | 41.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spvec","integer",10000)]` | 45.00 ns (15%) | 0.00 ns | 16.00 bytes (1%) | 1 |
| `["sparse","index",("spvec","integer",100000)]` | 48.00 ns (15%) | 0.00 ns | 16.00 bytes (1%) | 1 |
| `["sparse","index",("spvec","logical",1000)]` | 5.70 μs (15%) | 0.00 ns | 4.94 kb (1%) | 9 |
| `["sparse","index",("spvec","logical",10000)]` | 92.33 μs (15%) | 0.00 ns | 39.98 kb (1%) | 10 |
| `["sparse","index",("spvec","logical",100000)]` | 987.65 μs (15%) | 0.00 ns | 394.77 kb (1%) | 10 |
| `["sparse","index",("spvec","range",1000)]` | 229.00 ns (15%) | 0.00 ns | 832.00 bytes (1%) | 3 |
| `["sparse","index",("spvec","range",10000)]` | 487.00 ns (15%) | 0.00 ns | 2.00 kb (1%) | 3 |
| `["sparse","index",("spvec","range",100000)]` | 1.29 μs (15%) | 0.00 ns | 5.16 kb (1%) | 3 |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 31.28 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 62.73 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 12.33 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 19.42 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 35.56 ms (15%) | 4.16 ms | 45.91 mb (1%) | 8 |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 73.69 ms (15%) | 9.29 ms | 91.69 mb (1%) | 8 |
| `["sparse","transpose",("ctranspose",(600,400))]` | 16.69 μs (15%) | 0.00 ns | 60.55 kb (1%) | 7 |
| `["sparse","transpose",("ctranspose",(600,600))]` | 25.80 μs (15%) | 0.00 ns | 88.30 kb (1%) | 7 |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 29.69 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 61.07 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(600,400))]` | 9.94 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(600,600))]` | 17.28 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose",(20000,10000))]` | 34.14 ms (15%) | 4.15 ms | 30.66 mb (1%) | 8 |
| `["sparse","transpose",("transpose",(20000,20000))]` | 71.08 ms (15%) | 8.66 ms | 61.18 mb (1%) | 8 |
| `["sparse","transpose",("transpose",(600,400))]` | 12.95 μs (15%) | 0.00 ns | 42.11 kb (1%) | 7 |
| `["sparse","transpose",("transpose",(600,600))]` | 21.45 μs (15%) | 0.00 ns | 60.61 kb (1%) | 7 |
| `["string","join"]` | 251.04 ms (15%) | 159.00 ms | 224.39 mb (1%) | 22 |
| `["string","replace"]` | 206.67 μs (15%) | 0.00 ns | 22.05 kb (1%) | 7 |
| `["tuple","index",("sumelt","NTuple",3,Float32)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 13.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",60,Float32)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",60,Float64)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",8,Float32)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",8,Float64)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",3,Float32)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",3,Float64)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 13.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |

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
- `["io","read"]`
- `["io"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4563
Commit 3142819 (2016-06-06 22:30 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28025.34765625 MB free)
Uptime: 966464.0 sec
Load Avg:  1.0029296875  1.01220703125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     518386 s          0 s     213398 s   95669607 s          3 s
#2  3501 MHz    1130690 s          0 s      94591 s   95363114 s          0 s
#3  3501 MHz     317402 s          0 s      93242 s   96182640 s          0 s
#4  3501 MHz     272154 s          0 s      76329 s   96263326 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
