代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtfzirhtcu.html

[D08] 合并两个数组
来源：http://hz.0kj1m.cn/gtsnbvsghp.html

Py:   a + b;  a.extend(b)
来源：http://hz.dashuyun.cn/gtmbeopozp.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtawdwplub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtfhvkurnf.html

TS:   [...a, ...b];
来源：http://hz.guowangkeji.top/gtgtrheclz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cucudq.cn/gtecgcqjsu.html

Go:   append(a, b...)
来源：http://hz.yanxiufei.cn/gtsklcgcgx.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtnxwccbxq.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhiwuduotai.top/gtexqmoggb.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtgtntadox.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.chenzaomai.com/gtkpnneqix.html

PHP:  sort($arr);
来源：http://hz.jqgfzy.top/gtztmzpvri.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shanyushiyangtech.top/gtdqrsthjd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jlsjyb.cn/gtdnmoulzq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangtech.top/gtjzetrgbw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenzaomai.com/gtlbjmucsp.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtphaanash.html

C#:   list.Sort();
来源：http://hz.hywenlv.cn/gtamnophtq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yanxiufei.cn/gtpsgjhpvg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.jinghuilouyu.cn/gtfszabjmp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtqttcmhvn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gthtmmzuqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtmuzirfdr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxinkj.top/gtpghckofy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yueranfly.top/gthwoskinx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guannengcc.top/gtyxdmfcmt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gthpngdgps.html

[D11] 反转数组
来源：http://hz.shuidangran.top/gtjpzandlc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shzxlz.cn/gthnzmsrrb.html

PHP:  array_reverse($arr);
来源：http://hz.fzhhl.top/gtddvgohgh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sweek.top/gtqbssgopa.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtpgehvezi.html

Java: Collections.reverse(list);
来源：http://hz.yj202588.top/gtowwegjtb.html

Go:   slices.Reverse(arr)
来源：http://hz.jinghuilouyu.cn/gtcbmcofer.html

Ruby: arr.reverse
来源：http://hz.yj20258.top/gtljitalxb.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtlxlyhkad.html

[D12] 查找元素下标
来源：http://hz.aizwys.cn/gtsyswsifh.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtoexpdtgo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gtqfabayak.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guannengcc.top/gtjwkxjapa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtfdgrpgkj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jianghu66.top/gtnymfvjfs.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtdxicxxfj.html

Ruby: arr.index(x)
来源：http://hz.yonumen.top/gtvhkxvxxa.html

C#:   list.IndexOf(x);
来源：http://hz.yueranfly.top/gtbrxbqjqy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.iojbl.cn/gtqmbpkdaw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhixingplan.top/gtkjrlajfj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuxming.cn/gtopofdgfy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtjcbbzrnw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangkeji.top/gtkwgnmxej.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtkqnqovnd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gzhubu.top/gtavpsieci.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtnkpkapnf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tian-w.cn/gtviryacaf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yvedp.cn/gtcxdpmtgl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtpvowrfxv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fengsongda.top/gttqoijfrs.html

JS:   arr.map(x => x * 2)
来源：http://hz.mhx1999.top/gtfckvmyku.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gtrnvmlqmg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenlongwang.top/gtfpgxcbix.html

Go:   // 手写循环
来源：http://hz.meibo888.top/gtookjxzab.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cqqwz.cn/gtqgtqybph.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtegobebpr.html

[D15] 去重
来源：http://hz.yueranfly.top/gtiuztqnnu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtittdrcle.html

PHP:  array_unique($arr);
来源：http://hz.cdnleiting.top/gtmasvcxyw.html

JS:   [...new Set(arr)]
来源：http://hz.daria6918.cn/gtvcgbxfyg.html

TS:   [...new Set(arr)]
来源：http://hz.ybcxt.top/gtwmqtgwgc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sysykeji.top/gtdyguubnv.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shuidangran.top/gtertljcld.html

Ruby: arr.uniq
来源：http://hz.yj202588.top/gtswnsojhg.html

C#:   list.Distinct().ToList()
来源：http://hz.gotoacloud.top/gtduuohfaa.html

[D16] 求和与平均值
来源：http://hz.sufxvd.cn/gtxggdxiqq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gzhubu.top/gtifgfdxzn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zdqjudy.top/gtcumthenn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtvljwuwbw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ivvv.top/gtioxjordr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gtmxeutafw.html

Go:   // 手写循环累加
来源：http://hz.shzxlz.cn/gtprhcjfic.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.shzxlz.cn/gtooohqaut.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtdeqnyupe.html

[D17] 最大值与最小值
来源：http://hz.yuanzhike.top/gtyxgeycug.html

Py:   max(arr);  min(arr)
来源：http://hz.chenlongwang.top/gtohjtfepp.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtyrchlkdr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.bjfxy.top/gtzentmhru.html

TS:   Math.max(...arr);
来源：http://hz.wangshuangyany.cn/gtxgutuwah.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jyoumei.cn/gthqjwzkln.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xuetiantiany.cn/gtjpmkkhat.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtrrrflyqr.html

C#:   list.Max();  list.Min()
来源：http://hz.yueranfly.top/gttmtwdrdd.html

[D18] 扁平化嵌套数组
来源：http://hz.jyoumei.cn/gtzfzqwfcj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtibdsixho.html

PHP:  array_merge(...$nested);
来源：http://hz.xylfe.cn/gtjaumhaqa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtmwumjlok.html

TS:   nested.flat();
来源：http://hz.ydzc1.top/gtbgiftlis.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtcqxzwjgd.html

Go:   // 手写双层循环
来源：http://hz.ydjk.org.cn/gtlimvywjl.html

Ruby: nested.flatten
来源：http://hz.yonumen.top/gtsqxiqytl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtesmuteeq.html

[D19] 按字段分组
来源：http://hz.zhoulong.xyz/gtbmjialyt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jlsjyb.cn/gtznjchmwn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gtpzhdunib.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnxiangtu.top/gtolwpgjok.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.quarkkingdee.top/gtfqvofppk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gtaxrhvvax.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtkyjjbiex.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fzhhl.top/gtsvnlrkki.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.nwbrower.top/gtzvsswhnc.html

[D20] 统计每个元素出现次数
来源：http://hz.tanke756.top/gtoxqovkzf.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtqyfddejs.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtxbpkreng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gttpwslcbs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yongpay.top/gtmclcccgn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yonumen.top/gtkgiscers.html

Go:   // 手写 map[T]int
来源：http://hz.jqgufenzy.top/gtgiibpkhb.html

Ruby: arr.tally
来源：http://hz.yangfankeji.com/gtiqybcubx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.iojbl.cn/gtkwbzwzab.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigfzy.top/gtcsmskmki.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtvzhfmrug.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhoulong.xyz/gtgcmijyqd.html

JS:   arr.includes(x)
来源：http://hz.ybcxt.top/gteupxwocx.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtgzvewokt.html

Java: list.contains(x)
来源：http://hz.sysykeji.top/gtgfjwvzcf.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinghuilouyu.cn/gtsgtviwqk.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtvdqwqqcv.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtucnblfyg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.nanxinkj.top/gtkmkagzdn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hywenlv.cn/gttbkemulh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yangfankeji.com/gtxvxkokha.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gteyvrmdml.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtjaeushfk.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtcnqzoszb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhoulong.xyz/gtnbijgllq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yueranfly.top/gtznxyymfw.html

C#:   new List<int>(list);
来源：http://hz.havefunace.top/gtigfatynz.html

[D23] reduce 累积计算
来源：http://hz.yongpay.top/gtcoxzjvao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnxiangtu.top/gtypnucqza.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenzaomai.com/gtkmmgjpda.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xziqi.cn/gtzrxegszl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtpajtkkao.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gzhubu.top/gtelcvmbyr.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtfejanajb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtcmmvydrq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gthgfdyzik.html

[D24] 字典 / Map 基本操作
来源：http://hz.yueranfly.top/gtvghucyjj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxinkj.top/gtkuknchmn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnxiangtu.top/gttkmuswxt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.nanxinkj.top/gtmmwgsutc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.iojbl.cn/gtrljzzwar.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj20258.top/gtepssdzrt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jianghu66.top/gtojadkani.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hnxiangtu.top/gtcgnkcjpi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangkeji.top/gtvwqnpmyz.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtgymbakrm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.dianchejie.cn/gtckgowooh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangshuangyany.cn/gtqiiagyva.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.bjfxy.top/gtodpbeedp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtgrcjgqkt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtlisdbawe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhoulong.xyz/gtlpupjqbd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shuidangran.top/gtdooujpud.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hnqzz.top/gtrlcmyetb.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gtmggfqtmq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtpslsfyun.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtjetwkxlv.html

JS:   arr.join(", ")
来源：http://hz.jinghuilouyu.cn/gtpijyoqqi.html

TS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtpgbfbfai.html

Java: String.join(", ", list)
来源：http://hz.yueranfly.top/gtufnnwodc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.nanxuanxn.top/gtsuyogzft.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtohdxtrnj.html

C#:   string.Join(", ", list)
来源：http://hz.hywenlv.cn/gtndyathli.html

================================================================================
来源：http://hz.shuidangran.top/gtuzjynagg.html

E. 字符串处理
来源：http://hz.redwolf501.top/gtgsnnmzyt.html

================================================================================
来源：http://hz.cheryme.top/gtochecgom.html

[E01] 拼接字符串
来源：http://hz.yuxming.cn/gtblzhblry.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gtgzkozguu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.cdnleiting.top/gtmjmqrcji.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yangfankeji.com/gtlpbcsgby.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtxlgbmrzr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxinkj.top/gtohzsxjke.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xinyue.icu/gtnwlwekuo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.hfpthk.cn/gtjcomjiyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtebdzeloe.html

[E02] 重复字符串
来源：http://hz.hfpthk.cn/gtjydwcfiz.html

Py:   "ab" * 3
来源：http://hz.xuanzx.com/gtvkngytoj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.andypj.xyz/gtiyizxzwv.html

JS:   "ab".repeat(3)
来源：http://hz.xziqi.cn/gtnotwqnnk.html

TS:   "ab".repeat(3)
来源：http://hz.cdnleiting.top/gtfxhehqps.html

Java: "ab".repeat(3)
来源：http://hz.yueranfly.top/gteltilorf.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yvedp.cn/gtzqjvfxny.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtyyiihozj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.hammf.cn/gtxkmglyez.html

[E03] 截取子串
来源：http://hz.andypj.xyz/gtaqepstzh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ydjk.org.cn/gtmuoobjxe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtyeydrfta.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.meibo888.top/gtikqsduyh.html

TS:   s.slice(1, 4)
来源：http://hz.dashuyun.cn/gtqwlpgiel.html

Java: s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtqtxwsdja.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinghuilouyu.cn/gthwtognng.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yuanzhike.top/gtyljmygzw.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtjajdaeuw.html

[E04] 查找子串位置
来源：http://hz.sysykeji.top/gtzmfbicfy.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cqqwz.cn/gtbsvwxrqf.html

PHP:  strpos($s, "x");
来源：http://hz.yonumen.top/gtiqxvfhdd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtbeqtvfls.html

TS:   s.indexOf("x")
来源：http://hz.tianlin.xyz/gtiudkvolf.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtemfkgfjx.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtczuzidne.html

Ruby: s.index("x")
来源：http://hz.shangyingyoupin.top/gtrswqqqtp.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtjjxhhbfk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.kuanghao11.cn/gtdcbumlpr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhoulong.xyz/gtlgtglxdh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tanke756.top/gtwqfzmhbz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtoqkiuflq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gteerghhck.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xylfe.cn/gtvaapnfqi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zdqjudy.top/gtolslntrh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtqrsqhdeo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gtghuzetfv.html

[E06] 替换子串
来源：http://hz.ivvv.top/gtzzjhyxfo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yvedp.cn/gtadsqcsml.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.redwolf501.top/gtifzkqsbn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.chenlongwang.top/gtfyurmxhi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtadodyaab.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.dashuyun.cn/gthpjmjlbu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.guannengcc.top/gtnkbckhcv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xylfe.cn/gtlgzfetpi.html

C#:   s.Replace("a", "b")
来源：http://hz.ppjwa.cn/gtxefjbpdh.html

[E07] 按分隔符拆分
来源：http://hz.ybcxt.top/gthxkrudrn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yangfankeji.com/gtdgxrfplw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.aizwys.cn/gtyjpxbtom.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ehwqpu.com/gtksmlkaok.html

TS:   s.split(",")
来源：http://hz.chenlongwang.top/gtpekijraq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sxryk.cn/gtitfelcmg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtsboqpxna.html

Ruby: s.split(",");  s.split
来源：http://hz.dianchejie.cn/gtbmucmvno.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.sxryk.cn/gtxxsrwcor.html

[E08] 数组按分隔符合并
来源：http://hz.9152youxi.cn/gtjxvhcvoc.html

Py:   ",".join(items)
来源：http://hz.meibo888.top/gtazxqynnl.html

PHP:  implode(",", $items);
来源：http://hz.ybcxt.top/gtgomixlus.html

JS:   items.join(",")
来源：http://hz.sufxvd.cn/gtzfowhcey.html

TS:   items.join(",")
来源：http://hz.svipenyu.cn/gtewyoipsr.html

Java: String.join(",", items)
来源：http://hz.snrcjt.cn/gtizjatqxm.html

Go:   strings.Join(items, ",")
来源：http://hz.cucudq.cn/gtiihssrcm.html

Ruby: items.join(",")
来源：http://hz.daxiang520.top/gtwvcwafjf.html

C#:   string.Join(",", items)
来源：http://hz.yuxming.cn/gtnhhninco.html

[E09] 去除所有空白字符
来源：http://hz.shanyushiyangtech.top/gtxermcaon.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.shanyushiyangtech.top/gtldzjeukx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtwhdarbtu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.quarkkingdee.top/gtpfzvglae.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gttlijkouq.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.c1oappe.top/gttuzhuspp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.jqgufenzy.top/gtsqcgexba.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hnqzz.top/gtfmjaipzr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jlsjyb.cn/gtubwvodfj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtlbjmusiu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangdashe.top/gtrssefovc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guowangkeji.top/gtthupfrxz.html

JS:   "7".padStart(3, "0")
来源：http://hz.zhaomingkeji.xyz/gtapwwylam.html

TS:   "7".padStart(3, "0")
来源：http://hz.316326.xyz/gtiqllmvse.html

Java: String.format("%03d", 7)
来源：http://hz.tianlin.xyz/gtrpmyknpf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydjk.org.cn/gtmlijhaga.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.tian-w.cn/gtlpespobz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.jinyuanbaomall.cn/gtnipfisjw.html

[E11] 反转字符串
来源：http://hz.jianghu66.top/gtvqbyuejp.html

Py:   s[::-1]
来源：http://hz.316326.xyz/gtsmlaptrv.html

PHP:  strrev($s);
来源：http://hz.pengpengdd.cyou/gtppamwvwr.html

JS:   [...s].reverse().join("")
来源：http://hz.dianchejie.cn/gtyntejpfa.html

TS:   [...s].reverse().join("")
来源：http://hz.nwbrower.top/gtxuljyniy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.gzhubu.top/gtwykmcxce.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.tianlin.xyz/gtguovvljg.html

Ruby: s.reverse
来源：http://hz.zhiwuduotai.top/gtkloobbfz.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhiwuduotai.top/gtkbivporo.html

[E12] 统计某字符出现次数
来源：http://hz.daria6918.cn/gtfhaqmmqu.html

Py:   s.count("a")
来源：http://hz.yuanzhike.top/gtuvtvkgrw.html

PHP:  substr_count($s, "a");
来源：http://hz.cashguo.top/gtmnualkbz.html

JS:   s.split("a").length - 1
来源：http://hz.cucudq.cn/gtmynoobkc.html

TS:   s.split("a").length - 1
来源：http://hz.guowangkeji.top/gtnhlwctxg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtfmwhwodf.html

Go:   strings.Count(s, "a")
来源：http://hz.aibaodan.cn/gtlmgoewqn.html

Ruby: s.count("a")
来源：http://hz.wangshuangyany.cn/gtkjptkgcc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.316326.xyz/gtdybnktpl.html

[E13] 逐字符遍历
来源：http://hz.cqqwz.cn/gtmrfiouvm.html

Py:   for ch in s: print(ch)
来源：http://hz.mhx1999.top/gtikbfxhpz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.wangshuangyany.cn/gtodwzulff.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxinkj.top/gtdikbooxq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtpsoddkae.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hywenlv.cn/gtsngohyht.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yonumen.top/gtpudkgpxh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinqigfzy.top/gtlqhxwxbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.meibo888.top/gtbdkhhsmg.html

[E14] URL 编码与 Base64
来源：http://hz.cashguo.top/gtdvnjcejg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yueranfly.top/gtosrsveie.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.fengsongda.top/gtrgpxjuhx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.aizwys.cn/gtmuxwuops.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guannengcc.top/gtbpupmcwv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhiwuduotai.top/gtuzsbbmwf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jlsjyb.cn/gtzbsdrybs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ydzc1.top/gtiincjypd.html


<!-- 参考信息 -->