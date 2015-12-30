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
| `(:sumvector,Array{Int64,2},100)` | **(true,3.938952596640574)** | (false,0.4703597947175535) | **(true,1.3749915626898395)** | **(true,1.999970000899973)** |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9618404777992208) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100000)` | (false,0.9413198527509815) | **(true,1.070663936698182)** | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100)` | **(true,3.233516276263936)** | (false,0.34112276351324905) | (false,0.9090910743798648) | (false,0.7500012499937501) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9637105624482415) | (false,0.9653947268405455) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100)` | (false,1.0166592870915279) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100)` | **(true,1.2654991458985008)** | (false,0.8843410564823923) | (false,1.035294001384466) | **(true,1.666640001066624)** |
| `(:sumeach,BitArray{2},100000)` | (false,1.01130084509126) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100)` | (false,1.000013942846625) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9669515824210323) | (false,0.9784432194041799) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100)` | (false,0.22953201132727422) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100)` | **(true,1.0586671576447424)** | (false,1.044680104079261) | (false,1.0) | (false,1.0) |
| `(:sumrange,JLD.UnsupportedType,100000)` | **(true,3.3941983373968982)** | (false,0.39999800996636686) | **(true,1.272727223140505)** | **(true,1.499999750000125)** |
| `(:sumvector,BitArray{2},100000)` | **(true,1.5315937464001839)** | (false,0.8997206121212034) | **(true,1.3749991562518984)** | **(true,1.666665333336)** |
| `(:sumelt,Array{Float32,2},100000)` | (false,1.0179098038363767) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | **(true,1.1299918389432286)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100)` | (false,0.9997009997400172) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9705369320207068) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100000)` | (false,0.9072708821952951) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100000)` | (false,0.9184535996779025) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100)` | **(true,2.605261678996984)** | (false,0.5304890958487437) | **(true,1.2499943751265596)** | **(true,1.999970000899973)** |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.088797273822036)** | (false,0.9942323403997569) | (false,1.0) | (false,1.0) |
| `(:sumlogical,BitArray{2},100000)` | **(true,1.454766283047594)** | (false,0.8529002691806186) | **(true,1.2307688047345144)** | **(true,1.4999985000045)** |
| `(:sumcartesian,JLD.UnsupportedType,100)` | (false,1.0373207604622565) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9828594807397529) | (false,1.007181476861986) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100)` | **(true,1.3045679761449025)** | (false,0.8560387041294707) | (false,1.035294001384466) | **(true,1.666640001066624)** |
| `(:sumvector,Array{Int64,2},100000)` | **(true,4.111137415633095)** | (false,0.37877677820105715) | **(true,1.3749991562518984)** | **(true,1.999997000009)** |
| `(:sumrange,Array{Float32,2},100)` | **(true,1.4830291601927488)** | (false,0.7293933646633689) | (false,1.0333333259259276) | **(true,1.4999975000124999)** |
| `(:sumelt,Array{Int64,2},100)` | (false,1.0006367473575206) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9578516718811495) | (false,0.9616076569578028) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9962307298149127) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100000)` | (false,0.6205920593267146) | **(true,1.4883839954866862)** | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100000)` | (false,0.9660210834036431) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9834412938596947) | **(true,1.0534721482891043)** | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100000)` | **(true,2.8923781091299263)** | (false,0.4573063072092591) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumcolon,JLD.UnsupportedType,100)` | **(true,1.3852857403002437)** | (false,0.5847290777351674) | (false,0.5512821088099861) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100000)` | (false,1.0002975907142064) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100)` | (false,1.0001165959791807) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9751577366793165) | (false,1.0301451186712913) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100000)` | (false,0.424272721781195) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0087930992757475) | (false,0.9410905930698827) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100000)` | (false,0.8934507719815107) | **(true,1.1777905130371935)** | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9645651401834836) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100000)` | (false,1.0153524505517588) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100000)` | **(true,2.7437209625855647)** | (false,0.44255481778962935) | **(true,1.2499994375012655)** | **(true,1.999997000009)** |
| `(:sumlinear,Array{Int64,2},100)` | (false,1.0080453287420341) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100)` | (false,0.6797359077253785) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100)` | (false,1.0000147444111085) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | (false,1.034335534712022) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9966008892030428) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9785866934790755) | (false,1.0161950882462571) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100000)` | **(true,3.0430501179158056)** | (false,0.4484858328790407) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.984655633642738) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Float32,2},100000)` | **(true,2.915085386950186)** | (false,0.42084842397504396) | **(true,1.299999940000012)** | **(true,1.499999750000125)** |
| `(:sumelt,Array{Int64,2},100000)` | (false,0.9699060984345408) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100)` | **(true,3.7324244156770576)** | (false,0.3242838373512725) | **(true,1.1333331555557926)** | **(true,1.166666111112963)** |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9716065952118799) | (false,0.9494151599767804) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0325624208865347) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9552523917858642) | (false,0.9631362683072648) | (false,1.0) | (false,1.0) |
| `(:sumvector,Array{Float32,2},100)` | **(true,3.4656543688388326)** | (false,0.6533357451026816) | **(true,1.42856040844664)** | **(true,1.999970000899973)** |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9626882185979119) | (false,1.0060703979757493) | (false,1.0) | (false,1.0) |
| `(:sumcolon,JLD.UnsupportedType,100000)` | (false,0.9811278394591347) | **(true,1.731419375656394)** | (false,0.857142897959172) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100)` | (false,1.0027807016649726) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100000)` | (false,1.0090894478858967) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.996499618035267) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100)` | **(true,1.1803981538818664)** | (false,0.9333610376514236) | (false,1.0441174653986718) | **(true,1.666640001066624)** |
| `(:sumrange,Array{Int64,2},100)` | **(true,1.5984080649354941)** | (false,0.6429643903150024) | (false,1.0187499976562502) | **(true,1.4999975000124999)** |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9886122944913813) | **(true,1.0529151751443362)** | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9596213840545339) | **(true,1.054881664426058)** | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100)` | (false,0.9711547719561198) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9684077628129278) | (false,1.03591802260764) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100)` | **(true,1.1793654689325284)** | (false,0.863799912854635) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Int64,2},100000)` | (false,1.0386528711782335) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0011843280847337) | (false,1.0063357071141108) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100000)` | (false,0.4166209076030572) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100000)` | (false,1.000099350535932) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,BitArray{2},100)` | (false,0.9999436514612682) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.8415707452763596) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9481521428318768) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100000)` | **(true,1.2127135634465545)** | (false,0.9676470879883574) | **(true,1.2499999583333403)** | **(true,1.399999840000064)** |
| `(:sumvector,Array{Float32,2},100000)` | **(true,3.7774155637855196)** | (false,0.49239048446139994) | **(true,1.428570326533446)** | **(true,1.999997000009)** |
| `(:sumrange,JLD.UnsupportedType,100)` | **(true,1.9656735028068844)** | (false,0.5539581507904758) | (false,1.0249999968750003) | **(true,1.7499962500187498)** |
| `(:sumvector,BitArray{2},100)` | **(true,1.5275688418931488)** | (false,0.9910414623954849) | **(true,1.3749915626898395)** | **(true,1.6666533335999947)** |
| `(:sumelt,Array{Float32,2},100)` | (false,1.0000340983518663) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9558522791627831) | (false,1.0450836474413334) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0040809290803547) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100)` | (false,1.0006384210719639) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100000)` | **(true,1.0962083512603849)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100)` | (false,0.9891767159336359) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.8815904651222123) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0009623451081902) | (false,0.9707661149576161) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100000)` | **(true,2.6208159139495804)** | (false,0.5185366496400141) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumlogical,BitArray{2},100)` | **(true,1.121374761481401)** | (false,0.9880822950970435) | **(true,1.0599996640018816)** | **(true,1.4999850004499864)** |
| `(:sumrange,Array{Int64,2},100000)` | **(true,3.578147677646629)** | (false,0.37899145748065743) | **(true,1.272727223140505)** | **(true,1.499999750000125)** |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9337133276710511) | (false,0.9768017191232935) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100000)` | **(true,40.7984449524823)** | (false,1.0) | (false,1.0) | (false,1.0) |

