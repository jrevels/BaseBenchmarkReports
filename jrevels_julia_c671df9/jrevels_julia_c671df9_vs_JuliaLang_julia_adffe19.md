# Benchmark Report

## Properties

*Job:* jrevels/julia@c671df9 vs JuliaLang/julia@adffe19

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2#issuecomment-167877513)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory. Note that it's technically possible
for this JSON data to get out of sync with the below table. This would only happen in case
of a network error during the job, and as such is very unlikely. Just in case, you can always
verify that they are synced up by checking the commit history of both files.


All non-ID entries in the below table take the form `(isfailure, value)` where `isfailure`
is a boolean specifying whether or not the corresponding `value` was considered a failure.

By default, `value` is simply the ratio of the head commit result vs. comparison commit
result for the corresponding metric. Thus, `value < 1.0` would denote an improvement,
while `value > 1.0` would denote a regression (note that a tolerance of `0.05` is granted
by default when passing judgment on these results).

| Benchmark ID | time | % of time spent in GC | bytes allocated | number of allocations |
|--------------|------|-----------------------|-----------------|-----------------------|
| `(:sumvector,Array{Int64,2},100)` | 1.377361619e7 | 6.154884605824441 | 8.800144e6 | 200003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.19874186e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.68653685e7 | 16.165533916085923 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 4.391486042e7 | 2.1820145097333654 | 8.000016e6 | 150001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.013632703e7 | 27.51531773988666 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.22719859e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 4.938192395e7 | 14.01356890704345 | 7.0400224e7 | 250006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.25080994e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.154364779e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.792160997894737e8 | 9.495919138712317 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 2.74901863e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 3.070025848e7 | 27.315288712062934 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 1.323759042972973e8 | 7.8659292868970585 | 1.12000016e8 | 3.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.7911491484210527e8 | 7.0382524649324 | 8.8000144e7 | 2.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.15431633e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.663911142e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.018622117e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.38563982e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 486208.32 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.56780709e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 1.143237619e7 | 5.811067509852198 | 8.000144e6 | 200003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.338446478e7 | 17.29855930477586 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.834344913773585e8 | 8.554897067712357 | 1.28000192e8 | 3.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.245739719e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.89781061e6 | 23.040604683105656 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 5.095458478e7 | 13.615312344953342 | 7.0400224e7 | 250006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 1.3399633473972602e8 | 6.743966917512006 | 8.8000144e7 | 2.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 4.25775407e7 | 18.84849841226907 | 7.4400016e7 | 300001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.2501911e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.654082046e7 | 27.711308065210243 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.385439549e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 8.037420989e7 | 9.008595418481683 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 2.22532012e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 6.103689295e7 | 17.732471426368825 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 1.4012621755072463e8 | 6.089868422339445 | 1.12000192e8 | 2.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 3.942426795e7 | 18.635907794806467 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.1543222e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.155783653e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.122983948e7 | 5.657001633832344 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 494159.85 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.602033505e7 | 31.039003234831892 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.42717581e7 | 10.563441620693638 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.07846227e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20581535e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 1.160783085862069e8 | 6.296576908263331 | 8.0000144e7 | 2.000003e6 |
| `(:sumlinear,Array{Int64,2},100)` | 2.74849069e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,JLD.UnsupportedType,100)` | 7.85138334e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.154307149e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.02666738e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.379450652e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.339984324e7 | 25.273592115668126 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 1.3982929815942028e8 | 6.181365154102295 | 1.12000192e8 | 2.500006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.770043455e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 1.1904249197590362e8 | 11.109780510323672 | 1.04000016e8 | 3.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 821179.38 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 5.426431654e7 | 3.0954006636868314 | 1.3600016e7 | 350001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.587256614e7 | 22.048109350314125 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.18058873e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.241777433e7 | 23.761153094365003 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 1.133625884e7 | 5.8356449165599145 | 8.000144e6 | 200003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.11142855e6 | 25.14945408815433 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 2.900155283e7 | 14.942169363648688 | 4.8000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.388778218e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.25114452e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.379470383e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 4.495903406e7 | 14.349018438776168 | 5.6800224e7 | 250006.0 |
| `(:sumrange,Array{Int64,2},100)` | 3.783595897e7 | 21.082921200754313 | 1.30400016e8 | 300001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.749201755e7 | 21.30043497354038 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.906491785e7 | 19.161427123919285 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 1.8808505025e8 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.966841652631579e8 | 9.175316648468394 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 3.291801186e7 | 22.382365223656663 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 481673.08 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.681510107e7 | 28.33848902025148 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 1.18913978e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.15428406e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.155697487e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.05238987e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.3090328e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.7261970789473686e8 | 9.088724992602987 | 1.20000016e8 | 3.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 1.108084031e8 | 6.448239979631104 | 8.0000144e7 | 2.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 4.648234524e7 | 17.77646930725967 | 1.31200016e8 | 350001.0 |
| `(:sumvector,BitArray{2},100)` | 1.683606961e7 | 6.580444976357951 | 8.800144e6 | 250003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.154374417e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.579868073e7 | 27.897174182589314 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.771071794e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.74773681e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.40513758e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 1.976542335e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.05307403e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.545386745e7 | 30.107510465952647 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 1.2817120936842105e8 | 9.101729794505314 | 1.12000192e8 | 2.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 5.117703633e7 | 9.529727678514357 | 4.2400224e7 | 300006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.567244315e7 | 27.03250049627445 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 1.3306951004054055e8 | 7.751881154290833 | 1.12000016e8 | 3.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 1.988717811e7 | 0.0 | 16.0 | 1.0 |

