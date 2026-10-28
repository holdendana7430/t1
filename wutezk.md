代发 wailian999

Java: list.size();
来源：http://hz.daria6918.cn/gtlksfimpw.html

Go:   len(arr)
来源：http://hz.ybcxt.top/gttbugicyi.html

Ruby: arr.length; arr.size
来源：http://hz.yj20258888.top/gtokoccyud.html

C#:   list.Count;
来源：http://hz.aibaodan.cn/gtnoqeaylm.html

[D07] 切片 / 取子数组
来源：http://hz.gotoacloud.top/gtpfqbronv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhongyouzk.top/gtfoanrend.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shuidangran.top/gtjegndccn.html

JS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtqjavizfb.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtnqpbbqdy.html

Java: list.subList(1, 4);
来源：http://hz.jiagoushi.top/gtcakaefty.html

Go:   arr[1:4]
来源：http://hz.haohaochexian.top/gticydnxqm.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gtdhrvejkd.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtufmconrm.html

[D08] 合并两个数组
来源：http://hz.yvedp.cn/gtavmkphdm.html

Py:   a + b;  a.extend(b)
来源：http://hz.cashguo.top/gtzvkscvld.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtcdkuogav.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hywenlv.cn/gtoxogmeud.html

TS:   [...a, ...b];
来源：http://hz.haohaochexian.top/gtvjxmgiay.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xinyue.icu/gtnrrixjrs.html

Go:   append(a, b...)
来源：http://hz.fzhhl.top/gthecbnqmg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jyoumei.cn/gtnzknrgor.html

C#:   a.Concat(b).ToList()
来源：http://hz.feifeiyinyue.top/gtnewejjye.html

[D09] 排序（升序）
来源：http://hz.bjfxy.top/gttdjluenr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.redwolf501.top/gtgjovlxzi.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtzftmfsad.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtnwwworgd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtjmoevgkg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.birdmap.top/gtgjsezfku.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ybcxt.top/gtsiphcdha.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtdykkndsx.html

C#:   list.Sort();
来源：http://hz.yangfankeji.com/gtgdcyhsqg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yangfankeji.com/gtcvopvdoc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtkwiujbat.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydjk.org.cn/gtomvstxci.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtjvhisbyr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtgarflyoi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yuxming.cn/gtxzuopsim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gthqnuhwke.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtpdcvqbyo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtfssxsilo.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtktgemqmd.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xingfuxueyuan.xyz/gtrdugqqdb.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gthasunqzr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hysaishi.cn/gtjxyryjwc.html

TS:   [...arr].reverse();
来源：http://hz.jlsjyb.cn/gtliyjtpvq.html

Java: Collections.reverse(list);
来源：http://hz.sxryk.cn/gtqddrttjc.html

Go:   slices.Reverse(arr)
来源：http://hz.yangfankeji.com/gtqfpilxhe.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gtkqturhvx.html

C#:   list.Reverse();
来源：http://hz.jinghuilouyu.cn/gtsyxkxazb.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gttkrkkelg.html

Py:   arr.index(x);  x in arr
来源：http://hz.vqdsnc.cn/gttzylwgfc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xylfe.cn/gttijjfeit.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cdnleiting.top/gtjvmdrijo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtektadtlb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ehwqpu.com/gtzthukepn.html

Go:   slices.Index(arr, x)
来源：http://hz.jqgufenzy.top/gtfmbnwhhz.html

Ruby: arr.index(x)
来源：http://hz.yj202588.top/gtscjovgjm.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtudfbelrx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gaohongyu789.top/gtvllithhw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.c1oappe.top/gtlzoarkzi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinyuanbaomall.cn/gtqefhzwpo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtcykxlflr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtdcfkpyiz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenzaomai.com/gtzvaurpqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.kuanghao11.cn/gtifqojkms.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtdusaryjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenlongwang.top/gtmcespetl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtsqrhhfvs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuetiantiany.cn/gtziyydtzi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hywenlv.cn/gtaxsewnql.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtpicrcury.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhiwuduotai.top/gtltxhrkmx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xinyue.icu/gtlajevegs.html

Go:   // 手写循环
来源：http://hz.guowangkeji.top/gtabcfgffz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtsriirkvg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.bjfxy.top/gtrsppsrtk.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtkuctalmp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtdalchmke.html

PHP:  array_unique($arr);
来源：http://hz.dianchejie.cn/gtrquhtnye.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtaqxerpby.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtdelgusxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydzc1.top/gtftuhmfus.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtnymxjblp.html

Ruby: arr.uniq
来源：http://hz.nwbrower.top/gtyizhcpuf.html

C#:   list.Distinct().ToList()
来源：http://hz.tanke756.top/gtkdpnraor.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtmdrrhzuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gtdeqsouaa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.havefunace.top/gtavmtywis.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shanyushiyangtech.top/gtqaliwcab.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gtnqsmfitr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtbpgsywco.html

Go:   // 手写循环累加
来源：http://hz.cucudq.cn/gtpzhdwieq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gttwnovqil.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtrsazsnpo.html

[D17] 最大值与最小值
来源：http://hz.52xcode.cn/gtrbzxkpbw.html

Py:   max(arr);  min(arr)
来源：http://hz.kuanghao11.cn/gtvuextqqg.html

PHP:  max($arr);  min($arr);
来源：http://hz.ppjwa.cn/gtrkagmjbq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtwajqdzom.html

TS:   Math.max(...arr);
来源：http://hz.zhijiandao.cn/gtdbzeywnn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.52xcode.cn/gtoqcxnntn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhixingplan.top/gtunfhoeuw.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtktqkwgym.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtblnnukho.html

[D18] 扁平化嵌套数组
来源：http://hz.chenzaomai.com/gtrtgebhod.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xuetiantiany.cn/gtkfoqefak.html

PHP:  array_merge(...$nested);
来源：http://hz.sxryk.cn/gtkdjtutiz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.316326.xyz/gtxniuanzr.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtmvuwalrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.52xcode.cn/gtvoqhqcpv.html

Go:   // 手写双层循环
来源：http://hz.guannengcc.top/gtnqgwfege.html

Ruby: nested.flatten
来源：http://hz.cdnleiting.top/gtueoxnctx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.cucudq.cn/gtrlowmwdi.html

[D19] 按字段分组
来源：http://hz.haohaochexian.top/gtydksfgwv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.daria6918.cn/gtnbqtvbzx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhiwuduotai.top/gthdffggba.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgfzy.top/gtwgwoebwc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gotoacloud.top/gtjpbzulga.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtlbfxpqrb.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gthspbqqua.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zdqjudy.top/gtnujuscjg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cqqwz.cn/gtshvyzplj.html

[D20] 统计每个元素出现次数
来源：http://hz.cheryme.top/gtrrdndsix.html

Py:   Counter(arr)
来源：http://hz.yvedp.cn/gtqdzlzlsn.html

PHP:  array_count_values($arr);
来源：http://hz.nwbrower.top/gthjqlpfpj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hfpthk.cn/gtktreevad.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtoimlydkh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhengqikj.top/gtquxkwssx.html

Go:   // 手写 map[T]int
来源：http://hz.hongshengwenyu.top/gttckniuoy.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtbbxienym.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenjidiqi.icu/gtcwddgkqw.html

[D21] 判断是否包含某元素
来源：http://hz.dianchejie.cn/gtcufxddga.html

Py:   x in arr
来源：http://hz.pycfn.com/gtnoskpwkr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xingfuxueyuan.xyz/gtdajtfhzx.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtwxbvzxzu.html

TS:   arr.includes(x)
来源：http://hz.xuanzx.com/gtuntakefl.html

Java: list.contains(x)
来源：http://hz.cashguo.top/gthnovqrpg.html

Go:   slices.Contains(arr, x)
来源：http://hz.jyoumei.cn/gtiormhpex.html

Ruby: arr.include?(x)
来源：http://hz.cqqwz.cn/gtvfjgncaq.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtwlubewvh.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pengpengdd.cyou/gtyavhnpvn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gtoktkfoyy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtgchsgopg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtpswexslw.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtkiigblnz.html

Java: new ArrayList<>(list);
来源：http://hz.dashuyun.cn/gtnoxjmqxx.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhaomingkeji.xyz/gthbrjunyg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtlutrvalo.html

C#:   new List<int>(list);
来源：http://hz.gzhubu.top/gtapcbughl.html

[D23] reduce 累积计算
来源：http://hz.vqdsnc.cn/gtbcwxryss.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtltbhilpi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtkculisyi.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtxrizpnts.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtwzfydvev.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.wangdashe.top/gtydhebimn.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gtivnssmtl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sysykeji.top/gtastvhuhv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.smart0.xyz/gtiuukyyuj.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinyuanbaomall.cn/gtlknxneml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.chenjidiqi.icu/gtzthtvqug.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gtmoopzpcf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sufxvd.cn/gteyzxuvct.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenlongwang.top/gtevizayxi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gtgujyrhqs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtczdgvzyv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yj20258.top/gtoymiexeo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.svipenyu.cn/gtjngezxrl.html

[D25] Set 集合去重与交并差
来源：http://hz.yuanzhike.top/gtymzfoxxy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.52xcode.cn/gtbosplrti.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nwbrower.top/gtwhvtwdkj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yangfankeji.com/gtrfkgocvk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jqgfzy.top/gtjgkmalfm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xziqi.cn/gtlxnregtt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cheryme.top/gtzkrezuqa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yvedp.cn/gtmhifphus.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtajltjgsw.html

[D26] 数组转字符串
来源：http://hz.vqdsnc.cn/gtxroytsdk.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hammf.cn/gtgscwtpvz.html

PHP:  implode(", ", $arr);
来源：http://hz.shangyingyoupin.top/gtqhbhsinw.html

JS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtveofvgya.html

TS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtuyyjxued.html

Java: String.join(", ", list)
来源：http://hz.shangyingyoupin.top/gtwavzfqqw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.daxiang520.top/gtalmmvvky.html

Ruby: arr.join(", ")
来源：http://hz.gaohongyu789.top/gtjodkflxx.html

C#:   string.Join(", ", list)
来源：http://hz.svipenyu.cn/gtbvnjydgt.html

================================================================================
来源：http://hz.ehwqpu.com/gtdztjdzoq.html

E. 字符串处理
来源：http://hz.shzxlz.cn/gtisvydbat.html

================================================================================
来源：http://hz.nanxinkj.top/gtdwjgpbes.html

[E01] 拼接字符串
来源：http://hz.zhijiandao.cn/gtlwrnbmob.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yvedp.cn/gtcdyhcsog.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.havefunace.top/gtkumljshi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtsfawmlsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtwbnvcneb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnxiangtu.top/gtnopjaldz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.chenzaomai.com/gtfwftundk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yangfankeji.com/gtgmdzbsho.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sxryk.cn/gtofrdxgcm.html

[E02] 重复字符串
来源：http://hz.jinyuanbaomall.cn/gtotoinsrs.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gthxqyuzkb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nanxinkj.top/gtvstegtea.html

JS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtoxtnwagj.html

TS:   "ab".repeat(3)
来源：http://hz.cheryme.top/gttzkafwcn.html

Java: "ab".repeat(3)
来源：http://hz.havefunace.top/gtnqvaebmt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.pycfn.com/gtfpnzknqd.html

Ruby: "ab" * 3
来源：http://hz.snrcjt.cn/gtwjifchea.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.vqdsnc.cn/gtegakhraf.html

[E03] 截取子串
来源：http://hz.aibaodan.cn/gtarghuuso.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtifgjhiwt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.smart0.xyz/gtfbhndvtq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jiagoushi.top/gtxbmsyrhf.html

TS:   s.slice(1, 4)
来源：http://hz.yj202588.top/gthmkctbug.html

Java: s.substring(1, 4)
来源：http://hz.smart0.xyz/gtbcanwpiw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenzaomai.com/gtzjxqjewu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.guowangkeji.top/gtmofnyelf.html

C#:   s.Substring(1, 3)
来源：http://hz.yj20258888.top/gtrgzsvdzt.html

[E04] 查找子串位置
来源：http://hz.pycfn.com/gtlvjbfnyg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtjslamrwa.html

PHP:  strpos($s, "x");
来源：http://hz.xingfuxueyuan.xyz/gtseiopiuz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.pengpengdd.cyou/gtajcmomet.html

TS:   s.indexOf("x")
来源：http://hz.yonumen.top/gtawsqyjmw.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gtogxnkvfo.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtyjeqgsis.html

Ruby: s.index("x")
来源：http://hz.jqgufenzy.top/gtuqxjxwat.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtjnerhect.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.nanxuanxn.top/gtxjbtkidd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhaomingkeji.xyz/gtqlltrhni.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jqgufenzy.top/gtxpeflhnz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gtebkasdjm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtisaazbby.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.sweek.top/gttopwsqab.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258888.top/gtzpeleuus.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.feifeiyinyue.top/gtxeecgyhj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.havefunace.top/gttoogchyd.html

[E06] 替换子串
来源：http://hz.zhijiandao.cn/gtmhldsmdy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtqtncajmh.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cheryme.top/gtiehfoqsc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtqkpymbfn.html

TS:   s.replaceAll("a", "b")
来源：http://hz.smart0.xyz/gtkdlqsfow.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtrjstfceq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nwbrower.top/gtiwkiirfy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenlongwang.top/gtmvrraszs.html

C#:   s.Replace("a", "b")
来源：http://hz.316326.xyz/gtfqisvtcq.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtrqvrwmvt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtduuptssj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtjrevlmeu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yonumen.top/gtmfpkhkvi.html

TS:   s.split(",")
来源：http://hz.hnxiangtu.top/gtgoitemqw.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jyoumei.cn/gtyvnmfhvq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj202588.top/gtramsjzpw.html

Ruby: s.split(",");  s.split
来源：http://hz.dashuyun.cn/gtjidntmqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtkkmmxobr.html

[E08] 数组按分隔符合并
来源：http://hz.bjfxy.top/gtgxggrdbj.html

Py:   ",".join(items)
来源：http://hz.jqgfzy.top/gtoohdtsjz.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtonzmhkir.html

JS:   items.join(",")
来源：http://hz.jinghuilouyu.cn/gtssyemtdx.html

TS:   items.join(",")
来源：http://hz.pengpengdd.cyou/gtpoyawlif.html

Java: String.join(",", items)
来源：http://hz.guowangkeji.top/gtskbvkdiw.html

Go:   strings.Join(items, ",")
来源：http://hz.daria6918.cn/gthztubqig.html

Ruby: items.join(",")
来源：http://hz.sweek.top/gtjbkrrvyt.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gthgagdjtw.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtdlmkhdaw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.redwolf501.top/gtdhqeksme.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtipsuiqyk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtvphqbblp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shzxlz.cn/gtvqtyfmqf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yuanzhike.top/gtvaqmxtqw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ivvv.top/gtnlwkbrnw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sufxvd.cn/gtzznjuokw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.cheryme.top/gtibndgbwl.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hongshengwenyu.top/gtyqytsiwb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shanyushiyangkeji.top/gtnhzxuffp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtfgwgiueu.html

JS:   "7".padStart(3, "0")
来源：http://hz.ydjk.org.cn/gtgpzozzfi.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtwyukbleg.html

Java: String.format("%03d", 7)
来源：http://hz.gogol.net.cn/gtgrpeejyo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.shanyushiyangkeji.top/gtcoujebjx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cucudq.cn/gtaxrjhwcc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ydzc1.top/gtwanazbsu.html

[E11] 反转字符串
来源：http://hz.hywenlv.cn/gttwpuwzxv.html

Py:   s[::-1]
来源：http://hz.hongshengwenyu.top/gtjhqggxay.html

PHP:  strrev($s);
来源：http://hz.iojbl.cn/gtjxkhpuwi.html

JS:   [...s].reverse().join("")
来源：http://hz.sysykeji.top/gtowqmtclc.html

TS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtwtklkbbb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtnmwynxoh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ehwqpu.com/gtsprjueno.html

Ruby: s.reverse
来源：http://hz.kuanghao11.cn/gtsjpminlv.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nwbrower.top/gtbasuwdpl.html

[E12] 统计某字符出现次数
来源：http://hz.xziqi.cn/gtmohvetsh.html

Py:   s.count("a")
来源：http://hz.sxryk.cn/gttejivoqv.html

PHP:  substr_count($s, "a");
来源：http://hz.yuanzhike.top/gtaswxqmbo.html

JS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtxujxwhdl.html

TS:   s.split("a").length - 1
来源：http://hz.chenzaomai.com/gtvvixvoxj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.smart0.xyz/gtzcscvceg.html

Go:   strings.Count(s, "a")
来源：http://hz.gotoacloud.top/gtqvoeeovj.html

Ruby: s.count("a")
来源：http://hz.aizwys.cn/gtxwllbgii.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenlongwang.top/gtnjwdsssp.html

[E13] 逐字符遍历
来源：http://hz.9152youxi.cn/gtqfsgldjk.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gtcluhirmf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sxryk.cn/gtpwiljduc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shuidangran.top/gtodwlppbc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenzaomai.com/gtcfzbqpnq.html


<!-- 参考信息 -->