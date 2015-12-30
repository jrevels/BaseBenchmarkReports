# Benchmark Report

Job: jrevels/julia@adffe19

Tag Predicate: "arrays"

Triggered By: [https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195672](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195672)

**Below is a table of this job's results.** If available, the data used to generate this
table can be found in the JSON file in this directory. Note that it's technically possible
for this JSON data to get out of sync with the below table. This would only happen in case
of a network error during the job, and as such is very unlikely. Just in case, you can always
verify that they are synced up by checking the commit history of both files.


| Benchmark ID | time (ns) | % of time spent in GC | bytes allocated | number of allocations |
|--------------|-----------|-----------------------|-----------------|-----------------------|

| (:sumvector,Array{Int64,2},100) | 4.16087697e6 | 11.173039218279458 | 6.400144e6 | 100003.0 |
| (:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 3.277918748e7 | 0.0 | 16.0 | 1.0 |
| (:sumeach,JLD.UnsupportedType,100) | 3.47976212e6 | 0.0 | 16.0 | 1.0 |
| (:sumcolon,Array{Float32,2},100000) | 2.855608467e7 | 14.96976957992696 | 4.8000016e7 | 1.000001e6 |
| (:sumcolon,BitArray{2},100) | 1.34940287e7 | 6.482232356104886 | 8.800016e6 | 200001.0 |
| (:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 4.056529145e7 | 27.82034433884066 | 9.6000016e7 | 2.000001e6 |
| (:sumcartesian,Array{Int64,2},100) | 1.20852136e7 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,Array{Int64,2},100) | 3.712817352e7 | 17.22530528665369 | 6.8000224e7 | 150006.0 |
| (:sumrange,JLD.UnsupportedType,100000) | 4.270999989e7 | 23.973452746529137 | 8.0000016e7 | 2.000001e6 |
| (:sumeach,BitArray{2},100000) | 1.24128844e6 | 0.0 | 16.0 | 1.0 |
| (:sumlinear,Array{Float32,2},100) | 1.154337187e7 | 0.0 | 16.0 | 1.0 |
| (:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 4.899187351052632e8 | 9.37056549289201 | 4.79182416e8 | 2.9948901e7 |
| (:sumvector,JLD.UnsupportedType,100) | 3.6075119e6 | 8.500041140817466 | 5.600144e6 | 100003.0 |
| (:sumcolon,Array{Int64,2},100) | 2.399698914e7 | 34.560311492939434 | 1.24800016e8 | 100001.0 |
| (:sumcartesian,JLD.UnsupportedType,100) | 1.386827297e7 | 0.0 | 16.0 | 1.0 |
| (:sumvector,BitArray{2},100000) | 1.130892206744186e8 | 7.421035710966999 | 6.4000144e7 | 1.500003e6 |
| (:sumelt,Array{Float32,2},100000) | 1.1544346e6 | 0.0 | 16.0 | 1.0 |
| (:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.394287619e7 | 0.0 | 16.0 | 1.0 |
| (:sumelt,BitArray{2},100) | 1.004687614e7 | 0.0 | 16.0 | 1.0 |
| (:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.41161723e6 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,JLD.UnsupportedType,100) | 3.33012083e7 | 17.401265844749425 | 5.4400224e7 | 150006.0 |
| (:sumeach,Array{Int64,2},100000) | 570584.9 | 0.0 | 16.0 | 1.0 |
| (:sumcartesian,BitArray{2},100000) | 2.26321014e6 | 0.0 | 16.0 | 1.0 |
| (:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 3.366912971e7 | 16.685607412342517 | 8.8000016e7 | 1.500001e6 |
| (:sumlogical,BitArray{2},100000) | 1.2817958675e8 | 9.604312574907285 | 1.04000192e8 | 2.000006e6 |
| (:sumcolon,JLD.UnsupportedType,100) | 2.766790899e7 | 24.740981749507885 | 6.8800016e7 | 100001.0 |
| (:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.03252675e7 | 21.570004946003614 | 2.0000144e7 | 400003.0 |
| (:sumvector,Array{Int64,2},100000) | 3.882604481e7 | 15.030574457380716 | 6.4000144e7 | 1.000003e6 |
| (:sumrange,Array{Float32,2},100) | 2.866185222e7 | 25.74638849510712 | 7.2000016e7 | 200001.0 |
| (:sumelt,Array{Int64,2},100) | 6.2662166e6 | 0.0 | 16.0 | 1.0 |
| (:sumeach,JLD.UnsupportedType,100000) | 2.53411328e6 | 0.0 | 16.0 | 1.0 |
| (:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 2.657693671e7 | 28.125516668558344 | 7.2000016e7 | 150001.0 |
| (:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.523223501e7 | 0.0 | 16.0 | 1.0 |
| (:sumcolon,BitArray{2},100000) | 1.4160859421875e8 | 5.425984420937671 | 6.4000016e7 | 1.500001e6 |
| (:sumcartesian,Array{Int64,2},100000) | 1.9756775e6 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 5.886451902e7 | 18.22281857664554 | 1.09600224e8 | 450006.0 |
| (:sumlogical,Array{Int64,2},100000) | 4.823412193e7 | 12.290115513305102 | 8.8000192e7 | 1.500006e6 |
| (:sumlinear,Array{Float32,2},100000) | 1.15449832e6 | 0.0 | 16.0 | 1.0 |
| (:sumlinear,BitArray{2},100) | 1.155682366e7 | 0.0 | 16.0 | 1.0 |
| (:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 4.179584786e7 | 5.397210346054352 | 2.4000016e7 | 1.500001e6 |
| (:sumvector,JLD.UnsupportedType,100000) | 3.119262823e7 | 12.415768945332122 | 5.6000144e7 | 1.000003e6 |
| (:sumelt,JLD.UnsupportedType,100) | 1.785153158e7 | 0.0 | 16.0 | 1.0 |
| (:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 2.594130688e7 | 33.50273646949089 | 1.29600016e8 | 200001.0 |
| (:sumcolon,Array{Int64,2},100000) | 2.639087495e7 | 9.545885612591245 | 5.6000016e7 | 1.000001e6 |
| (:sumcartesian,JLD.UnsupportedType,100000) | 2.04704858e6 | 0.0 | 16.0 | 1.0 |
| (:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.1297476e6 | 0.0 | 16.0 | 1.0 |
| (:sumelt,BitArray{2},100000) | 1.2059541e6 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,JLD.UnsupportedType,100000) | 5.071916641e7 | 12.42402945212069 | 8.8000192e7 | 1.500006e6 |
| (:sumlinear,Array{Int64,2},100) | 2.74623169e6 | 0.0 | 16.0 | 1.0 |
| (:sumeach,Array{Float32,2},100) | 1.154305581e7 | 0.0 | 16.0 | 1.0 |
| (:sumcolon,JLD.UnsupportedType,100000) | 3.072836969e7 | 13.915849246344534 | 4.8000016e7 | 1.000001e6 |
| (:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 9.541765081e7 | 23.936353535065912 | 2.00000144e8 | 4.000003e6 |
| (:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.386507576e7 | 0.0 | 16.0 | 1.0 |
| (:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.772231746e7 | 0.0 | 16.0 | 1.0 |
| (:sumrange,Array{Float32,2},100000) | 4.029359632e7 | 25.430482023327727 | 8.0000016e7 | 2.000001e6 |
| (:sumelt,Array{Int64,2},100000) | 821261.46 | 0.0 | 16.0 | 1.0 |
| (:sumrange,BitArray{2},100) | 1.452488019e7 | 9.321130425193983 | 1.2000016e7 | 300001.0 |
| (:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 3.703068479e7 | 22.84293199074249 | 8.0000016e7 | 1.500001e6 |
| (:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.175888e6 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 9.803507706e7 | 22.41088024464362 | 2.08000192e8 | 4.500006e6 |
| (:sumlinear,JLD.UnsupportedType,100) | 1.973128226530612e8 | 0.0 | 16.0 | 1.0 |
| (:sumvector,Array{Float32,2},100) | 3.30346312e6 | 8.569054129003895 | 5.600144e6 | 100003.0 |
| (:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 9.57925695e6 | 24.08916927221874 | 1.9200144e7 | 400003.0 |
| (:sumcartesian,Array{Float32,2},100) | 1.387383684e7 | 0.0 | 16.0 | 1.0 |
| (:sumlinear,BitArray{2},100000) | 1.25643413e6 | 0.0 | 16.0 | 1.0 |
| (:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.388639802e7 | 0.0 | 16.0 | 1.0 |
| (:sumlogical,Array{Float32,2},100) | 3.301204805e7 | 17.484103782500068 | 5.4400224e7 | 150006.0 |
| (:sumelt,JLD.UnsupportedType,100000) | 2.84715738e6 | 0.0 | 16.0 | 1.0 |
| (:sumrange,Array{Int64,2},100) | 2.581981991e7 | 31.561167090496294 | 1.28000016e8 | 200001.0 |
| (:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 3.70102946e7 | 20.57160270018789 | 1.04000016e8 | 2.000001e6 |
| (:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 5.606881245e7 | 19.0389713720611 | 9.6000224e7 | 450006.0 |
| (:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 5.023588018333333e8 | 8.918263589533279 | 4.78846416e8 | 2.9927901e7 |
| (:sumcolon,Array{Float32,2},100) | 2.735512595e7 | 25.07975101348412 | 6.8800016e7 | 100001.0 |
| (:sumlinear,Array{Int64,2},100000) | 542638.75 | 0.0 | 16.0 | 1.0 |
| (:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 2.702793444e7 | 28.36236402158978 | 7.3600016e7 | 200001.0 |
| (:sumrange,JLD.UnsupportedType,100) | 2.908736055e7 | 25.350114682011515 | 7.2000016e7 | 200001.0 |
| (:sumeach,Array{Float32,2},100000) | 1.15432804e6 | 0.0 | 16.0 | 1.0 |
| (:sumeach,BitArray{2},100) | 1.157681906e7 | 0.0 | 16.0 | 1.0 |
| (:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.41220361e6 | 0.0 | 16.0 | 1.0 |
| (:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.25746617e6 | 0.0 | 16.0 | 1.0 |
| (:sumrange,BitArray{2},100000) | 1.453141953939394e8 | 8.552252918006904 | 9.6000016e7 | 2.500001e6 |
| (:sumlinear,JLD.UnsupportedType,100000) | 1.15426413e6 | 0.0 | 16.0 | 1.0 |
| (:sumvector,Array{Float32,2},100000) | 2.977397785e7 | 12.905294391201231 | 5.6000144e7 | 1.000003e6 |
| (:sumvector,BitArray{2},100) | 1.132885519e7 | 6.067839920001214 | 6.400144e6 | 150003.0 |
| (:sumelt,Array{Float32,2},100) | 1.156428612e7 | 0.0 | 16.0 | 1.0 |
| (:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 8.919089339e7 | 26.55522890390618 | 1.92000144e8 | 4.000003e6 |
| (:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 1.948548265e7 | 0.0 | 16.0 | 1.0 |
| (:sumeach,Array{Int64,2},100) | 3.2373225e6 | 0.0 | 16.0 | 1.0 |
| (:sumcartesian,Array{Float32,2},100000) | 2.12920347e6 | 0.0 | 16.0 | 1.0 |
| (:sumcartesian,BitArray{2},100) | 1.96011578e7 | 0.0 | 16.0 | 1.0 |
| (:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 2.41111838e6 | 0.0 | 16.0 | 1.0 |
| (:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100) | 2.547148569e7 | 32.55843997075691 | 1.28000016e8 | 150001.0 |
| (:sumlogical,Array{Float32,2},100000) | 4.920669685e7 | 17.39919510760979 | 8.8000192e7 | 1.500006e6 |
| (:sumlogical,BitArray{2},100) | 4.090451177e7 | 10.593392554048126 | 4.0000224e7 | 200006.0 |
| (:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000) | 1.0147991165979381e8 | 27.251000467933267 | 2.08000192e8 | 4.500006e6 |
| (:sumrange,Array{Int64,2},100000) | 3.748463476e7 | 20.178287384210353 | 8.8000016e7 | 2.000001e6 |

