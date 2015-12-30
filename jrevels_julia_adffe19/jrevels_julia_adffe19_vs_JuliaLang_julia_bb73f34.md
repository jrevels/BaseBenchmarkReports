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
| `(:sumvector,Array{Int64,2},100)` | (false,0.9955492213525619) | (false,1.0138205689940183) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0002348899849025) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100000)` | (false,1.0219423727874994) | (false,0.9733652449167378) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100)` | (false,1.0188005308625907) | (false,0.9818176199088663) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9976609975831529) | (false,0.9818016623474095) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100)` | (false,1.0250520138290469) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100)` | (false,1.0115302726044944) | (false,0.9884958534375357) | (false,1.0) | (false,1.0) |
| `(:sumeach,BitArray{2},100000)` | **(true,1.5607769174553523)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100)` | (false,0.9999864093914923) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0102370735391484) | (false,1.0154506385778506) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100)` | (false,0.21321756381309875) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100)` | (false,1.0188670739575325) | **(true,1.1167291961096253)** | (false,1.0) | (false,1.0) |
| `(:sumrange,JLD.UnsupportedType,100000)` | **(true,1.1677831258908564)** | **(true,1.2163571241803421)** | (false,0.9090909256198317) | (false,1.0) |
| `(:sumvector,BitArray{2},100000)` | **(true,1.0700125934232712)** | (false,0.9541823351259582) | (false,1.0) | (false,1.0) |
| `(:sumelt,Array{Float32,2},100000)` | (false,1.0000483738550476) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0173957377364382) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100)` | (false,1.0001146015481654) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9999715342020048) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100000)` | **(true,1.1037859308323834)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100000)` | **(true,1.3166071488474866)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100)` | (false,0.8007725465113537) | (false,0.7920478613224574) | (false,0.8750028124367202) | (false,1.0) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0067469302461978) | (false,0.9775168952629654) | (false,1.0) | (false,1.0) |
| `(:sumlogical,BitArray{2},100000)` | **(true,1.0682733331593377)** | (false,0.9876901601138641) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,JLD.UnsupportedType,100)` | (false,1.0059075206664594) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0122490977080185) | (false,1.000648870861771) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100)` | (false,0.9024726149183085) | (false,1.013689668220715) | (false,0.8000006588213592) | (false,1.0) |
| `(:sumvector,Array{Int64,2},100000)` | (false,0.9996895004511727) | (false,1.0083256437797061) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Float32,2},100)` | (false,1.0098788985864067) | (false,1.0210968057251255) | (false,1.0) | (false,1.0) |
| `(:sumelt,Array{Int64,2},100)` | (false,0.9998903373026468) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0130580670639817) | (false,1.019652384871903) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9488479015302561) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100000)` | (false,0.6670231708360032) | **(true,1.453552392638672)** | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100000)` | (false,0.9977498321387778) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0006800579842625) | (false,1.0025229449765594) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100000)` | (false,1.0132288476878646) | (false,0.9825942226434664) | (false,1.0) | (false,1.0) |
| `(:sumcolon,JLD.UnsupportedType,100)` | **(true,1.1310792989816283)** | (false,0.8767813993685946) | (false,0.5512821088099861) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100000)` | (false,1.0003148332775273) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100)` | (false,0.9997580034322943) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0065348656411417) | (false,0.988708339390223) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100000)` | **(true,1.0707382326917105)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.005750782059174) | (false,1.0040193949409202) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100000)` | (false,1.004653045335005) | (false,0.9790766867535878) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0000662817316275) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100000)` | (false,0.9999148312429056) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100000)` | (false,0.7772788237524992) | (false,0.8198419419167169) | (false,0.8750002812493672) | (false,1.0) |
| `(:sumlinear,Array{Int64,2},100)` | (false,0.9999518206574307) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100)` | (false,0.9890840717911825) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100)` | (false,1.0000445633679176) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | **(true,1.0659131432571234)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9999177157082065) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.021570200577408) | (false,0.9899135377574597) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100000)` | (false,1.0258506473880924) | (false,1.0075879771729095) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9999649696135264) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,Array{Int64,2},100000)` | **(true,1.7441436474051055)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Float32,2},100000)` | (false,0.9943478786913766) | (false,0.9712000102781606) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100)` | (false,1.0376719094757099) | (false,0.9799234496864813) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9955292151428317) | (false,0.9779365327841557) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0000332107598258) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0065051696822829) | (false,1.0142654615894329) | (false,1.0) | (false,1.0) |
| `(:sumvector,Array{Float32,2},100)` | (false,0.9944663804798642) | (false,0.999143331053141) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0267825145680045) | (false,0.9793647929633332) | (false,1.0) | (false,1.0) |
| `(:sumcolon,JLD.UnsupportedType,100000)` | (false,1.0481034947251417) | **(true,1.5924497152979118)** | (false,0.857142897959172) | (false,1.0) |
| `(:sumlinear,BitArray{2},100000)` | **(true,1.586724575575152)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100)` | (false,1.0000841534655696) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0020637246573734) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100)` | (false,1.0060201384427263) | (false,1.0348552646183748) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Int64,2},100)` | (false,1.0093681794999534) | **(true,1.088359213955022)** | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0135014025934397) | (false,1.001760711110313) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0264476495906918) | (false,0.9989192580144435) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100)` | (false,1.0217330978038528) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0002436959321013) | (false,1.0049256331587315) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100)` | (false,1.0084492967634449) | (false,1.0195098948701475) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Int64,2},100000)` | (false,1.0358715526055062) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0121569166883255) | (false,1.0178402284641401) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100000)` | (false,1.009205926467763) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100000)` | (false,1.0000318122462022) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,BitArray{2},100)` | (false,0.9998381184090067) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.010680356732686) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9987830777698425) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100000)` | (false,0.7454453723931584) | **(true,1.3360605529775336)** | (false,1.0) | (false,1.0) |
| `(:sumvector,Array{Float32,2},100000)` | (false,1.0050558840317632) | (false,0.9928975620841992) | (false,1.0) | (false,1.0) |
| `(:sumrange,JLD.UnsupportedType,100)` | **(true,1.121837453465971)** | (false,0.8724887656785338) | (false,0.5625000546874932) | (false,1.0) |
| `(:sumvector,BitArray{2},100)` | **(true,1.0715490781881505)** | (false,0.9393660543257442) | (false,1.0) | (false,1.0) |
| `(:sumelt,Array{Float32,2},100)` | (false,0.9999649182642033) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0157109617791729) | (false,0.9958781826754375) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9999737651686691) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100)` | (false,0.999936500132802) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100000)` | (false,1.0002253323424253) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100)` | **(true,1.127470628401065)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0105188972291788) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0089130910285484) | **(true,1.1168589197971348)** | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100000)` | **(true,1.1278584234134574)** | (false,0.958813818869575) | (false,1.0) | (false,1.0) |
| `(:sumlogical,BitArray{2},100)` | (false,0.9810930416753533) | (false,1.0477724898130694) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9965920354408643) | (false,0.9714259457608768) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Int64,2},100000)` | (false,0.9983039692187134) | (false,1.0117197650739054) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100000)` | **(true,2.368098865724573)** | (false,1.0) | (false,1.0) | (false,1.0) |

