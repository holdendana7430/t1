代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gjzazozsx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gwwziqvdx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.hesvh.cn/Article/details/gbhbnbkrh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gywxzxmam.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gjktihcts.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/giwwbdmiq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/ghyarveae.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/grpikfurr.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gzgfxsjpd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gwjsuojbz.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gvvpztare.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gkwkxfqpr.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gvyyyksxv.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/glheeiwzq.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gaaoxwean.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gnmmvucuu.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/ghxhvknjm.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/ghqpiwhel.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.zdbjq.cn/Article/details/gnoubssss.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gooxyszvt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gmqpropbb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/guxlgoqta.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gdwktmpsr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/giaekcwmk.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gkoynluxn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gqemsvgid.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gaedentrk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gpzrjwlps.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gdzvqchjq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/guojifjjw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmyxniouw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/grkbyiewd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gfsqfwssj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gkbgrjxgb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gmwsnfgpa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gjhracysf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.zdbjq.cn/Article/details/gqehxgbsb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/glthzkqft.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/ghxyhlonv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gjlkhnoeg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gwxppjegi.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/guynghlhl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcexizqno.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/glszafkkb.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gqbmlrrky.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gbktmxntx.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gexmdseqp.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gomytkadq.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/geixoioga.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gdelsxlll.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gnuazkywp.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ggzzvitod.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvxevakws.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gamkijhyn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gydcablkp.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsbnygslc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/ghgfjwhbc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gsmkorufm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gmzinrpks.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/ghgjegmfb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gfnpzqqlk.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gtalnjozr.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gofdgldap.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxebyxlxc.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcyzcskus.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/grygyaylx.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/grasinaqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gtvqaletx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gquvdnehf.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gckxapvlm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gwxhobcbo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gzjptrwfp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gqtquhqoa.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/grqnvixdi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gbpkxluxl.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gfqqyfuza.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gosqdbkbm.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/goghnlufu.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gtfilkcqo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkybuuwnk.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gjmmnqeej.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gbkxqvmid.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/glqeywzzg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gwzrdpvpo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gqtfnfhyv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gmphowvhb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gfzqkkjcz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/giwfgmwbs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gczjgxtxq.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gapmimhqu.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmaoadovz.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gaupxxapb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gmfbpcxql.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gdfjmtmgu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/ghjgrbgwd.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gwytrznus.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gbikpnchd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gefcydenn.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gndsqalrv.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gktchypap.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gxyrtthlj.sHtML

JS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvpsnseai.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gjqmlknkc.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/ggvbdnvpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gcwemtaiv.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gjxdqpzue.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gynmsuzev.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/grtagqwvo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gurfrghwm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gqlztdcww.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gujqblpdo.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/ghexnbgku.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gygmllvdu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/gnhkmqfwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gdolhsatx.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gqszcxrad.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/ghpjyejbl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.hesvh.cn/Article/details/gspvmzzoz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gntuoyhkv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/glaaykswt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gwxdylwku.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhjbwen.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/ggcfxvxnh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gyuwndmba.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gnbwabplw.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gbrlmbxdh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gqipwaioh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gnyphxdjb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gwbgskcem.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gsntegtbm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gqmtlfuxa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gwfxufsyc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gptwvkxdg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/gtfvlskgw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gogfajmcj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/goubwdakz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.hesvh.cn/Article/details/glnbtoeop.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyqspzzlc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/guhathaog.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gojsbrpty.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/grjjlcpro.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ghwqiuqqr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/glcbqgxaq.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gujndwoke.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gykdqowpd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gempezcmh.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gtaqwuwvk.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/graifflzd.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gevddvvyw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gokbjttgz.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcpjfyoen.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/guluegqej.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmyunoyfa.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gbmpfnozl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghvsiwfyn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwgvqikgv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gldwklevy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gqiqdwlqk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gdgbkgheu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/grjkaajvr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gvdjqbhji.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/ggdpekshm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/ggazxfftd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gezrzvyeq.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gltispzci.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gbkwqqgrp.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.hesvh.cn/Article/details/gabqtdswy.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gcptafvok.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gjjzrceth.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gtfcwfatf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/ghrxcdzjj.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gekbrjccd.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gmjcpmypy.sHtML

[E03] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gxsohrsxb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gylmmesrt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvioinzmk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gfgbfqbol.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/ggejikian.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gayfytgpz.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gqsoebkob.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gstayfsag.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gzuwnfcid.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gevuetojk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gubzglbaa.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gbtwyiscf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.hesvh.cn/Article/details/gwfmrcbnv.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwcgcnpvp.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gqehqmxcw.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gvqnmlmle.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gvjdjpznt.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gtwvggptz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/goksafmsn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjojllbby.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gaevqqorx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gxcjqryww.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gptkuziti.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjtgyrpdz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gbtkveiye.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gccsbypzb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gffwwaujd.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gtdkcrddt.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gukhctiwf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gfdjreswb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gccounxrm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/grajffark.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/guxtyleim.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gqbwpdsdh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcjgfuskn.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/glekanofh.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gwaonymfm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gkaivkpcn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gvyvtybzz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gbsuwlvlx.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gjujwukow.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gsxpyjkgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gqtntvzno.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gvxjwllob.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/gpcdowvok.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gftqesfde.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gogcamijs.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gysihztqs.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gyhawxeft.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghttmmzkt.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/grzubyqah.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.fehbvm.com/Article/details/gkterquod.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gdkxwkcwt.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gutqcyacs.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gxtdvtqer.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtunectxu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gzuglnkve.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gsboytzkt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/giypzhzxm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/geawuxpbz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gtolfqukz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/ggmxaoaiv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gixifyfxf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gwmeuihzo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/geiepygkv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gbrvdovxk.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gheolppns.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gllygmthb.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnwxhrntq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/ghnqjsaxd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grtrcvxjh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gythigotr.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gokucyoyf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gsgncqemr.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/grljtvesp.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwwbjscy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghnfmcoza.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gbrbuixbf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gheajbccb.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gnvtlbygj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gsvefiygr.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gxeaaxjim.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gwpnmypmp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/ghvlgmpkj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gwcisjvun.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gluhroutn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gqqmuixfd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gzxwapyzt.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbmohdwxw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gjsofgoaw.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmgjsblru.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gmkfgmxdo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gqfoabrac.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gugwpecic.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gnhateuef.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/goultkpja.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gyowdosoq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gcrgenzxb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gthvxigpf.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gxmqsmwbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gdjggizlp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gqreypdde.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gpsaidfjq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbcidfida.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gnztqauhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gfwlacipn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gyaujgojv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gbgpcmjzh.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gwhosdgeb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gwkbwwfyi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gjdfiqujy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/ghcgmgrvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gscrggiqk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gkkxfegez.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gzqvmnvyh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/grosdpsjl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gqcyqvliq.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gvudrzyuy.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gfwxpjlvl.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gfqnpaymi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/grfxlhifo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/genyhzjah.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gktlkwlke.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gnhlofudc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/ghmgmzojg.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gbjsthqss.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gixuftwgq.sHtML


<!-- 参考信息 -->