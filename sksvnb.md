代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.cdnleiting.top/gtjzdfqluw.html

Java: list.subList(1, 4);
来源：http://hz.0kj1m.cn/gtauoihqtz.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gthxlxdfsy.html

Ruby: arr[1, 3]
来源：http://hz.zhixingplan.top/gtjbpnqocd.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtfvnpkyif.html

[D08] 合并两个数组
来源：http://hz.mhx1999.top/gtymdfphwc.html

Py:   a + b;  a.extend(b)
来源：http://hz.kuanghao11.cn/gtfrgxabgn.html

PHP:  array_merge($a, $b);
来源：http://hz.gotoacloud.top/gtpjlxnvti.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nanxuanxn.top/gtmryjiicf.html

TS:   [...a, ...b];
来源：http://hz.jyoumei.cn/gtdogtdtsg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.0kj1m.cn/gtazfrduvb.html

Go:   append(a, b...)
来源：http://hz.cashguo.top/gtgqilsezy.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cdnleiting.top/gtjytfldvt.html

C#:   a.Concat(b).ToList()
来源：http://hz.snrcjt.cn/gtvqnfcyct.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtlggsmysy.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gttzbanyis.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtscmgrlaj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.svipenyu.cn/gtznysxijz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ybcxt.top/gtfplspdom.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtzbtoievo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtfnscjunr.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtnjbtdswu.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtuiwkjvuj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xinyue.icu/gtmqofsrbj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtrvekcbpu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhiwuduotai.top/gtxitgzgzq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtlpbnycbv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtnhdhuhno.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtzdhiiquc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xylfe.cn/gtuvqoxbyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.c1oappe.top/gtcooepwhe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtkbdrprju.html

[D11] 反转数组
来源：http://hz.yj20258.top/gtmzzmymeh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tanke756.top/gteqjktcgd.html

PHP:  array_reverse($arr);
来源：http://hz.snrcjt.cn/gtmwhrmsfs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hysaishi.cn/gthozyyqje.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtkixhfmzg.html

Java: Collections.reverse(list);
来源：http://hz.chenzaomai.com/gtjgsbqwlr.html

Go:   slices.Reverse(arr)
来源：http://hz.zycfv.cn/gtozwwcwxy.html

Ruby: arr.reverse
来源：http://hz.shanyushiyangtech.top/gtviespwrg.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gteathclpb.html

[D12] 查找元素下标
来源：http://hz.aibaodan.cn/gtiojkunoy.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gtlgopjrad.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tian-w.cn/gtwwubgefz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtkpfccyfw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhaomingkeji.xyz/gtgwdmoghf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.iojbl.cn/gtybvwpmhl.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtrzvvmdkh.html

Ruby: arr.index(x)
来源：http://hz.wangdashe.top/gtqdauuvcl.html

C#:   list.IndexOf(x);
来源：http://hz.shuidangran.top/gtysgohpgv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.aibaodan.cn/gtwcpqnirr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.guannengcc.top/gtggrjymbq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.c1oappe.top/gtsnrdyqen.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtxqftefrh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cqqwz.cn/gtsdalhgyg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtmltjqofb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ivvv.top/gtqxotgxpi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yvedp.cn/gtkctqmayp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.9152youxi.cn/gthgiuoiqs.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xziqi.cn/gtdfnrdzlq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xinyue.icu/gtbkdhflme.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ppjwa.cn/gtlyrizfua.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtkdvrvgqj.html

TS:   arr.map(x => x * 2)
来源：http://hz.nanxuanxn.top/gtoginbcum.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgufenzy.top/gtcztycksg.html

Go:   // 手写循环
来源：http://hz.gzhubu.top/gtdyqlppct.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hfpthk.cn/gttjjbntyo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtjodoqgsn.html

[D15] 去重
来源：http://hz.tanke756.top/gtvhikiyii.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtdyzdvxeb.html

PHP:  array_unique($arr);
来源：http://hz.vqdsnc.cn/gtgkqwkqcj.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtzwlbloga.html

TS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gtvuyjoufi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yvedp.cn/gtnnlmhxnn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtoekjlewp.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtfabspisu.html

C#:   list.Distinct().ToList()
来源：http://hz.zhongyouzk.top/gtkxfcxbiy.html

[D16] 求和与平均值
来源：http://hz.pengpengdd.cyou/gtnsmjigjp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jyoumei.cn/gtysmegczx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.shangyingyoupin.top/gtedwibprs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gthimwnrfn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtwhzsusvd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gttaycwfix.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gttbjtuuqo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daria6918.cn/gtxbvhqjsm.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnqzz.top/gtdcatjrhv.html

[D17] 最大值与最小值
来源：http://hz.pycfn.com/gthbknknkr.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gtsjaalerj.html

PHP:  max($arr);  min($arr);
来源：http://hz.meibo888.top/gtghrtazpe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ywan-chungtsiang.top/gtwecjljfc.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gteaftgrat.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gtgponlicg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.andypj.xyz/gtcosmsxau.html

Ruby: arr.max;  arr.min
来源：http://hz.zhijiandao.cn/gtobsreypv.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtrronjhqw.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gthhxqqkxl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtznqyveud.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtqvptzfrv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtibxuprkr.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtjacuuoxn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.fengsongda.top/gthxvozudo.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtjkkpkvjs.html

Ruby: nested.flatten
来源：http://hz.shuidangran.top/gtqwydvlip.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.quarkkingdee.top/gtzbxgnlum.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtnwomeinb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jianghu66.top/gtlyajepwo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gteabhbawj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ydjk.org.cn/gtkbefbkns.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hysaishi.cn/gttqxxkptv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuanzx.com/gtyptkjmny.html

Go:   // 手写 map[string][]T
来源：http://hz.mhx1999.top/gtresffliy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jlsjyb.cn/gtkazvtvdx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sxryk.cn/gtabzvkgyq.html

[D20] 统计每个元素出现次数
来源：http://hz.feifeiyinyue.top/gtvsuuwcml.html

Py:   Counter(arr)
来源：http://hz.vqdsnc.cn/gtsffwljhp.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtgabongya.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuanzx.com/gtvxdznhjg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtnbggxprx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydjk.org.cn/gtdaslrgks.html

Go:   // 手写 map[T]int
来源：http://hz.gotoacloud.top/gtujubdlty.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtacslaute.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtixbgokgs.html

[D21] 判断是否包含某元素
来源：http://hz.guowangkeji.top/gtqptxycfd.html

Py:   x in arr
来源：http://hz.gaohongyu789.top/gthzjsxidx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenzaomai.com/gtyzfjtwhs.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtynkstnmv.html

TS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtxydibyvw.html

Java: list.contains(x)
来源：http://hz.cheryme.top/gtkpyrkeww.html

Go:   slices.Contains(arr, x)
来源：http://hz.xylfe.cn/gtykdnuleb.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gtstmjwmfo.html

C#:   list.Contains(x)
来源：http://hz.hammf.cn/gthmqvyolh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtfcfhivlh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cashguo.top/gtjubdejpq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gzhubu.top/gtyhskgxca.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.havefunace.top/gtlhbksufy.html

TS:   [...arr];
来源：http://hz.jinghuilouyu.cn/gtcrebceid.html

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gtmtyjphrt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.nwbrower.top/gtfmyiyezt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yuxming.cn/gtnposkstj.html

C#:   new List<int>(list);
来源：http://hz.zhoulong.xyz/gtaumhxqye.html

[D23] reduce 累积计算
来源：http://hz.ywan-chungtsiang.top/gtoungkeqy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtxpkgnuom.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.svipenyu.cn/gtjnyzubjb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtebrmsauk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.haohaochexian.top/gtknvnynvu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tanke756.top/gtcormvkyg.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtgcopdlgf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jinqigfzy.top/gtpjvijiwl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gtalilehwf.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtfddfqzcy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.feifeiyinyue.top/gtmakwqona.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.mhx1999.top/gtannhrmto.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.iojbl.cn/gtamyxsdtz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtfclaesob.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.dianchejie.cn/gtbnrresmq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.aibaodan.cn/gtznzjxrde.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ehwqpu.com/gtgfttoplr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.c1oappe.top/gthguvogle.html

[D25] Set 集合去重与交并差
来源：http://hz.yuxming.cn/gtboyegizl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gtnmfxdpzs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.kuanghao11.cn/gtdwnjsccs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gtuxeemsow.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.hysaishi.cn/gtpvegjhyc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gttvryvltn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gogol.net.cn/gtsqmmqaay.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.c1oappe.top/gtgxylhqsv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.nwbrower.top/gtapduntho.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtszjtlpzy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pengpengdd.cyou/gtxxiyzuxk.html

PHP:  implode(", ", $arr);
来源：http://hz.redwolf501.top/gtgygadnlk.html

JS:   arr.join(", ")
来源：http://hz.zhongyouzk.top/gtquaxvibv.html

TS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtgyftlkgo.html

Java: String.join(", ", list)
来源：http://hz.hnqzz.top/gtdnxjpmlk.html

Go:   strings.Join(strs, ", ")
来源：http://hz.andypj.xyz/gtiurwgifs.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gtmwsajthn.html

C#:   string.Join(", ", list)
来源：http://hz.fengsongda.top/gtdchejvab.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgigdmsuz.html

E. 字符串处理
来源：http://hz.ybcxt.top/gtpqfgiyfx.html

================================================================================
来源：http://hz.yj20258.top/gtvilbfnfe.html

[E01] 拼接字符串
来源：http://hz.daria6918.cn/gtzosbrvcg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtgwawtzby.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhixingplan.top/gtyxmyvrro.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtypgugebe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ehwqpu.com/gtkzzsjfzb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yonumen.top/gtnaoallrm.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj202588.top/gtpjqqtpfh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.daxiang520.top/gtmelhoysk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258.top/gtcuoiuixa.html

[E02] 重复字符串
来源：http://hz.meibo888.top/gtyxpjyizj.html

Py:   "ab" * 3
来源：http://hz.dianchejie.cn/gtmkqgyxbq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yongpay.top/gtgrbszmbb.html

JS:   "ab".repeat(3)
来源：http://hz.nwbrower.top/gtsczdxbov.html

TS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtwttujwzu.html

Java: "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtabzykljp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhongyouzk.top/gtblmcfgwl.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtenbelcei.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yanxiufei.cn/gtidckohnu.html

[E03] 截取子串
来源：http://hz.tanke756.top/gthrgvufyn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.mhx1999.top/gtwkhaulnj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.9152youxi.cn/gtdjsdglag.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.ivvv.top/gtxsqvdkvc.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtmtaolboa.html

Java: s.substring(1, 4)
来源：http://hz.ehwqpu.com/gthrzhxwyh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ybcxt.top/gtfqvaflnq.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.aizwys.cn/gtrhifoyan.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtgugtqqlq.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtkgtmsiyp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.tian-w.cn/gtyxdbfizz.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtpblgwzhb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fzhhl.top/gtqqjumacq.html

TS:   s.indexOf("x")
来源：http://hz.shangyingyoupin.top/gtspntvbnf.html

Java: s.indexOf("x")
来源：http://hz.yuanzhike.top/gtbwimaxcc.html

Go:   strings.Index(s, "x")
来源：http://hz.cqqwz.cn/gtygoqkawy.html

Ruby: s.index("x")
来源：http://hz.yonumen.top/gtaxmfvvxn.html

C#:   s.IndexOf("x")
来源：http://hz.xziqi.cn/gthohelcqr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtriikvquj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.jqgufenzy.top/gtkujfnsvx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtxikalvfe.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.daxiang520.top/gtojtcxcbd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtfhfrojdl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zdqjudy.top/gtgwrpybnn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ydjk.org.cn/gtbrnqluqp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hfpthk.cn/gtaosnbeng.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jinqigufen.top/gtkhmjjkha.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtguqfcfyb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtkreyadbm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtrnzqxjmg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.wangdashe.top/gtjwixtvjp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtghvisrbg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj202588.top/gthtpeztsn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.sysykeji.top/gtsshmngzi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.snrcjt.cn/gtyhltortk.html

C#:   s.Replace("a", "b")
来源：http://hz.yueranfly.top/gtzaqtgvdc.html

[E07] 按分隔符拆分
来源：http://hz.kuanghao11.cn/gtlzstsmia.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yj20258888.top/gtvvbcvsrs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yanxiufei.cn/gthykpchvc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.snrcjt.cn/gtpyuaumur.html

TS:   s.split(",")
来源：http://hz.wangshuangyany.cn/gthoerqwrc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.daxiang520.top/gtdsxdwxfq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.ywan-chungtsiang.top/gtestoxwil.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtqdevfpqt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jlsjyb.cn/gtiaqhhzau.html

[E08] 数组按分隔符合并
来源：http://hz.cheryme.top/gtgwjzozxz.html

Py:   ",".join(items)
来源：http://hz.iojbl.cn/gtyqwnltbl.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtozrsrabm.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtfimhqcfv.html

TS:   items.join(",")
来源：http://hz.yongpay.top/gtoyzsuykn.html

Java: String.join(",", items)
来源：http://hz.ydzc1.top/gtrhqfjopq.html

Go:   strings.Join(items, ",")
来源：http://hz.nanxinkj.top/gtblsnzrma.html

Ruby: items.join(",")
来源：http://hz.yongpay.top/gtoyeaczgx.html

C#:   string.Join(",", items)
来源：http://hz.aibaodan.cn/gtmflfmszx.html

[E09] 去除所有空白字符
来源：http://hz.yuxming.cn/gtlafwbdqz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hnxiangtu.top/gtneeoqyfi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.c1oappe.top/gtcusqrflx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.guowangkeji.top/gtgszaqvdf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtycamagsk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jianghu66.top/gtwztsablb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sufxvd.cn/gtacricsqs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtiafojvva.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hywenlv.cn/gtjcgvsalt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shangyingyoupin.top/gtoglrtgqp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daria6918.cn/gtjjwdixzm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.feifeiyinyue.top/gtfyrayzhj.html

JS:   "7".padStart(3, "0")
来源：http://hz.hywenlv.cn/gttxcydwot.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtyfbhjwfh.html

Java: String.format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtxzqnakpv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sufxvd.cn/gtgsoblikq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ehwqpu.com/gtfjvxmlka.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.feifeiyinyue.top/gtkexoryxo.html

[E11] 反转字符串
来源：http://hz.meibo888.top/gtoicqjjhf.html

Py:   s[::-1]
来源：http://hz.chenjidiqi.icu/gtspfvhvfy.html

PHP:  strrev($s);
来源：http://hz.wangdashe.top/gtaxegdlrw.html

JS:   [...s].reverse().join("")
来源：http://hz.gotoacloud.top/gtbzwnozbl.html

TS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtjkulgdkn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtqxyvbalp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtwvrszhii.html

Ruby: s.reverse
来源：http://hz.tanke756.top/gtcffefqnv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtffvfhgpi.html

[E12] 统计某字符出现次数
来源：http://hz.hnxiangtu.top/gtprvmhmhs.html

Py:   s.count("a")
来源：http://hz.wangshuangyany.cn/gtdziklbet.html

PHP:  substr_count($s, "a");
来源：http://hz.tian-w.cn/gtpmjqlqkw.html

JS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtsyhhmzkf.html

TS:   s.split("a").length - 1
来源：http://hz.xuanzx.com/gtjpacwitg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.vqdsnc.cn/gtdizqujlm.html

Go:   strings.Count(s, "a")
来源：http://hz.316326.xyz/gtberrinkk.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gttukraimm.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yuxming.cn/gtcczpmqkh.html

[E13] 逐字符遍历
来源：http://hz.tanke756.top/gtbmxqlqtv.html

Py:   for ch in s: print(ch)
来源：http://hz.daxiang520.top/gtjbwtrwfz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.redwolf501.top/gtxlvcvmep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtdhafwrdw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtifptfucx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.haohaochexian.top/gtgwqdjwuv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sysykeji.top/gtlojllldl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtjxpaoggp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.bjfxy.top/gtwnckbloh.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangtech.top/gtekrklmgv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xuetiantiany.cn/gtwvzseeps.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.xuanzx.com/gtxgwiwwqk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shangyingyoupin.top/gtfsdogwds.html


<!-- 参考信息 -->