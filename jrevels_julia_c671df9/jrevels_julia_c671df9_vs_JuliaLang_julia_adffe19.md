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
| `(:sumvector,Array{Int64,2},100)` | **(true,3.326439169707404)** | (false,0.5650379280134399) | **(true,1.3749915626898395)** | **(true,1.999970000899973)** |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.976363803188836) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100000)` | (false,0.8968177001458426) | **(true,1.1665233063059386)** | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100)` | **(true,2.31641688974903)** | (false,0.44756611105103433) | (false,0.9090910743798648) | (false,0.7500012499937501) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9915123587385706) | (false,1.00581534900988) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100)` | (false,1.0161233878457772) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100)` | **(true,1.3354955912520112)** | (false,0.8144469789169408) | (false,1.035294001384466) | **(true,1.666640001066624)** |
| `(:sumeach,BitArray{2},100000)` | (false,0.9467965501545174) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100)` | (false,0.9987687480828283) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9839767000822741) | (false,1.0474288814472623) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100)` | (false,0.983516715025201) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100)` | **(true,1.0645611569166535)** | (false,0.9190169787657136) | (false,1.0) | (false,1.0) |
| `(:sumrange,JLD.UnsupportedType,100000)` | **(true,3.0901128716737727)** | (false,0.3333573939616766) | **(true,1.399999920000016)** | **(true,1.499999750000125)** |
| `(:sumvector,BitArray{2},100000)` | **(true,1.0649064130133794)** | **(true,1.3621353339705915)** | **(true,1.3749991562518984)** | **(true,1.666665333336)** |
| `(:sumelt,Array{Float32,2},100000)` | (false,0.9999787151265281) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | **(true,1.1817317214915088)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100)` | (false,1.0167977692911578) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9891126207486259) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100000)` | (false,0.8608137397543983) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100000)` | **(true,1.1390546975767113)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100)` | **(true,3.269892411780751)** | (false,0.7138053655043148) | **(true,1.42856040844664)** | **(true,1.999970000899973)** |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9831027743680164) | (false,1.034000605537121) | (false,1.0) | (false,1.0) |
| `(:sumlogical,BitArray{2},100000)` | **(true,1.113905460549174)** | **(true,1.161541688415167)** | **(true,1.2307688047345144)** | **(true,1.4999985000045)** |
| `(:sumcartesian,JLD.UnsupportedType,100)` | (false,0.897116007593287) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9403754947685382) | **(true,1.1191669628909044)** | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100)` | **(true,1.5234927659175233)** | (false,0.7800945498124162) | **(true,1.294116435991146)** | **(true,1.666640001066624)** |
| `(:sumvector,Array{Int64,2},100000)` | **(true,3.3570108870662105)** | (false,0.46188584962542) | **(true,1.3749991562518984)** | **(true,1.999997000009)** |
| `(:sumrange,Array{Float32,2},100)` | **(true,1.49899816972208)** | (false,0.751888236707265) | (false,1.0333333259259276) | **(true,1.4999975000124999)** |
| `(:sumelt,Array{Int64,2},100)` | (false,0.9961640457464899) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0122357911511117) | (false,1.0006665864253623) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.899200067934852) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100000)` | (false,0.5082063697258246) | **(true,1.981326980130036)** | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100000)` | **(true,1.1157720598521337)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0396063979470809) | (false,0.9764962832002784) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100000)` | **(true,2.90492084052571)** | (false,0.4789582370264422) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumcolon,JLD.UnsupportedType,100)` | **(true,1.3403417696448217)** | (false,0.8186836994935436) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100000)` | (false,0.9999496093302417) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100)` | (false,0.9985889551872937) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9844950462053212) | **(true,1.0756837136247586)** | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100000)` | (false,0.19654924085596995) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.024580573615286) | (false,0.9344051826307115) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100000)` | (false,0.8663322472125878) | **(true,1.1765332562507536)** | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9762625289318433) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100000)` | (false,1.0001233425518021) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100000)` | **(true,3.5890599610734526)** | (false,0.5504416821814366) | **(true,1.428570326533446)** | **(true,1.999997000009)** |
| `(:sumlinear,Array{Int64,2},100)` | (false,0.9783459711962651) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100)` | (false,0.43860484072621947) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100)` | (false,0.9987005639025759) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | (false,1.000070233526104) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9953322457258953) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9521275337223136) | **(true,1.1063617119170948)** | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100000)` | **(true,2.8173980941797034)** | (false,0.48286746775084743) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9990347095149757) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Float32,2},100000)` | **(true,2.8844478352051888)** | (false,0.45379095732692054) | **(true,1.299999940000012)** | **(true,1.499999750000125)** |
| `(:sumelt,Array{Int64,2},100000)` | (false,0.5703087463924653) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100)` | **(true,2.992588305228018)** | (false,0.4201764710328743) | **(true,1.1333331555557926)** | **(true,1.166666111112963)** |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9701226345250465) | (false,0.9664911616073283) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.011961905410022) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9444617697534903) | **(true,1.0741974599372923)** | (false,1.0) | (false,1.0) |
| `(:sumvector,Array{Float32,2},100)` | **(true,3.5292164836062843)** | (false,0.6811947280645254) | **(true,1.42856040844664)** | **(true,1.999970000899973)** |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9521961134186068) | **(true,1.0597663058685267)** | (false,1.0) | (false,1.0) |
| `(:sumcolon,JLD.UnsupportedType,100000)` | (false,0.8951831398362148) | **(true,1.1558048745403429)** | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100)` | (false,1.0025491923892382) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100000)` | (false,0.9953598438297709) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9949257014644369) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100)` | **(true,1.3719527384717707)** | (false,0.8350721397334666) | (false,1.0441174653986718) | **(true,1.666640001066624)** |
| `(:sumrange,Array{Int64,2},100)` | **(true,1.4951946592287528)** | (false,0.6395937955047171) | (false,1.0187499976562502) | **(true,1.4999975000124999)** |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | **(true,1.0570959263291144)** | (false,1.0249014841876614) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0109219424895937) | (false,1.0477472009578475) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100)` | (false,0.9208960985226531) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9895298215369284) | (false,1.0385823149003282) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100)` | **(true,1.2172697208010153)** | (false,0.9132903477015786) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Int64,2},100000)` | (false,0.8719331427222351) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0081447457001307) | (false,1.0148582025591586) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100000)` | (false,0.417532107403025) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100000)` | (false,1.0000039765066602) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,BitArray{2},100)` | (false,0.9985359644155118) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.8511740075755193) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0226192820173763) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100000)` | (false,1.0013055202736343) | **(true,1.2664726900684125)** | **(true,1.2499999583333403)** | **(true,1.399999840000064)** |
| `(:sumvector,Array{Float32,2},100000)` | **(true,3.6331116057290305)** | (false,0.5300351394156942) | **(true,1.428570326533446)** | **(true,1.999997000009)** |
| `(:sumrange,JLD.UnsupportedType,100)` | **(true,1.6168821076793134)** | (false,0.7179940835676292) | **(true,1.8222220395062134)** | **(true,1.7499962500187498)** |
| `(:sumvector,BitArray{2},100)` | **(true,1.126953646912717)** | **(true,1.3343424152156098)** | **(true,1.3749915626898395)** | **(true,1.6666533335999947)** |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9577433186568813) | **(true,1.0774936898097367)** | (false,1.0) | (false,1.0) |
| `(:sumelt,Array{Float32,2},100)` | (false,1.000002330271902) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9091044381967428) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100)` | (false,0.9837606904805527) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100000)` | **(true,1.1296756603009819)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100)` | (false,1.0028086457692593) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.851514614852426) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0155461122290752) | (false,0.924406819832234) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100000)` | **(true,2.6905048746017113)** | (false,0.5247783337092519) | **(true,1.2727266776872488)** | **(true,1.6666640000106667)** |
| `(:sumlogical,BitArray{2},100)` | **(true,1.1232385179512379)** | (false,1.0079329902575758) | **(true,1.0599996640018816)** | **(true,1.4999850004499864)** |
| `(:sumrange,Array{Int64,2},100000)` | **(true,3.294914886430265)** | (false,0.4049624998350186) | **(true,1.272727223140505)** | **(true,1.499999750000125)** |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9398915562662444) | (false,1.0084486419057277) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100000)` | **(true,17.223405672057428)** | (false,1.0) | (false,1.0) | (false,1.0) |

