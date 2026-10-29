代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/givwenqsu.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtiowqeul.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gppvpzmsy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/giaxkwqjj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gabomblxo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gjxjtcrtm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/givmersqr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gtjsakatm.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gooneussr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gdzuypohb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/grkmdovwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gecuecliz.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gtfmrswxl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gxyrweimv.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gzviscknm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gniretrgy.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.zdbjq.cn/Article/details/grkoddgpm.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gasxrlmin.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/guikipbcj.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gamindasx.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gcvsqezol.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gexnezmnh.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gktldccsi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/grrpqslqn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/ghkidiuwx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gzekwfaue.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gnwfpgmyk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqvimopcc.sHtML

Ruby: arr.index(x)
来源：http://blog.zdbjq.cn/Article/details/gtdvdfsvo.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/ghxukziyn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gyravkqvp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gncrcityu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gmachsmgv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gzxvvsmcs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gwoppxxlh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gshhxrvlh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gjfjvhzjd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.hesvh.cn/Article/details/gemiqfhes.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gmuvmhdkt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/guyrzdltd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gtdqswfvz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gomaayjhf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gmwekcrlb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gvkciaoah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtnyhhkwg.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gqjymbycz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnmyqdqiv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gamavddpf.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/guksbxqcg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.hesvh.cn/Article/details/gvozgycbi.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gshbeafwe.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/glxdfmapp.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gwnjmnmuz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gmaartelf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gkciaenxy.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gpcjocqlc.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/giihltgil.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/grzhihxkb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gjyypgaus.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gjbhippyf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gbcmlapdc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/grexhiuhe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gjaejoicx.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gbvhrcran.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gpiyzwxig.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gliswxsvd.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gedmaljmx.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gnlpmzpjo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdbylrbdl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/grkcepqvn.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gdmsqjbob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gsihhwesb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gccwazzsy.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gpfqurucl.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gbkvekwrr.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gypjudnik.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gbijhdbtj.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gdymvtoqo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gaxvexkpy.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gagrylxts.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/giryjejrk.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gztptoxdz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gigtbexuj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gwjkqyqjm.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvbxogt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gqeqdkrkd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/gunchyuks.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gojbwrvyt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gmexmqkfg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gzhoasnab.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gpibaxnpx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gslbeolzp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gpvlrowzl.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gsdbdiezc.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gpguthgyd.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjpkswhub.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gqplbtvnq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/grnrrrytj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gykasocpg.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gvcfinver.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/grukkxmgs.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fehbvm.com/Article/details/gjxuxspfb.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gnrgzzmcs.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/ghedvvhwx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gxednuwyw.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gcvwgawkp.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gkqdkuxlh.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gtnpufzyq.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gsmlfiuxs.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/ghkupsbyj.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gpbtzvszn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.hesvh.cn/Article/details/gwpwjldkd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gnydffnzu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gydmkzjkw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gfharouml.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gpuwdrqsf.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gpirbwzvr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gedrieirv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gnaayjmia.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gkswqcxnq.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gmbkezvej.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gpqacatgk.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/glfojbnlc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gbiwxlxpz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gvidfgcki.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gwsxhqwdd.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gprsvsakg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gmzlefevr.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gygkobshz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.zdbjq.cn/Article/details/gnizkixgs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbdroqy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gsvmzvmdb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/girkyjicc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ggqgwgzhb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gegmlseeh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/guycoublf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gldmpagdg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gptlgtpau.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/gpkyxhxor.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/ghzvlmdde.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gqkpiwqol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gylvflfth.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gepukhsvd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsevhsgmq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/gydlanqoi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/glgtrekqq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/glldjopif.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gwesjvntk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gnwmnbwrn.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/glxskldrf.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/glytbfufx.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gtpjrpmsa.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/ghramuiot.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gcyahgcvs.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gqudbigfd.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gmrwzinus.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghcwzqdbm.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gynhkszyn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzowzstqw.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gajhsimws.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/goalakiuy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gahdeglmh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gcicvfjtg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gelvzuwob.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/grsycwluf.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gintfpapt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gtaducnaz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gfpnfupoz.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gmgmppnya.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/ggkpnofbo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gtgobmprx.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gihoyakzo.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzdtiwtsu.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gmpjhougb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gamilvici.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/ggiluzfdv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/ggddknmxg.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gjdckirji.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gcpmknucm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/grrvbdqon.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gkgtbbgvp.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gxhawgiln.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gskcdmzkv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gvcieadpu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gbjyhwlqm.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gjavccsdc.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gciwpbpkb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/guhlxeqtx.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gwlamovgx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gnwhpbjxh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gcwfsagwc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ggynspwzd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gxzpfszvf.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/grdrbrcax.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gznxuqhvo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gimmwxlqg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gzcdaaicu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fehbvm.com/Article/details/gtqcowzmq.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/grzsvgxiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gjhkxqikc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsxxcaczk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gmlknadyi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gautdlbum.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gjukuegih.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gegiphkjf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/glmoqvpep.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gzpyzejnx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpglhxdmv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gqgkscspw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gckyautwm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gbwlzqamv.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gzmkougky.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gythxkmre.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gcjtkxxwm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/geqcprdqf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/guuxrutlv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gxegfrbts.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gpnrljsqq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/glowzzisx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gcdwdfcgs.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gnkyxhjxo.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gzydlwuyn.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gqgicbyvw.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gddqbwebf.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gesqyggdi.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/grosiczhn.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gsrzbjena.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/guxntohkd.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/glmqyfmhc.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gmrcdcygh.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gyoxmcwiw.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gyiqqmshy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gqrstquuc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gxgemfwfa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gvaahdobb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/glzhihksq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gxohwmwwq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gsbqttywo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gbehdqdod.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gvbtgeegk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gsqfqlmnj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gqrrujmuy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gsgnjjihg.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/guekjxkem.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gxfabkfsi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gcfwarmku.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjduwgwff.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gzkeeyabx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/grgnpkzoy.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gddaeamep.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gsiaegdnv.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gogdrfvxt.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gejwdjyyp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gambaratv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gnobhypkx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gcsbgdnsu.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gicziusep.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gfwxltjsb.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gwamyjuza.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/grgmuxekt.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gopoiayow.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gstpdyvuj.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gzualfmbp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gpffnvlec.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gnhvsedlc.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/grpvswhtv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gtpmutsva.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gqhygxrxh.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gcpqgeeqa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gkgokxfzk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfgaugirn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gmwdhatcg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gaggmvxcj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gntafzndt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gezjrqeva.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gmsxdoacm.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gnzogwhox.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gjoizdcem.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gbrvzoyje.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/ghxgxwhck.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggclgknkv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gjdjmtitr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gwdnpglip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gwdgwocaj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gcwozvqcq.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gtghuxoij.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gozeddsar.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gocjvdmvq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/ggndvzgpg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/ghcekkqun.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gtrqtzkep.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gfgclrbbk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gguacdipf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/ghbaiqdiz.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/godgyidtk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gcjhvclfz.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gqjcsuavi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/glxqrmykb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gzrebabwb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gnzthhhty.sHtML


<!-- 参考信息 -->