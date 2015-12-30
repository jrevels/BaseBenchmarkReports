# Benchmark Report

## Properties

*Job:* jrevels/julia@adffe19 vs JuliaLang/julia@bb73f34

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195664)

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
| `(:sumvector,Array{Int64,2},100)` | 4.12058878e6 | 11.093973529661437 | 6.400144e6 | 100003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.244224963e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.90464407e7 | 14.461341477887283 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 1.827139575e7 | 4.9615768614305376 | 8.800016e6 | 200001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.07281139e7 | 27.42385776909535 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.528611327e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 3.682598214e7 | 17.265589864767904 | 6.8000224e7 | 150006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.95935319e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.154310845e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.9048489215789473e8 | 9.40916957906159 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 2.74983665e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 2.450827266e7 | 31.409501212973517 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 4.549590695e7 | 23.710204718302855 | 8.0000016e7 | 2.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.5992796905e8 | 5.4413161963279615 | 6.4000144e7 | 1.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.15460514e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.41074345e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.00245735e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.41124616e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 536125.56 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.95693695e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 3.53788309e6 | 8.320331918831116 | 5.600144e6 | 100003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.3917795e7 | 16.587959949278147 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.7670120283333334e8 | 7.144219417269143 | 1.04000192e8 | 2.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.387500815e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.041422637e7 | 21.146515266424938 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 3.314964483e7 | 17.545293224423887 | 5.4400224e7 | 150006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 3.86509499e7 | 15.152800233299626 | 6.4000144e7 | 1.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 2.849593061e7 | 25.766059665745228 | 7.2000016e7 | 200001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.24455637e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.647001236e7 | 28.209894681866064 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.478668835e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 1.1159096851111111e8 | 6.545365081944792 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 1.97503813e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.925911966e7 | 18.016306709551454 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 4.808117518e7 | 12.507624687294609 | 8.8000192e7 | 1.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 2.751320273e7 | 24.820410671362087 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.15475221e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.155497029e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.198677323e7 | 5.25541774005131 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 2.55464015e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.577532637e7 | 33.14809412960407 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.643814488e7 | 9.313771397472832 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.12923456e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20562114e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 3.117165414e7 | 12.126448158993266 | 5.6000144e7 | 1.000003e6 |
| `(:sumlinear,Array{Int64,2},100)` | 2.74751823e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,JLD.UnsupportedType,100)` | 1.769426411e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.154362759e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.05469323e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.38442737e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.696297174e7 | 23.411107536482206 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 5.004953692e7 | 12.533550684351557 | 8.8000192e7 | 1.500006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.770058343e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 4.018938384e7 | 25.4603495571033 | 8.0000016e7 | 2.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 1.44116828e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 1.965703956e7 | 7.162792739941158 | 1.2000016e7 | 300001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.703115128e7 | 22.454156309068097 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.15479492e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.90220859e7 | 22.610071390382032 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 3.28670195e6 | 8.503877751074713 | 5.600144e6 | 100003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.75351806e6 | 23.652826971330843 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 3.07284543e7 | 13.796989748778445 | 4.8000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.385216975e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.9593518e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.387140284e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 3.279331151e7 | 17.650026883621248 | 5.4400224e7 | 150006.0 |
| `(:sumrange,Array{Int64,2},100)` | 2.559983297e7 | 31.736389322441845 | 1.28000016e8 | 200001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.746723237e7 | 20.173973266575157 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.638719488e7 | 18.893636971024026 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 1.9786371195918366e8 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.965076736315789e8 | 8.956927461553258 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 2.723539214e7 | 25.25578340461272 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 560263.28 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.694920769e7 | 28.37919293793727 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 2.87353457e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.15430919e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.155503311e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.43707302e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.25736118e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.3283807044871795e8 | 9.632849623242578 | 9.6000016e7 | 2.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 2.954648602e7 | 12.67771133661536 | 5.6000144e7 | 1.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 2.876642842e7 | 25.24836783955713 | 7.2000016e7 | 200001.0 |
| `(:sumvector,BitArray{2},100)` | 1.600673049e7 | 4.6361825502489005 | 6.400144e6 | 150003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.154320856e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.972141529e7 | 26.30733195561166 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.763830131e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.74707539e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.12955716e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 2.207643891e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.43672792e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.551303588e7 | 33.82955128118886 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 5.355456852e7 | 16.51886042655997 | 8.8000192e7 | 1.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 4.575207992e7 | 9.56938295400599 | 4.0000224e7 | 200006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 1.0142242657731959e8 | 27.235372920725464 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 3.729907315e7 | 20.407835559108356 | 8.8000016e7 | 2.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 1.15429105e6 | 0.0 | 16.0 | 1.0 |

