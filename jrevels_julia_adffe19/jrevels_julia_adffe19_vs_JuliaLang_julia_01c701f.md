# Benchmark Report

## Properties

*Job:* jrevels/julia@adffe19 vs JuliaLang/julia@01c701f

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195007)

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
| `(:sumvector,Array{Int64,2},100)` | 4.17823364e6 | 11.013847117369018 | 6.400144e6 | 100003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.288748894e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.850633587e7 | 14.781459141859557 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 1.354351614e7 | 6.647351455906379 | 8.800016e6 | 200001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.042975627e7 | 27.647776194009865 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.538986161e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 3.734628335e7 | 17.01031561644282 | 6.8000224e7 | 150006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.25306068e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.15434081e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.956597423333333e8 | 9.183317379994332 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 1.306819815e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 2.455645879e7 | 28.632460365634316 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 4.24665009e7 | 24.217627039482643 | 8.0000016e7 | 2.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.1273057451685393e8 | 7.459635643099855 | 6.4000144e7 | 1.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.45442652e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.395028743e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.004353056e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.41148904e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 534853.46 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.23645473e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 4.27993461e6 | 10.822457972611602 | 6.400144e6 | 100003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.772521816e7 | 15.764772618236583 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.3681350763157895e8 | 9.328149877915152 | 1.04000192e8 | 2.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.383105386e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.261137276e7 | 19.54575086882004 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 3.393549169e7 | 17.588741417398595 | 5.5200224e7 | 200006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 3.91552682e7 | 14.91516230908307 | 6.4000144e7 | 1.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 2.886798986e7 | 25.755882034878685 | 7.2000016e7 | 200001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.24739152e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.675985699e7 | 28.079926027473373 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.555708676e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 1.1153118755555555e8 | 6.527527476967944 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 1.97568211e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 6.206378769e7 | 18.232314397872678 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 5.044736478e7 | 11.78707975512966 | 8.8000192e7 | 1.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 2.441539156e7 | 31.61332854475883 | 1.24800016e8 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.15466625e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.155739784e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.224744422e7 | 5.290611769317961 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 1.17475146e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.563274708e7 | 34.34872584505724 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.626856695e7 | 9.586921057276989 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.1293783e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20564519e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Int64,2},100)` | 2.76714809e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 3.855286816e7 | 15.861750310800035 | 6.4000144e7 | 1.000003e6 |
| `(:sumelt,JLD.UnsupportedType,100)` | 1.156663756e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.154346896e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.10552145e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.387768684e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.567690537e7 | 23.567037516398617 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 5.341032489e7 | 18.411326760942124 | 9.6000192e7 | 2.000006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.772110324e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 4.231897292e7 | 24.138362214398548 | 8.0000016e7 | 2.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 821391.29 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 1.454744338e7 | 9.196563031551994 | 1.2000016e7 | 300001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.66923173e7 | 22.51265173683431 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.15467917e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.742129139e7 | 22.446622602334976 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 3.3585319e6 | 9.00470721331682 | 5.600144e6 | 100003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.51976984e6 | 24.072768347777426 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 2.75329387e7 | 9.318215914640373 | 5.6000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.387290997e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.25687751e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.386646987e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 3.348927889e7 | 17.313540646136264 | 5.4400224e7 | 150006.0 |
| `(:sumrange,Array{Int64,2},100)` | 2.57112081e7 | 32.298258112609105 | 1.28000016e8 | 200001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.686130804e7 | 20.695407487874178 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.678824138e7 | 18.841460888095924 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 2.7491187e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.062503274444444e8 | 8.779935224528737 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 2.745839533e7 | 25.229850954099405 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 538743.44 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.722684055e7 | 28.474988976476368 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 2.84762825e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.15429001e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.157844202e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.41140599e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.25772747e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.2407889042307693e8 | 10.08613492612684 | 9.6000016e7 | 2.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 2.984371764e7 | 12.659922893890094 | 5.6000144e7 | 1.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 2.889007646e7 | 25.592797622378573 | 7.2000016e7 | 200001.0 |
| `(:sumvector,BitArray{2},100)` | 1.104803955e7 | 6.412482984112557 | 6.400144e6 | 150003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.156352281e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.929044878e7 | 26.315985475737097 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.765880216e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.7474686e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.1290458e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 1.959960241e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.41137345e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.518614296e7 | 32.81892215097255 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 5.269435444e7 | 16.06876705197971 | 8.8000192e7 | 1.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 4.095910062e7 | 10.730058062708709 | 4.0000224e7 | 200006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 1.0167342184536083e8 | 27.048088453258977 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 3.950232367e7 | 19.26757713029246 | 8.8000016e7 | 2.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 2.042489017e7 | 0.0 | 16.0 | 1.0 |

