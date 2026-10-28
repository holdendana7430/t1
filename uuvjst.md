代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtiscjdlwj.html

TS:   [...a, ...b];
来源：http://hz.shangyingyoupin.top/gtvmvkpugt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtimimrlig.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtgkhuhyjv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.mhx1999.top/gtwutrkrli.html

C#:   a.Concat(b).ToList()
来源：http://hz.52xcode.cn/gtyojrxbze.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtkzuofwmz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtkmtpkbiw.html

PHP:  sort($arr);
来源：http://hz.yj202588.top/gtnldfrdui.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtiyjknvyg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenlongwang.top/gtxwyjosed.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtwwdshlel.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtenvitezt.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtdqiovqkz.html

C#:   list.Sort();
来源：http://hz.chenzaomai.com/gtiiusgmns.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhaomingkeji.xyz/gtzuedgees.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhoulong.xyz/gtvrwozeow.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gthceayrhv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtpsdychna.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hfpthk.cn/gtgdhzlgzc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fzhhl.top/gtmxbsqfdp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.birdmap.top/gtijwnhcsx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtycsvasiv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jianghu66.top/gtjffenwpu.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtrdguphie.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtstxhbnhb.html

PHP:  array_reverse($arr);
来源：http://hz.zhiwuduotai.top/gtbdiinhce.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtykfbslcn.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtdxtttbdr.html

Java: Collections.reverse(list);
来源：http://hz.hysaishi.cn/gtvmhuxhbw.html

Go:   slices.Reverse(arr)
来源：http://hz.redwolf501.top/gtjrorgcjh.html

Ruby: arr.reverse
来源：http://hz.mhx1999.top/gtgzkwvbfi.html

C#:   list.Reverse();
来源：http://hz.hongshengwenyu.top/gtqorfaghp.html

[D12] 查找元素下标
来源：http://hz.yanxiufei.cn/gtgsqmcwnq.html

Py:   arr.index(x);  x in arr
来源：http://hz.xziqi.cn/gtydpjeylh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nwbrower.top/gtylqsxdyy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtzifxfhst.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.svipenyu.cn/gtfeiepfqq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.wangdashe.top/gtsmervqxu.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtnhtovkrm.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtssahejll.html

C#:   list.IndexOf(x);
来源：http://hz.jqgufenzy.top/gtoripjjin.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnqzz.top/gticefdckn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhaomingkeji.xyz/gtgcdfkhnz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenlongwang.top/gtqabcngxj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtoywoptug.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtypaosphe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.svipenyu.cn/gtwlejqiwk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinyuanbaomall.cn/gtojbtkpjo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.iojbl.cn/gtzpkomclj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shangyingyoupin.top/gtmegjczww.html

[D14] 映射转换（每个元素变形）
来源：http://hz.kuanghao11.cn/gtvjsvvjuv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuanzhike.top/gtbjmxbscm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.daria6918.cn/gtrwkamclv.html

JS:   arr.map(x => x * 2)
来源：http://hz.hongshengwenyu.top/gtenxcpfxm.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtexninxor.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.mhx1999.top/gtpycompcb.html

Go:   // 手写循环
来源：http://hz.fzhhl.top/gtasdhswdn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtfzdtczbr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.52xcode.cn/gtnlzpfpaj.html

[D15] 去重
来源：http://hz.zhaomingkeji.xyz/gtbpokuuvu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtrtjtkhav.html

PHP:  array_unique($arr);
来源：http://hz.xuanzx.com/gtlsnadtoy.html

JS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtzooejsrx.html

TS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gttriayaez.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenlongwang.top/gtsebbewps.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gzhubu.top/gtffokhvjj.html

Ruby: arr.uniq
来源：http://hz.zhiwuduotai.top/gtfqdaiqix.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtkkqzttfh.html

[D16] 求和与平均值
来源：http://hz.wangshuangyany.cn/gtjmtdcegf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.wangdashe.top/gtlsbnzvnc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ivvv.top/gtlyxugtke.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cdnleiting.top/gtimhrfrrb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtettyznmm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtzniqvvdx.html

Go:   // 手写循环累加
来源：http://hz.chenlongwang.top/gtydoecgsb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.cdnleiting.top/gtfpusfkhk.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtchhpygko.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gttmudocfd.html

Py:   max(arr);  min(arr)
来源：http://hz.yuxming.cn/gtpxbzmagm.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtqvvqnxgq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhijiandao.cn/gtzoloceei.html

TS:   Math.max(...arr);
来源：http://hz.cheryme.top/gtkekjhstz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yueranfly.top/gttozisuqc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hnqzz.top/gtmiftwoeg.html

Ruby: arr.max;  arr.min
来源：http://hz.fzhhl.top/gtmwddbtcw.html

C#:   list.Max();  list.Min()
来源：http://hz.ivvv.top/gtvftzgqnh.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtylwhtnpq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ydjk.org.cn/gtjzmgbkof.html

PHP:  array_merge(...$nested);
来源：http://hz.daxiang520.top/gtkzbiqvtm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhongyouzk.top/gtmgfetvtl.html

TS:   nested.flat();
来源：http://hz.yj202588.top/gtynyvzlyc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shuidangran.top/gtbvxkzeaz.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtlukyzhhh.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtjlelycml.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.vqdsnc.cn/gtjdxairoj.html

[D19] 按字段分组
来源：http://hz.dianchejie.cn/gtmzenedij.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.havefunace.top/gtfhecutkf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zycfv.cn/gthsjwdhsz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guowangkeji.top/gtuhbzxjgi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtytrgfpmj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhengqikj.top/gtlitcisio.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtfmrjomnw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xuetiantiany.cn/gtxhnhmjwp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gthdukebnd.html

[D20] 统计每个元素出现次数
来源：http://hz.zhijiandao.cn/gtgbdslveq.html

Py:   Counter(arr)
来源：http://hz.quarkkingdee.top/gtldtshixq.html

PHP:  array_count_values($arr);
来源：http://hz.chenlongwang.top/gtxkehssmf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhongyouzk.top/gtgispmuzi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtmsrokzyb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jianghu66.top/gtijwfjyll.html

Go:   // 手写 map[T]int
来源：http://hz.guowangkeji.top/gtxoaqlvfi.html

Ruby: arr.tally
来源：http://hz.sysykeji.top/gtevheonru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.guannengcc.top/gttpcjhhld.html

[D21] 判断是否包含某元素
来源：http://hz.hnxiangtu.top/gtzbwdxsae.html

Py:   x in arr
来源：http://hz.yvedp.cn/gtxnworagk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenlongwang.top/gtvqcqjodb.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtdwbitagg.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtjsakgjuj.html

Java: list.contains(x)
来源：http://hz.sweek.top/gtdaoywlhh.html

Go:   slices.Contains(arr, x)
来源：http://hz.xinyue.icu/gtoftmsvlc.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtjmhtrgmo.html

C#:   list.Contains(x)
来源：http://hz.jianghu66.top/gtxrgwsvym.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtvsntdppa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xziqi.cn/gtmxornijy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhiwuduotai.top/gttuvfnxfi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtvlwbhbsi.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtrweqosri.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtutgnsfrb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hywenlv.cn/gtadifkzgi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yvedp.cn/gtzcbxksci.html

C#:   new List<int>(list);
来源：http://hz.quarkkingdee.top/gtlifdwhyl.html

[D23] reduce 累积计算
来源：http://hz.hongshengwenyu.top/gtafuvqodq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yanxiufei.cn/gthxnmscpt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yuanzhike.top/gtewuudkqi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gthxigdmcv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.kuanghao11.cn/gtzthzcsdk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yongpay.top/gtrazqswld.html

Go:   // 手写循环
来源：http://hz.52xcode.cn/gtppvvxzen.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.svipenyu.cn/gtisunnail.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hysaishi.cn/gtbiicthij.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gttytrxxpg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hongshengwenyu.top/gtytnbehmz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.aibaodan.cn/gtrjaxbuci.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtrdlrrlyq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.zhiwuduotai.top/gtlrpmulxd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuanzhike.top/gtiheyseod.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.9152youxi.cn/gtfsltlmec.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.9152youxi.cn/gtwrplabps.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.kuanghao11.cn/gtwngstmkd.html

[D25] Set 集合去重与交并差
来源：http://hz.birdmap.top/gtkwzfccqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinghuilouyu.cn/gttwotfmrn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xziqi.cn/gtsrrzqsyo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aizwys.cn/gtfclhnudf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xinyue.icu/gtpfuorxhh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yuanzhike.top/gtsxdkbkli.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gtcynqmism.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jinghuilouyu.cn/gtdptgmwgw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnxiangtu.top/gtovsrxbpn.html

[D26] 数组转字符串
来源：http://hz.sufxvd.cn/gtpbyxnhdq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yanxiufei.cn/gtfsgdyfai.html

PHP:  implode(", ", $arr);
来源：http://hz.kuanghao11.cn/gtgsxuxtcu.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtfknmdbrk.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gtgrxcxoqi.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtyaagvtxp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yueranfly.top/gtgcndabtw.html

Ruby: arr.join(", ")
来源：http://hz.yvedp.cn/gtlvghoroc.html

C#:   string.Join(", ", list)
来源：http://hz.fzhhl.top/gtfavtpzbk.html

================================================================================
来源：http://hz.yuxming.cn/gteeulevvi.html

E. 字符串处理
来源：http://hz.svipenyu.cn/gthnplfxbh.html

================================================================================
来源：http://hz.quarkkingdee.top/gtnxvjypuq.html

[E01] 拼接字符串
来源：http://hz.hysaishi.cn/gtmhvjbapd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gtacwcczqe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtrlfgqdlk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtbxmtdgeh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yj202588.top/gtituqjkja.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shuidangran.top/gtgxlxzcdu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhixingplan.top/gthaajjpuq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tian-w.cn/gtnucoiodj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtzuwugszz.html

[E02] 重复字符串
来源：http://hz.tianlin.xyz/gtiiegitcn.html

Py:   "ab" * 3
来源：http://hz.dashuyun.cn/gtmdafuwnm.html

PHP:  str_repeat("ab", 3);
来源：http://hz.bjfxy.top/gthfzecaum.html

JS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gtlievhtpz.html

TS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gtxlcaytxi.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtwdgcxnvz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.ydjk.org.cn/gtthalkwgn.html

Ruby: "ab" * 3
来源：http://hz.jqgfzy.top/gtqoruxwqy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shanyushiyangtech.top/gtyapbdebl.html

[E03] 截取子串
来源：http://hz.shangyingyoupin.top/gtkqoevemn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gtebqmexxv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.guowangkeji.top/gttybvzpza.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtdetrmqgg.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gthuxcabht.html

Java: s.substring(1, 4)
来源：http://hz.havefunace.top/gtnplfoago.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yangfankeji.com/gtyvvykemp.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yvedp.cn/gttyxcvkfu.html

C#:   s.Substring(1, 3)
来源：http://hz.9152youxi.cn/gtcovbklle.html

[E04] 查找子串位置
来源：http://hz.jqgfzy.top/gteripvmyk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.mhx1999.top/gtmqijpfae.html

PHP:  strpos($s, "x");
来源：http://hz.yanxiufei.cn/gtliyahply.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ehwqpu.com/gtkfysomsg.html

TS:   s.indexOf("x")
来源：http://hz.zhijiandao.cn/gtwvxfrzgz.html

Java: s.indexOf("x")
来源：http://hz.cheryme.top/gtfupyjruj.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gtiwhsvldb.html

Ruby: s.index("x")
来源：http://hz.shzxlz.cn/gtwcjiwphw.html

C#:   s.IndexOf("x")
来源：http://hz.birdmap.top/gtcpoocebc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.bjfxy.top/gtubdrrnxp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yueranfly.top/gtannpaqmb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.daxiang520.top/gtaqbrtuic.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtkmhkxqdc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hywenlv.cn/gtdtlawxpn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtlipouhez.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.hongshengwenyu.top/gtjqojxrtt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hywenlv.cn/gtuowpijkx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgfzy.top/gtnngwmlvc.html

[E06] 替换子串
来源：http://hz.jqgfzy.top/gtenjidtih.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtpazgeuby.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhixingplan.top/gtdfrlcwos.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhiwuduotai.top/gtjoktaqlx.html

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtydtabeeg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangshuangyany.cn/gtdhvparwv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinqigfzy.top/gtwclumams.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gtuoqxcgff.html

C#:   s.Replace("a", "b")
来源：http://hz.svipenyu.cn/gtokpqkopm.html

[E07] 按分隔符拆分
来源：http://hz.feifeiyinyue.top/gtiebdxejg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.jiagoushi.top/gtvablcmyc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.xuanzx.com/gtzdhogefz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shanyushiyangtech.top/gtwylehsqx.html

TS:   s.split(",")
来源：http://hz.daxiang520.top/gtyanmnhuf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhaomingkeji.xyz/gtvqdaduly.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenjidiqi.icu/gtwmvpbgey.html

Ruby: s.split(",");  s.split
来源：http://hz.chenlongwang.top/gthzscamxj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ppjwa.cn/gtvwaaqdhb.html

[E08] 数组按分隔符合并
来源：http://hz.zhaomingkeji.xyz/gtapkwjtll.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtawblhlxs.html

PHP:  implode(",", $items);
来源：http://hz.iojbl.cn/gtefdehitf.html

JS:   items.join(",")
来源：http://hz.cashguo.top/gtkjwqetxl.html

TS:   items.join(",")
来源：http://hz.mhx1999.top/gtriyoeqdl.html

Java: String.join(",", items)
来源：http://hz.zhaomingkeji.xyz/gtrqggmfhv.html

Go:   strings.Join(items, ",")
来源：http://hz.yangfankeji.com/gthhdkaemv.html

Ruby: items.join(",")
来源：http://hz.kuanghao11.cn/gtlfdsjrjk.html

C#:   string.Join(",", items)
来源：http://hz.cqqwz.cn/gtvwnjdryn.html

[E09] 去除所有空白字符
来源：http://hz.tianlin.xyz/gtcfwgsvlo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shzxlz.cn/gtlvqnhsfj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.gzhubu.top/gtkhgvtyxw.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gzhubu.top/gtjgmxywav.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.316326.xyz/gtnkhundoh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.snrcjt.cn/gtrxpptulv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fzhhl.top/gtpynedouc.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ivvv.top/gtjxuepilc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.birdmap.top/gtsgessjde.html

[E10] 左侧补零 / 定长填充
来源：http://hz.fengsongda.top/gtsfztskqs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hfpthk.cn/gtejwxiqgu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.aibaodan.cn/gtsxmawbyu.html

JS:   "7".padStart(3, "0")
来源：http://hz.nanxinkj.top/gtdiootrdr.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenjidiqi.icu/gtksghprkt.html

Java: String.format("%03d", 7)
来源：http://hz.kuanghao11.cn/gteioffjyd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.andypj.xyz/gthokkcrpw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtzlyfvzhx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.tianlin.xyz/gttqvkrqrz.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtmlowjlpc.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtenixulcn.html

PHP:  strrev($s);
来源：http://hz.zycfv.cn/gtotqjbfvf.html

JS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtysivaivt.html

TS:   [...s].reverse().join("")
来源：http://hz.tanke756.top/gtckvzqedw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.pycfn.com/gtqcwbkozs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hammf.cn/gtkurvhvel.html

Ruby: s.reverse
来源：http://hz.pengpengdd.cyou/gtlvcmzvsc.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhoulong.xyz/gtjcuiducr.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtgsqeebmi.html

Py:   s.count("a")
来源：http://hz.hfpthk.cn/gtorjzcfou.html

PHP:  substr_count($s, "a");
来源：http://hz.birdmap.top/gtoyonclfy.html

JS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtqsygvgnz.html

TS:   s.split("a").length - 1
来源：http://hz.ybcxt.top/gtgxcultkb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sweek.top/gthjyomija.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtddgchdvm.html

Ruby: s.count("a")
来源：http://hz.yanxiufei.cn/gtphiebacs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtkymbccwk.html

[E13] 逐字符遍历
来源：http://hz.havefunace.top/gtyvmttyyu.html

Py:   for ch in s: print(ch)
来源：http://hz.shanyushiyangkeji.top/gtvohhxibn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtkbcaxrjo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ybcxt.top/gtrycarrtp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hammf.cn/gtdabmgsbe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtzthsemea.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigufen.top/gthmokfhah.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sweek.top/gtxygosmht.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.sxryk.cn/gtvqidxjkk.html

[E14] URL 编码与 Base64
来源：http://hz.dashuyun.cn/gtyecgcpxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jlsjyb.cn/gtytnfbdnz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yuanzhike.top/gtnmiquxyz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cheryme.top/gtnqbhmkru.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtxqlocxtx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.xziqi.cn/gtvdmrofbt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuetiantiany.cn/gtyhukfchw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj20258888.top/gtgvjyggrz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.316326.xyz/gtkxflcyij.html

[E15] HTML 转义 / 反转义
来源：http://hz.dianchejie.cn/gtnhwjzltf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.shanyushiyangtech.top/gtjyeefdcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtftjqmani.html


<!-- 参考信息 -->