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
| `(:sumvector,Array{Int64,2},100)` | (false,0.2922242870977623) | **(true,1.836990023182247)** | (false,0.727277190009618) | (false,0.5000074998875017) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0170004241561919) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100000)` | **(true,1.0592458543975136)** | (false,0.9365199658227061) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100)` | (false,0.3105626150284026) | **(true,2.980966614434501)** | **(true,1.0999998000004)** | **(true,1.3333311111259258)** |
| `(:sumcartesian,Array{Int64,2},100)` | **(true,1.1683868255303698)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0218765796909435) | (false,1.0365437623715006) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100)` | (false,0.7312881059200842) | **(true,1.2309693412852032)** | (false,0.9659091993798201) | (false,0.6000095997696056) |
| `(:sumeach,BitArray{2},100000)` | (false,1.0096707267860665) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Float32,2},100)` | (false,0.9999775608567811) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0497480671701334) | (false,0.9924719261775844) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100)` | (false,0.9415515179937418) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100)` | (false,0.9287715602662595) | **(true,1.07236971792243)** | (false,1.0) | (false,1.0) |
| `(:sumrange,JLD.UnsupportedType,100000)` | (false,0.30192999504700263) | **(true,3.067256923256947)** | (false,0.6666667111111052) | (false,0.571428693877516) |
| `(:sumvector,BitArray{2},100000)` | (false,0.6608297894763999) | **(true,1.0783956077518553)** | (false,0.7272731735529887) | (false,0.600000479999424) |
| `(:sumelt,Array{Float32,2},100000)` | **(true,1.2599858883114088)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.7855598358061505) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100)` | (false,0.9996044928338534) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0205307859121509) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100000)` | **(true,1.0980467827519511)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100000)` | (false,0.8716548928189656) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100)` | (false,0.29541754112831503) | **(true,1.6915707686021573)** | (false,0.6666716665916678) | (false,0.40000719991360106) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.1040554771192124)** | (false,0.9119144603072842) | (false,1.0) | (false,1.0) |
| `(:sumlogical,BitArray{2},100000)` | (false,0.7093886531465994) | **(true,1.1682339931729602)** | (false,0.8125002812495781) | (false,0.666667333332) |
| `(:sumcartesian,JLD.UnsupportedType,100)` | **(true,1.0597701281955816)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | **(true,1.2317428079675823)** | (false,0.8449521943425068) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100)` | (false,0.633008406845402) | **(true,1.2999139009376481)** | (false,0.775281605855622) | (false,0.6666733332000027) |
| `(:sumvector,Array{Int64,2},100000)` | (false,0.280883340843886) | **(true,2.219592709924917)** | (false,0.7272731735529887) | (false,0.500000749998875) |
| `(:sumrange,Array{Float32,2},100)` | (false,0.6724408418942451) | **(true,1.3916674676258936)** | (false,0.9677419424210877) | (false,0.666667777774074) |
| `(:sumelt,Array{Int64,2},100)` | (false,1.0001214174086264) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.015270928335197) | (false,0.9995997818728665) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | **(true,1.1212458770155218)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,BitArray{2},100000)` | **(true,1.3864871545913118)** | (false,0.7661250129942198) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Int64,2},100000)` | (false,0.9060370450291512) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.009954173236088) | (false,1.0197371248530727) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Int64,2},100000)` | (false,0.27245749067852004) | **(true,2.537124049527661)** | (false,0.7857146530605947) | (false,0.600000959997696) |
| `(:sumcolon,JLD.UnsupportedType,100)` | (false,0.7005519896744741) | **(true,1.4278718357393105)** | (false,0.9936305740597995) | (false,0.6666688888740742) |
| `(:sumlinear,Array{Float32,2},100000)` | (false,1.0002712341539504) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100)` | (false,1.0002324376392142) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.033934523524771) | (false,0.9655896226840694) | (false,1.0) | (false,1.0) |
| `(:sumeach,JLD.UnsupportedType,100000)` | (false,0.46258366138503826) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9832509992027736) | (false,1.0064128409487099) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Int64,2},100000)` | **(true,1.0991083137333855)** | (false,0.9079125485881323) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0247955304175589) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,BitArray{2},100000)` | (false,0.983378708763181) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,JLD.UnsupportedType,100000)` | (false,0.27629373844165805) | **(true,2.1893523732640965)** | (false,0.6666671666659166) | (false,0.400000719999136) |
| `(:sumlinear,Array{Int64,2},100)` | (false,1.0068168843419019) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100)` | (false,0.6540855893588116) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100)` | (false,1.0000022826812496) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,JLD.UnsupportedType,100000)` | **(true,1.258465575220644)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0044205307671095) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9977046275361421) | (false,0.9250115302576086) | (false,1.0) | (false,1.0) |
| `(:sumlogical,JLD.UnsupportedType,100000)` | (false,0.4141163031184555) | **(true,2.067504226952738)** | (false,0.8571431020403965) | (false,0.800000479998848) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.999648431093448) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Float32,2},100000)` | (false,0.3521912759470992) | **(true,2.307302087213051)** | (false,0.7692308047337223) | (false,0.6666667777777407) |
| `(:sumelt,Array{Int64,2},100000)` | (false,0.9994515612623458) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100)` | (false,0.2669122037072444) | **(true,2.964710804296247)** | (false,0.8823530795846123) | (false,0.8571432653049563) |
| `(:sumrange,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0288500891131336) | (false,1.039355329968913) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9881803960908567) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.0751488104673776)** | (false,0.9593907800128787) | (false,1.0) | (false,1.0) |
| `(:sumvector,Array{Float32,2},100)` | (false,0.2924450095906902) | **(true,1.5383470672375545)** | (false,0.7000053999028018) | (false,0.5000074998875017) |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0330380265228183) | (false,0.9318320139404651) | (false,1.0) | (false,1.0) |
| `(:sumcolon,JLD.UnsupportedType,100000)` | (false,0.9541602254730026) | (false,0.8522507791924345) | (false,0.8750000312499921) | (false,0.6666668888887407) |
| `(:sumcartesian,Array{Float32,2},100)` | (false,0.9969862160841934) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,BitArray{2},100000)` | (false,1.003292437000146) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0036516496846264) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100)` | (false,0.7324913988063066) | **(true,1.244750957925408)** | (false,0.9577466455061867) | (false,0.6000095997696056) |
| `(:sumrange,Array{Int64,2},100)` | (false,0.6568843486349478) | **(true,1.4485655864410247)** | (false,0.9815950942828106) | (false,0.666667777774074) |
| `(:sumcolon,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9949744750772276) | (false,0.9729111605578259) | (false,1.0) | (false,1.0) |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9579122328539323) | (false,1.0013887361621205) | (false,1.0) | (false,1.0) |
| `(:sumlinear,JLD.UnsupportedType,100)` | (false,0.014167105821285109) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumlinear,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.0318212053412739) | (false,0.9776811258506091) | (false,1.0) | (false,1.0) |
| `(:sumcolon,Array{Float32,2},100)` | (false,0.852601167357085) | **(true,1.1759205660329677)** | (false,1.0) | (false,1.0) |
| `(:sumlinear,Array{Int64,2},100000)` | **(true,1.1079850094538235)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcolon,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,1.011267183979889) | (false,0.9974029612675634) | (false,1.0) | (false,1.0) |
| `(:sumelt,JLD.UnsupportedType,100000)` | **(true,1.0571094287991334)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Float32,2},100000)` | (false,0.9997974316477544) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,BitArray{2},100)` | (false,1.0003355644333585) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.1749788318933643)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,0.9778498164047265) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,BitArray{2},100000)` | (false,0.6915735757486121) | **(true,1.1736941536281622)** | (false,0.8000000266666631) | (false,0.7142857959183441) |
| `(:sumvector,Array{Float32,2},100000)` | (false,0.26900866555293074) | **(true,1.9807601868078641)** | (false,0.700000539999028) | (false,0.500000749998875) |
| `(:sumrange,JLD.UnsupportedType,100)` | (false,0.6001648969983848) | **(true,1.3800731217540143)** | (false,0.5487805428316411) | (false,0.5714297959148689) |
| `(:sumvector,BitArray{2},100)` | (false,0.6432081219736625) | (false,0.9872659121586932) | (false,0.727277190009618) | (false,0.6000047999424007) |
| `(:sumelt,Array{Float32,2},100)` | (false,0.9999530986732125) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumvector,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | (false,1.0399911410298344) | (false,0.9593917492293901) | (false,1.0) | (false,1.0) |
| `(:sumelt,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.995751090558006) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumeach,Array{Int64,2},100)` | (false,0.9996177396247089) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,Array{Float32,2},100000)` | (false,0.9040374258177665) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,BitArray{2},100)` | (false,0.9909820823614524) | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumcartesian,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.1734103541625893)** | (false,1.0) | (false,1.0) | (false,1.0) |
| `(:sumrange,SubArray{Int64,2,Array{Int64,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100)` | (false,0.9849109176027763) | (false,1.0107583236221638) | (false,1.0) | (false,1.0) |
| `(:sumlogical,Array{Float32,2},100000)` | (false,0.4084832886697032) | **(true,1.8627873230685223)** | (false,0.7857146530605947) | (false,0.600000959997696) |
| `(:sumlogical,BitArray{2},100)` | (false,0.7950595598221124) | **(true,1.151412334442444)** | (false,0.9433965254523183) | (false,0.6666733332000027) |
| `(:sumlogical,SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},1},100000)` | **(true,1.0589523605674875)** | (false,0.9731180610715597) | (false,1.0) | (false,1.0) |
| `(:sumrange,Array{Int64,2},100000)` | (false,0.2965202771588973) | **(true,2.5060047898601807)** | (false,0.7857143163265262) | (false,0.6666667777777407) |
| `(:sumlinear,JLD.UnsupportedType,100000)` | (false,1.016676744588198) | (false,1.0) | (false,1.0) | (false,1.0) |

