# Benchmark Report

## Properties

*Job:* jrevels/julia@adffe19

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/commit/adffe19dfb704444789429bffa51f4e05b386125#commitcomment-15195672)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory. Note that it's technically possible
for this JSON data to get out of sync with the below table. This would only happen in case
of a network error during the job, and as such is very unlikely. Just in case, you can always
verify that they are synced up by checking the commit history of both files.


| Benchmark ID | time (ns) | % of time spent in GC | bytes allocated | number of allocations |
|--------------|-----------|-----------------------|-----------------|-----------------------|
| `(:sumvector,Array{Int64,2},100)` | 4.20666783e6 | 11.125884554011776 | 6.400144e6 | 100003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.267490644e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.914310651e7 | 15.052050926122668 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 1.341001137e7 | 6.731452594495332 | 8.800016e6 | 200001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.124803624e7 | 27.899916396091683 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.737900411e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 3.722424884e7 | 17.457193240340008 | 6.8000224e7 | 150006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.24612683e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.154304152e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.254968474736842e8 | 9.974274164482129 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 2.76982515e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 2.498379796e7 | 29.233193726432212 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 4.321724615e7 | 24.1914197644756 | 8.0000016e7 | 2.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.1252138421839081e8 | 7.808874736056357 | 6.4000144e7 | 1.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.15430745e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.52230949e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.002383028e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.41115792e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 577156.36 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.23917144e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 3.59763849e6 | 8.45287062234045 | 5.600144e6 | 100003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.436638509e7 | 16.886021428891876 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.2739404036842105e8 | 10.149038240027703 | 1.04000192e8 | 2.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.38841808e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.038142143e7 | 22.526011755481328 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 3.477660991e7 | 18.93203137911135 | 5.4400224e7 | 150006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 3.914005979e7 | 15.237572820615505 | 6.4000144e7 | 1.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 2.987113605e7 | 26.996965721779432 | 7.2000016e7 | 200001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.24673596e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.782510458e7 | 29.602311680890107 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.54744329e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 1.3127902948e8 | 5.888302634588509 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 1.97607379e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.980822484e7 | 18.48097481390549 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 4.831432879e7 | 13.148583387136705 | 8.8000192e7 | 1.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 2.863641671e7 | 26.330120261057804 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.15441254e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.157707699e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.543813497e7 | 5.302200583579627 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 2.54095097e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.624041552e7 | 33.377748154091414 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.643307514e7 | 9.639542788074772 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.14965617e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20605848e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 3.177411585e7 | 12.175956881350814 | 5.6000144e7 | 1.000003e6 |
| `(:sumlinear,Array{Int64,2},100)` | 2.74805353e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,JLD.UnsupportedType,100)` | 1.788976698e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.156299239e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.05642407e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.384434866e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.63072951111111e7 | 23.721994388566834 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 5.063762819e7 | 12.935835868607674 | 8.8000192e7 | 1.500006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.772293078e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 4.097180635e7 | 25.434178450916807 | 8.0000016e7 | 2.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 820889.28 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 1.469282141e7 | 9.349401913734104 | 1.2000016e7 | 300001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.744432248e7 | 22.66129391788172 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.1546693e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.954523584848484e7 | 22.58406452415638 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 3.3120342e6 | 8.551032337823735 | 5.600144e6 | 100003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.58677596e6 | 24.701838620950145 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 3.094968272e7 | 14.23745356328214 | 4.8000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.385323531e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.24313748e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.386166349e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 3.445310665e7 | 18.98294445640515 | 5.4400224e7 | 150006.0 |
| `(:sumrange,Array{Int64,2},100)` | 2.613556804e7 | 31.553527327283742 | 1.28000016e8 | 200001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.763816835e7 | 20.359973071596855 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.975052489e7 | 20.367909130840555 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 2.2051281026530612e8 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.003471187368421e8 | 8.95884986375313 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 2.840321453e7 | 26.633167822763383 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 998525.57 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.966011581e7 | 30.722533835228788 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 2.87318824e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.16925849e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.157828992e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.43752212e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.25732908e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.495921717647059e8 | 8.656697857575079 | 9.6000016e7 | 2.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 2.981279463e7 | 12.985623350469375 | 5.6000144e7 | 1.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 3.021720991e7 | 26.762458546173836 | 7.2000016e7 | 200001.0 |
| `(:sumvector,BitArray{2},100)` | 1.122952254e7 | 6.306367075284594 | 6.400144e6 | 150003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.154398873e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.954949641e7 | 26.651679972425974 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.76573373e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.7480181e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.12922603e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 1.960115734e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.43697228e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.564945734e7 | 32.650476932054126 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 4.869839038e7 | 18.14785686380622 | 8.8000192e7 | 1.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 4.202164916e7 | 11.48476442116922 | 4.0000224e7 | 200006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 1.0259098706451613e8 | 28.511486064716223 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 3.759986725e7 | 20.478674681670693 | 8.8000016e7 | 2.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 1.15437246e6 | 0.0 | 16.0 | 1.0 |

