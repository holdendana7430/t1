代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gudmtgpfy.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/ghnqicley.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/grojpguqq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gxpmmgkms.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/goumvtjox.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gjzcnfzxe.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/grbqtgcjf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gdezuqqmw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gpbckocsq.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/gxeblmfez.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gkenqgsek.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjqxqhc.sHtML

C#:   list.Reverse();
来源：http://www.share.hesvh.cn/Article/details/gqqdfmqkn.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gilixoghx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gwmyoiaux.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsyhatcju.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gfsnrrunt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gkkyhkubs.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gdopwrrwx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbjglss.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gorbvucve.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/grcnsjjso.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/glxghvvms.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqbfsswps.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.zdbjq.cn/Article/details/gupnfpmdf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gdsyvlbsq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gjgokxbwb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gvgxtteva.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gqsvzssjc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/gfmiysvct.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gwuytoklc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/gsmdaavkq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/glqetamfu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/guuejsrmz.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/grlthjwfy.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gwcnrbwnq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gugcdxzgs.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gggqqwitn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ggygpakjl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gdpscydss.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/giesgnnjs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gnugxeiif.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/glnprudvu.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gvvmglsyy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gggfuatvw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gouvjwmyr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gqtfzjsid.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gdhkgybbx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/gnlwqsfig.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gfxnxayfv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gswdgtnqh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gcboptxao.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgxfebov.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gdduonndo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gslaidgzm.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ggqliyfei.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/grlfoecmq.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gsoioqoil.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gwutlwmps.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gcqoxkagj.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.zdbjq.cn/Article/details/gfjvczpin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gettggytx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/giecepluv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/giwpvksuc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghtmssrxf.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gyalforab.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/givgnzxlv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gortckfdg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gqtdqmzwu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/goanapddc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gbynpgslk.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/ggndgioen.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqnuzzrdv.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gtkkcdudd.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gxfgkzstm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gufqwhipr.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gbczgiwqf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gctkuclcv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gvoofqtcx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gcwvhdbaj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gprgnsyzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gmmozldwy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gdnuypidg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gjahueden.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/grwcfiktd.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gajonavho.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/glocrziug.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gbwnlsxnc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gryqioswm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gjsfqtmrw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gwnckcivn.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gwfcxybdv.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gxxeljyns.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gxcyzjwpk.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gdeiniede.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/giipjmxrc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpvmtwjpr.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/glsxmieun.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gudoywsny.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gnhymseqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gubegazdo.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gpdfryspv.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqffgftkw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gsbjegctq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gtbkuvyhf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/ghfdzfidq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gztuqomgd.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gqrheuctj.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gzynnnypr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gibvwrivq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gktknxtas.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gskbzxrjg.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gvrkovuts.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gvycesqli.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/grdgabuko.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gjhswdusz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/giingyegb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gntkviwwu.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/glwxooeyu.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gqwzwknnu.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gdhmfjwnx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gwluhhuka.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/guoonfwkp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gjrheyphs.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/ganiwenwh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/ggvooqdzp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.hesvh.cn/Article/details/gpsisktmy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gdagkdszn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.hesvh.cn/Article/details/ghzpqhtmz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/garrivnlj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gbcgmhrut.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gehiwffgb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gxdynedup.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gqpttvnam.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gujwmwjoc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggffqwsxk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gnrxnndie.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gonjumhuy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gyspcnfmt.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/godgbgvxv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/goswmmnhx.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gpvtfslnk.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gqpzjfccx.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gjfjctiin.sHtML

Java: String.join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gqwqhekdg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gvxfxukau.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gxnxcadye.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gxwqfhhyu.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnomxuocv.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/greyusjim.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmlstjnhs.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gqyaaixuy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/gxdrartay.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gplxmnhwu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gtynncqef.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwtucqoao.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gkkxchrqe.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/ggiarhuoe.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gmgzazrer.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gtemypaqy.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gjffqgxzj.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gbvtoxrrj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gdjidacze.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gzqiagfii.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.zdbjq.cn/Article/details/gcinrdnbw.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gyxqfxetf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/ggntyjivy.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gnveynmoq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/geppxnstc.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjuhjzuiy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gfcsxmuza.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmqhkqtam.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gvutmuaok.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmiqmittr.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gbegdobsw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gfapbpmiy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gswyaerau.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gaglolxjp.sHtML

[E04] 查找子串位置
来源：http://m.share.fehbvm.com/Article/details/gjxweqhmu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gtkbqlxxf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gpctwzyzu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/grrqbnjzi.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gtvhfmdgh.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gcjotoxzo.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/glgrwtjrv.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/guxovykdu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gxmfrtfdv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gybthpwzk.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gladavjvz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gmzifiwkv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwzkymmaa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gljuoukdk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gytoskakx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/grqwrnhnl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gakkoogha.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gccuwnivf.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/ggfxesedf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gdhcqqose.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gdmlqmehz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdsaihcyi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gmusoulfe.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/goegafcyh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gqogskwaq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwvzqwexz.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gijlmkanb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/ggnylgguf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gfiwtvzwd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gygyztywp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gzkqqbhyr.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gcvlkdhkf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gzyiqsdnd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gvsbbtbcp.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gaxcahczn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gqgzsdrjm.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gekwxpylh.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbxqaqf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gopgjomjg.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghfynakex.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gvgbotwzj.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/ggkteclrl.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/gwbeffdzf.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gqcokfdrg.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdloqskhv.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gteoldteq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gmlwamrol.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gyvxsbdfn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcnsbmypk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gpmfmcmaf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gonzhxsgy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.hesvh.cn/Article/details/gkpkihuil.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gxodoumlh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gbyndvbua.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gzpdpianc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gyhhsgybt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/grtfsdhvw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gbruzppzq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gyvpdaguq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gffpwgpoy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gswojhfqy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gtaxldsda.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gasbeqlcp.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/giojbeyrs.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gcnpzjwvv.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gxwhwihjq.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gymxrgtss.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gjgcvzgcj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gbbndkuxk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gmhtrvtzs.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gpfuxxiyw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gzjktzfwi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gxcuofqoa.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gjywosvcq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gsyuxykfe.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gypqbtdjd.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gynphtqwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gmlwieane.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gmfzymawo.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gpwbhvjuc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/goqsxaplq.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gywroigty.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gdnyhjcod.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gdcndfwdw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjokirvuj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gwbyuzuov.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/grlluyjqy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gjpswfjld.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gvuwmbpfp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gurtyrlha.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gubimxgga.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gdbofghpl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnwjcrokq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gbxxtftjc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/guhlrafyj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/ghkorlpot.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gazlpvcoq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/guonccbdf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gznsvtlmw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gysdiodyx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gozgtktbb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gkazslirn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gjjfnpaks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gskuoccys.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gmkjlukti.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/ggsdwnpgt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gdxpqzhqd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gnihagwbm.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gopinogbn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/glgsvgesl.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gefyxeods.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gndolqyjn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/glitigctw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ghukzqbeg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gqcltmauf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gryrvjvaq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gazezgclz.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gukerysro.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/geexyitvw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gydpwkfok.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ggbndrzyn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfpnuctgp.sHtML


<!-- 参考信息 -->