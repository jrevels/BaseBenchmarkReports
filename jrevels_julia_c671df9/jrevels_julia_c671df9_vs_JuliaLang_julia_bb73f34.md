# Benchmark Report

## Properties

*Job:* jrevels/julia@c671df9 vs JuliaLang/julia@bb73f34

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2#issuecomment-167877739)

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
| `(:sumvector,Array{Int64,2},100)` | 1.62473188e7 | 5.301843863656548 | 8.800144e6 | 200003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.236885388e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.704338867e7 | 15.950918157543331 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 4.406098794e7 | 2.1004889912229188 | 8.000016e6 | 150001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.962552949e7 | 27.278328988456852 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.228159765e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 5.266999384e7 | 13.286457598292486 | 7.0400224e7 | 250006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.25721157e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.154371474e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.7452869555e8 | 9.1361069758517 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 2.77020174e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 2.61603233e7 | 29.328817389686847 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 1.3336633906849316e8 | 7.770407785131747 | 1.12000016e8 | 3.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.6798127263793105e8 | 7.076954952470599 | 8.8000144e7 | 2.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.17516388e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.748390245e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.004250605e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.36001472e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 489793.96 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.59146832e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 1.144267463e7 | 5.625265367395231 | 8.000144e6 | 200003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.696513797e7 | 16.844675257900946 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.830051834528302e8 | 8.594148422957518 | 1.28000192e8 | 3.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.22865272e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.009586585e7 | 22.21822513880153 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 5.449124987e7 | 12.920610999504625 | 7.0400224e7 | 250006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 1.5924210173770493e8 | 5.677657531861575 | 8.8000144e7 | 2.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 4.226929134e7 | 18.520947822777323 | 7.4400016e7 | 300001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.26838861e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.626004888e7 | 27.704396784979004 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.38904281e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 8.058865757e7 | 8.664197879668107 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 2.18056333e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 6.224360533e7 | 17.514630820089906 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 1.4873728958461538e8 | 5.684834956589585 | 1.12000192e8 | 2.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 3.922094397e7 | 17.338875224468243 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.154647e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.155843558e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.106430609e7 | 5.407088848829318 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 489754.63 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.613369309e7 | 30.505202560398175 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.400896926e7 | 11.125908878259109 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.07828175e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20592382e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Int64,2},100)` | 2.7679518e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 1.103932027159091e8 | 6.5100655618605465 | 8.0000144e7 | 2.000003e6 |
| `(:sumelt,JLD.UnsupportedType,100)` | 7.84766402e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.154352712e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.02786043e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.381998491e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.431056157e7 | 24.45732832723335 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 1.5335728044615385e8 | 5.74742092948093 | 1.12000192e8 | 2.500006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.772213333e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 1.1837951246428572e8 | 10.787631564043727 | 1.04000016e8 | 3.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 821204.46 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 5.448751693e7 | 2.99482181456817 | 1.3600016e7 | 350001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.607516226e7 | 22.058320590777345 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.19908314e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.342069049e7 | 22.602323306554595 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 1.140749247e7 | 5.877035802695863 | 8.000144e6 | 200003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.24509419e6 | 24.762373473341523 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 2.893363236e7 | 14.928393875326687 | 4.8000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.390968911e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.25529915e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.381636018e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 4.48364307e7 | 13.917459554536032 | 5.6800224e7 | 250006.0 |
| `(:sumrange,Array{Int64,2},100)` | 4.135982701e7 | 19.8082757820955 | 1.30400016e8 | 300001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.670965429e7 | 21.474474836089236 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.81300485e7 | 18.359716617554216 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 1.8828110592307693e8 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.9404252331578946e8 | 8.933839253623235 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 3.206409497e7 | 21.29017132363312 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 499569.7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.695807688e7 | 28.295636729345148 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 1.18642879e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.15461275e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.157675522e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.05311947e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.31083846e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.730453425e8 | 8.743131413218359 | 1.20000016e8 | 3.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 1.1146978910344827e8 | 6.379971056695107 | 8.0000144e7 | 2.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 5.120590516e7 | 16.91928877904202 | 1.31200016e8 | 350001.0 |
| `(:sumvector,BitArray{2},100)` | 1.680725804e7 | 6.578111412595663 | 8.800144e6 | 250003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.156400305e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.500440795e7 | 27.387630062140676 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.773143994e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.74816961e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.33448844e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 1.981489767e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.14863113e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.544530256e7 | 30.99925282528831 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 1.2815842474025974e8 | 8.882258609973794 | 1.12000192e8 | 2.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 5.203338512e7 | 9.223662009404208 | 4.2400224e7 | 300006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.562063693e7 | 27.33790771061544 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 1.3350437541666667e8 | 7.643387749746649 | 1.12000016e8 | 3.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 1.99081932e7 | 0.0 | 16.0 | 1.0 |

