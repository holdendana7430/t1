代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.shanyushiyangkeji.top/gtfpbcxevm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.daria6918.cn/gtovhrhuib.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtvhtejqgs.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtbszydllo.html

TS:   arr.slice(1, 4);
来源：http://hz.52xcode.cn/gthokncdwj.html

Java: list.subList(1, 4);
来源：http://hz.hammf.cn/gtzsrmykeq.html

Go:   arr[1:4]
来源：http://hz.yongpay.top/gtnmtguqjd.html

Ruby: arr[1, 3]
来源：http://hz.sufxvd.cn/gtzifgzpel.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhaomingkeji.xyz/gtdouhyuje.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtucozympa.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtjirpduvo.html

PHP:  array_merge($a, $b);
来源：http://hz.iojbl.cn/gtmrgbxmbg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtnkqyliyo.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtrdnsszgx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.fzhhl.top/gtxuctsxij.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtlikiurnl.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jianghu66.top/gtudolmrej.html

C#:   a.Concat(b).ToList()
来源：http://hz.yj20258.top/gtcbjacpiw.html

[D09] 排序（升序）
来源：http://hz.zhengqikj.top/gtupikcayf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtklepckqc.html

PHP:  sort($arr);
来源：http://hz.gaohongyu789.top/gtqntmudzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yangfankeji.com/gtmxkbvhcs.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.0kj1m.cn/gtfqdvvzot.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtcdsmojjw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtpiobzbpg.html

Ruby: arr.sort
来源：http://hz.jqgfzy.top/gtncrlppss.html

C#:   list.Sort();
来源：http://hz.sxryk.cn/gtvgurjlqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jiagoushi.top/gtcwdiepvu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.c1oappe.top/gtshufcnku.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtbecxfheu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtgedwxtfl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daxiang520.top/gtksmkdjea.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sxryk.cn/gtlwxtxxec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sufxvd.cn/gtuuewcswr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj20258.top/gtkvapoqek.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shuidangran.top/gtcerxkmoq.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gtvfctijwn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yonumen.top/gtlxjysnqs.html

PHP:  array_reverse($arr);
来源：http://hz.svipenyu.cn/gteqtckmob.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xinyue.icu/gtuwwoiueg.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtozgqsdap.html

Java: Collections.reverse(list);
来源：http://hz.redwolf501.top/gtehzpqrpd.html

Go:   slices.Reverse(arr)
来源：http://hz.xziqi.cn/gtngwkzcut.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtlpebnbwh.html

C#:   list.Reverse();
来源：http://hz.jinyuanbaomall.cn/gtgwgvgmyh.html

[D12] 查找元素下标
来源：http://hz.shangyingyoupin.top/gtguuoirmg.html

Py:   arr.index(x);  x in arr
来源：http://hz.mhx1999.top/gtrzcpfpcw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.dashuyun.cn/gtkdpbonef.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtkhwldbzf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtkkppmusk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtlxmnwbgp.html

Go:   slices.Index(arr, x)
来源：http://hz.yuxming.cn/gtomxvhkvo.html

Ruby: arr.index(x)
来源：http://hz.aizwys.cn/gtoqtfqxmw.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtyvbshepk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtizsfiyzf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cheryme.top/gtzjyqdryz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cheryme.top/gtxcegsall.html

JS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtapyltkaj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtswsriwcn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj20258888.top/gthjenfnql.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gtuwmajnfy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ppjwa.cn/gtkbmudsjc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangtech.top/gtkauehldr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtkifuidcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtmxrzsart.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gtmlkmtuob.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtqxqenjdf.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gttehzcxbe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.feifeiyinyue.top/gtapopjnxg.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtibholgov.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gteuzccafj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.daria6918.cn/gtnptgicit.html

[D15] 去重
来源：http://hz.snrcjt.cn/gtbbuedyit.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtwxatxmxo.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtwkdvmbev.html

JS:   [...new Set(arr)]
来源：http://hz.snrcjt.cn/gtzilppczq.html

TS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtwbdlhpvj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.pycfn.com/gtjfkcijyd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtnwdrzcmp.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtwyzgtfsx.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtyngatuka.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtperkufcn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtvrzaojtp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xingfuxueyuan.xyz/gtfdexnzaf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtndvhmvky.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtimnuzhpw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtigvrkuzr.html

Go:   // 手写循环累加
来源：http://hz.jianghu66.top/gtslsimaoc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtzbmsvptm.html

C#:   list.Sum();  list.Average()
来源：http://hz.tianlin.xyz/gtsmizemnb.html

[D17] 最大值与最小值
来源：http://hz.zhixingplan.top/gtpkvznfft.html

Py:   max(arr);  min(arr)
来源：http://hz.zhongyouzk.top/gtkljpergu.html

PHP:  max($arr);  min($arr);
来源：http://hz.mhx1999.top/gtxwydbtzl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gtlofqleud.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gteucexqzi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yonumen.top/gtqjzemhkd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jianghu66.top/gtjbzgjehh.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtpwovhpoa.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gtmvpiwyst.html

[D18] 扁平化嵌套数组
来源：http://hz.xuetiantiany.cn/gticwtkwgu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hnqzz.top/gtxeyodsoi.html

PHP:  array_merge(...$nested);
来源：http://hz.cucudq.cn/gtmjpxwtxo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hammf.cn/gtotvtrlln.html

TS:   nested.flat();
来源：http://hz.cqqwz.cn/gtsmnhbite.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gotoacloud.top/gtlhypqoxr.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gthttburpa.html

Ruby: nested.flatten
来源：http://hz.zhaomingkeji.xyz/gtjruhjhgg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gtltjqscnl.html

[D19] 按字段分组
来源：http://hz.yanxiufei.cn/gttjudtdvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtlqmzhmji.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gttwpyfnzu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xingfuxueyuan.xyz/gttqdprxan.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtbwlcayls.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtodjbqiaw.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtsvbgdyng.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhongyouzk.top/gtamosnbdz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jlsjyb.cn/gtvwvhsifi.html

[D20] 统计每个元素出现次数
来源：http://hz.aizwys.cn/gtqeboabkw.html

Py:   Counter(arr)
来源：http://hz.xylfe.cn/gttzqtdijw.html

PHP:  array_count_values($arr);
来源：http://hz.0kj1m.cn/gtpiiemujt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtuzfpzapn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtjcyfiawr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hywenlv.cn/gtomjbsrjf.html

Go:   // 手写 map[T]int
来源：http://hz.vqdsnc.cn/gtdgbbjlom.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtvucssqae.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gttyrfppyh.html

[D21] 判断是否包含某元素
来源：http://hz.sysykeji.top/gtuhwvbdlc.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtwppjdbiv.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gthuxfqkyl.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtfycnaheq.html

TS:   arr.includes(x)
来源：http://hz.xylfe.cn/gtrkmtpzml.html

Java: list.contains(x)
来源：http://hz.nanxinkj.top/gthnjpglcp.html

Go:   slices.Contains(arr, x)
来源：http://hz.smart0.xyz/gtvouetbpc.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtpphfuoeb.html

C#:   list.Contains(x)
来源：http://hz.tian-w.cn/gtueqvndve.html

[D22] 复制数组（避免共享引用）
来源：http://hz.snrcjt.cn/gtwfezjnyn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.shangyingyoupin.top/gtbbybnliq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hywenlv.cn/gtgpxmfsqc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtqriigahc.html

TS:   [...arr];
来源：http://hz.quarkkingdee.top/gtniqjklwt.html

Java: new ArrayList<>(list);
来源：http://hz.ppjwa.cn/gtjthnjpga.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ehwqpu.com/gtgpntyjek.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yonumen.top/gtccincxrp.html

C#:   new List<int>(list);
来源：http://hz.cucudq.cn/gtxkwrpvzm.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtcncojccw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydjk.org.cn/gtwbcdfqfd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.redwolf501.top/gtzrmfgskx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtcscfoeuj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gthyznpvbv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.snrcjt.cn/gtydywzlkh.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtxjiyjqlt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.smart0.xyz/gteppfkykx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shangyingyoupin.top/gtwpahhokl.html

[D24] 字典 / Map 基本操作
来源：http://hz.cashguo.top/gtxxwhqioo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hysaishi.cn/gtotipfuui.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xingfuxueyuan.xyz/gtvmryrsoc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yuanzhike.top/gtyzmsvsuh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.daxiang520.top/gtaxddmvcw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ybcxt.top/gtdbromhyo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtorrrfssx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ybcxt.top/gtcfjqmzbr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.316326.xyz/gtmoxqfqpa.html

[D25] Set 集合去重与交并差
来源：http://hz.hnqzz.top/gtlosapfpb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xinyue.icu/gtlopdpozw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtlfxtckeg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.wangshuangyany.cn/gtmneelrbx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jianghu66.top/gtnddzjwgw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtvdwehtje.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtbffumerg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtwssnhmfs.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinghuilouyu.cn/gtwgxiscmd.html

[D26] 数组转字符串
来源：http://hz.yangfankeji.com/gtvsmrehdy.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sxryk.cn/gtnojxrtwo.html

PHP:  implode(", ", $arr);
来源：http://hz.316326.xyz/gtvzvcwsns.html

JS:   arr.join(", ")
来源：http://hz.andypj.xyz/gtmoyfvjud.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtmqsardmr.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtitcvmopn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xziqi.cn/gtlrvfsepk.html

Ruby: arr.join(", ")
来源：http://hz.yanxiufei.cn/gtczrdxpqh.html

C#:   string.Join(", ", list)
来源：http://hz.zhengqikj.top/gtjsutzixn.html

================================================================================
来源：http://hz.cdnleiting.top/gtjwvtbllm.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtxqlccxld.html

================================================================================
来源：http://hz.ydzc1.top/gthoexnohx.html

[E01] 拼接字符串
来源：http://hz.tianlin.xyz/gtntjgxepy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ybcxt.top/gtxniawuuy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtganpunjk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhengqikj.top/gtdhkkhogu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.kuanghao11.cn/gtumtyvpzs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtaprghkxr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.dashuyun.cn/gtdtjglowh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtrhbfuutf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.9152youxi.cn/gtdyckcxih.html

[E02] 重复字符串
来源：http://hz.ybcxt.top/gtxnthxcyj.html

Py:   "ab" * 3
来源：http://hz.0kj1m.cn/gtyunjzuuf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.iojbl.cn/gtgptmqvwl.html

JS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtooyboyxy.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtajzexbrt.html

Java: "ab".repeat(3)
来源：http://hz.xinyue.icu/gtaimjjxhp.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gtwjfhippv.html

Ruby: "ab" * 3
来源：http://hz.0kj1m.cn/gtvjjyzigk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.quarkkingdee.top/gtwvhwokfr.html

[E03] 截取子串
来源：http://hz.bjfxy.top/gtnoayjkuh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.iojbl.cn/gttdgyyaiw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zhengqikj.top/gtxuvskepo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.c1oappe.top/gtrbdrtnrw.html

TS:   s.slice(1, 4)
来源：http://hz.nanxuanxn.top/gtiljsmfaq.html

Java: s.substring(1, 4)
来源：http://hz.yuanzhike.top/gtekubtydv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinghuilouyu.cn/gtzrwkfops.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtywfmljzl.html

C#:   s.Substring(1, 3)
来源：http://hz.nwbrower.top/gtragztpxo.html

[E04] 查找子串位置
来源：http://hz.52xcode.cn/gtzmjwcuam.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtuzaopzia.html

PHP:  strpos($s, "x");
来源：http://hz.birdmap.top/gtjjeivzgb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.smart0.xyz/gtmimabqdn.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtnuturedp.html

Java: s.indexOf("x")
来源：http://hz.xziqi.cn/gtcnmtrmur.html

Go:   strings.Index(s, "x")
来源：http://hz.zhaomingkeji.xyz/gtvmwsjcvk.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gthtziozye.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtssflblho.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.wangdashe.top/gtddzohyoe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hfpthk.cn/gtcmkleeht.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hysaishi.cn/gtzwtfuakn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.ywan-chungtsiang.top/gttwweccbx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.mhx1999.top/gtavpejaxa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.0kj1m.cn/gtlixiywaa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xinyue.icu/gtpdhhodxk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhiwuduotai.top/gtvprsdlbp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nwbrower.top/gtqbhpovzv.html

[E06] 替换子串
来源：http://hz.nanxuanxn.top/gtlasmosci.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtbmlnpddo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.tianlin.xyz/gtzqfunfxx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtkkmcgvgc.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cdnleiting.top/gtufuutebv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtgykqbqks.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtibdnzcnq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.nwbrower.top/gtqdtpzkmt.html

C#:   s.Replace("a", "b")
来源：http://hz.cashguo.top/gtlgwxqxkl.html

[E07] 按分隔符拆分
来源：http://hz.cashguo.top/gtqfmssayz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtmtlxhdfv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigfzy.top/gtrgdzlwas.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.fengsongda.top/gtdzmotssl.html

TS:   s.split(",")
来源：http://hz.jinqigufen.top/gtwyazkyau.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.mhx1999.top/gtuhnqqihq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cashguo.top/gtvmclksxp.html

Ruby: s.split(",");  s.split
来源：http://hz.gzhubu.top/gtdcfabfut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ppjwa.cn/gtmxabjlrx.html

[E08] 数组按分隔符合并
来源：http://hz.nanxuanxn.top/gtdeiareji.html

Py:   ",".join(items)
来源：http://hz.gaohongyu789.top/gtwcgxpuvu.html

PHP:  implode(",", $items);
来源：http://hz.jqgfzy.top/gtutaidxky.html

JS:   items.join(",")
来源：http://hz.chenzaomai.com/gtulkahvtf.html

TS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtfcffvdus.html

Java: String.join(",", items)
来源：http://hz.fengsongda.top/gtolwxqazk.html

Go:   strings.Join(items, ",")
来源：http://hz.pycfn.com/gtknovfoao.html

Ruby: items.join(",")
来源：http://hz.wangshuangyany.cn/gtnliwlocx.html

C#:   string.Join(",", items)
来源：http://hz.sufxvd.cn/gtdrlyvxkl.html

[E09] 去除所有空白字符
来源：http://hz.hysaishi.cn/gttwniuhpq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gtlumjvhtj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.iojbl.cn/gtytxyklui.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.zhongyouzk.top/gtflztyscb.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.tian-w.cn/gtsdxakpmg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.chenjidiqi.icu/gtfxpzqmtj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.sweek.top/gttmzyyzsg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cashguo.top/gtqjiolmkq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.9152youxi.cn/gtfcenlqkx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.316326.xyz/gtllgbsgfd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zdqjudy.top/gtwegpyzvb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.cashguo.top/gtjyyobhvq.html

JS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtchqwjndc.html

TS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtgvomluzy.html

Java: String.format("%03d", 7)
来源：http://hz.xuetiantiany.cn/gtbjavuzch.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.cashguo.top/gtfdzffgvz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.hysaishi.cn/gteeunkotb.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.wangdashe.top/gtywofszdq.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtcyvbeltj.html

Py:   s[::-1]
来源：http://hz.svipenyu.cn/gtospelgtl.html

PHP:  strrev($s);
来源：http://hz.havefunace.top/gtrjzcjquo.html

JS:   [...s].reverse().join("")
来源：http://hz.zhoulong.xyz/gtufzkuggf.html

TS:   [...s].reverse().join("")
来源：http://hz.tian-w.cn/gtvzcwlccq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ydzc1.top/gtnfwukavb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtooqapxvo.html

Ruby: s.reverse
来源：http://hz.tian-w.cn/gtbfswbono.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangtech.top/gtzkdfbkhe.html

[E12] 统计某字符出现次数
来源：http://hz.sufxvd.cn/gtfrzifzkc.html

Py:   s.count("a")
来源：http://hz.jqgfzy.top/gtmrqkyzjl.html

PHP:  substr_count($s, "a");
来源：http://hz.52xcode.cn/gtndmppnvh.html

JS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtlygjsrzt.html

TS:   s.split("a").length - 1
来源：http://hz.jiagoushi.top/gtooluxseg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.meibo888.top/gtdvtezybe.html

Go:   strings.Count(s, "a")
来源：http://hz.zhoulong.xyz/gtvkvidxsh.html

Ruby: s.count("a")
来源：http://hz.jlsjyb.cn/gtcosqistz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.hnxiangtu.top/gtkbzdmzjx.html

[E13] 逐字符遍历
来源：http://hz.redwolf501.top/gtmivccgce.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxinkj.top/gtmjdwpyxd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtvwmmhbyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhongyouzk.top/gtcuguuahp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtpaciylmz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.52xcode.cn/gtkairsrhl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.havefunace.top/gtnwfjtthn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.svipenyu.cn/gtmcbaoggj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hywenlv.cn/gtvrfethqr.html


<!-- 参考信息 -->