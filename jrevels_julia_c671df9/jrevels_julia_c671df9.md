# Benchmark Report

## Properties

*Job:* jrevels/julia@c671df9

*Tag Predicate:* `"arrays"`

*Triggered By:* [link](https://github.com/jrevels/julia/pull/2)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JSON file in this directory. Note that it's technically possible
for this JSON data to get out of sync with the below table. This would only happen in case
of a network error during the job, and as such is very unlikely. Just in case, you can always
verify that they are synced up by checking the commit history of both files.


| Benchmark ID | time (ns) | % of time spent in GC | bytes allocated | number of allocations |
|--------------|-----------|-----------------------|-----------------|-----------------------|
| `(:sumvector,Array{Int64,2},100)` | 1.62179765e7 | 5.085149779279719 | 8.800144e6 | 200003.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.236439599e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Float32,2},100000)` | 2.68758299e7 | 15.851635512376552 | 4.8000016e7 | 1.000001e6 |
| `(:sumcolon,BitArray{2},100)` | 4.381779883e7 | 2.0770959383790695 | 8.000016e6 | 150001.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.00122829e7 | 26.528704766676263 | 9.6000016e7 | 2.000001e6 |
| `(:sumcartesian,Array{Int64,2},100)` | 1.286245173e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Int64,2},100)` | 5.276931283e7 | 13.286897645397183 | 7.0400224e7 | 250006.0 |
| `(:sumeach,BitArray{2},100000)` | 1.25694739e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,Array{Float32,2},100)` | 1.15431192e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.7463599615e8 | 9.070208406471018 | 4.79182416e8 | 2.9948901e7 |
| `(:sumeach,JLD.UnsupportedType,100)` | 2.74865767e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,Array{Int64,2},100)` | 3.035056358e7 | 27.863139487238943 | 1.24800016e8 | 100001.0 |
| `(:sumrange,JLD.UnsupportedType,100000)` | 1.4948006977272728e8 | 6.840785795961313 | 1.12000016e8 | 3.000001e6 |
| `(:sumvector,BitArray{2},100000)` | 1.7000170440350878e8 | 6.929919581596394 | 8.8000144e7 | 2.500003e6 |
| `(:sumelt,Array{Float32,2},100000)` | 1.15447535e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.402516543e7 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100)` | 1.007352895e7 | 0.2226951699653906 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.38673147e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100000)` | 462308.0 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100000)` | 2.59643967e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100)` | 1.163034896e7 | 5.645626734605031 | 8.000144e6 | 200003.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.348034842e7 | 17.721198240169926 | 8.8000016e7 | 1.500001e6 |
| `(:sumlogical,BitArray{2},100000)` | 1.827171111698113e8 | 8.469229540701605 | 1.28000192e8 | 3.000006e6 |
| `(:sumcartesian,JLD.UnsupportedType,100)` | 1.228879964e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.002409769e7 | 21.796696394983474 | 2.0000144e7 | 400003.0 |
| `(:sumlogical,JLD.UnsupportedType,100)` | 5.411313531e7 | 12.992244743313528 | 7.0400224e7 | 250006.0 |
| `(:sumvector,Array{Int64,2},100000)` | 1.5864391806557378e8 | 5.583754891764365 | 8.8000144e7 | 2.000003e6 |
| `(:sumrange,Array{Float32,2},100)` | 4.29525539e7 | 18.891851844622483 | 7.4400016e7 | 300001.0 |
| `(:sumelt,Array{Int64,2},100)` | 6.24624952e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.665766848e7 | 28.196228751807258 | 7.2000016e7 | 150001.0 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.387764456e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,BitArray{2},100000)` | 8.048549657e7 | 8.564861218628067 | 6.4000016e7 | 1.500001e6 |
| `(:sumcartesian,Array{Int64,2},100000)` | 2.39088949e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 6.152312179e7 | 17.677282883120377 | 1.09600224e8 | 450006.0 |
| `(:sumlogical,Array{Int64,2},100000)` | 1.4416505462686568e8 | 5.833247579872656 | 1.12000192e8 | 2.500006e6 |
| `(:sumcolon,JLD.UnsupportedType,100)` | 3.872737526e7 | 17.384678225918833 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Float32,2},100000)` | 1.15438483e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100)` | 1.157682321e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 4.1059817e7 | 5.330459514392536 | 2.4000016e7 | 1.500001e6 |
| `(:sumeach,JLD.UnsupportedType,100000)` | 493263.24 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.5970274e7 | 32.58647459435721 | 1.29600016e8 | 200001.0 |
| `(:sumcolon,Array{Int64,2},100000)` | 2.364675449e7 | 10.906416036238697 | 5.6000016e7 | 1.000001e6 |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.07795573e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,BitArray{2},100000)` | 1.20573506e6 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,JLD.UnsupportedType,100000)` | 1.106426159090909e8 | 6.342591552476419 | 8.0000144e7 | 2.000003e6 |
| `(:sumlinear,Array{Int64,2},100)` | 2.74710704e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,JLD.UnsupportedType,100)` | 7.85679388e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100)` | 1.156342534e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | 2.02774303e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.379513528e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.396694419e7 | 23.874811334153677 | 2.00000144e8 | 4.000003e6 |
| `(:sumlogical,JLD.UnsupportedType,100000)` | 1.4471619441791046e8 | 5.887936540229618 | 1.12000192e8 | 2.500006e6 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.806837002e7 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,Array{Float32,2},100000)` | 1.1811943540476191e8 | 10.770189723520964 | 1.04000016e8 | 3.000001e6 |
| `(:sumelt,Array{Int64,2},100000)` | 821094.81 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100)` | 5.425103747e7 | 3.0163314921724873 | 1.3600016e7 | 350001.0 |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.574141841e7 | 22.132061930973997 | 8.0000016e7 | 1.500001e6 |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.18447667e6 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.115587776e7 | 22.726147444630573 | 2.08000192e8 | 4.500006e6 |
| `(:sumvector,Array{Float32,2},100)` | 1.139222224e7 | 5.564834007175505 | 8.000144e6 | 200003.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 9.29390347e6 | 24.143664528246518 | 1.9200144e7 | 400003.0 |
| `(:sumcolon,JLD.UnsupportedType,100000)` | 2.89230786e7 | 14.779689947054898 | 4.8000016e7 | 1.000001e6 |
| `(:sumcartesian,Array{Float32,2},100)` | 1.389238149e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,BitArray{2},100000)` | 1.25237432e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.382291374e7 | 0.0 | 16.0 | 1.0 |
| `(:sumlogical,Array{Float32,2},100)` | 4.475190718e7 | 13.953767016492606 | 5.6800224e7 | 250006.0 |
| `(:sumrange,Array{Int64,2},100)` | 4.155147943e7 | 20.499575245427565 | 1.30400016e8 | 300001.0 |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 3.692872704e7 | 21.010612129293236 | 1.04000016e8 | 2.000001e6 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 5.811629477e7 | 18.387395183586058 | 9.6000224e7 | 450006.0 |
| `(:sumlinear,JLD.UnsupportedType,100)` | 1.8823605976923078e8 | 0.0 | 16.0 | 1.0 |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 4.9363210331578946e8 | 8.776908891143318 | 4.78846416e8 | 2.9927901e7 |
| `(:sumcolon,Array{Float32,2},100)` | 3.195971362e7 | 21.02255155196144 | 6.8800016e7 | 100001.0 |
| `(:sumlinear,Array{Int64,2},100000)` | 486929.18 | 0.0 | 16.0 | 1.0 |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.679564582e7 | 28.120941577557502 | 7.3600016e7 | 200001.0 |
| `(:sumelt,JLD.UnsupportedType,100000)` | 1.18726742e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Float32,2},100000)` | 1.15440774e6 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,BitArray{2},100)` | 1.157732379e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.05310205e6 | 0.0 | 16.0 | 1.0 |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.30990979e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,BitArray{2},100000)` | 1.7350297510714287e8 | 8.722171744310543 | 1.20000016e8 | 3.500001e6 |
| `(:sumvector,Array{Float32,2},100000)` | 1.1162222793258427e8 | 6.210198761525413 | 8.0000144e7 | 2.000003e6 |
| `(:sumrange,JLD.UnsupportedType,100)` | 5.186320219e7 | 16.860380677317682 | 1.31200016e8 | 350001.0 |
| `(:sumvector,BitArray{2},100)` | 1.694142678e7 | 6.436060658659867 | 8.800144e6 | 250003.0 |
| `(:sumelt,Array{Float32,2},100)` | 1.154386174e7 | 0.0 | 16.0 | 1.0 |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 8.619333148e7 | 26.816164537982274 | 1.92000144e8 | 4.000003e6 |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 1.771191874e7 | 0.0 | 16.0 | 1.0 |
| `(:sumeach,Array{Int64,2},100)` | 2.76761858e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,Array{Float32,2},100000)` | 2.40557473e6 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,BitArray{2},100)` | 1.977601247e7 | 0.0 | 16.0 | 1.0 |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 2.05236321e6 | 0.0 | 16.0 | 1.0 |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | 2.551461368e7 | 31.425573724608697 | 1.28000016e8 | 150001.0 |
| `(:sumlogical,Array{Float32,2},100000)` | 1.2876193288157895e8 | 8.674343717192043 | 1.12000192e8 | 2.500006e6 |
| `(:sumlogical,BitArray{2},100)` | 5.127136574e7 | 9.334148876875448 | 4.2400224e7 | 300006.0 |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | 9.658100613e7 | 26.614744779415105 | 2.08000192e8 | 4.500006e6 |
| `(:sumrange,Array{Int64,2},100000)` | 1.486271375e8 | 6.830018367838821 | 1.12000016e8 | 3.000001e6 |
| `(:sumlinear,JLD.UnsupportedType,100000)` | 1.990760927e7 | 0.0 | 16.0 | 1.0 |

